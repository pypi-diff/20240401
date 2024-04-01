# Comparing `tmp/allure-behave-2.9.44.tar.gz` & `tmp/allure-behave-2.9.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allure-behave-2.9.44.tar", last modified: Wed Sep 29 20:24:24 2021, max compression
+gzip compressed data, was "allure-behave-2.9.45.tar", last modified: Fri Oct 15 08:22:17 2021, max compression
```

## Comparing `allure-behave-2.9.44.tar` & `allure-behave-2.9.45.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:24.065609 allure-behave-2.9.44/
--rw-r--r--   0 runner    (1001) docker     (121)     2141 2021-09-29 20:24:24.065609 allure-behave-2.9.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2021-09-29 20:24:05.000000 allure-behave-2.9.44/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:24.061609 allure-behave-2.9.44/allure_behave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2141 2021-09-29 20:24:23.000000 allure-behave-2.9.44/allure_behave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      711 2021-09-29 20:24:23.000000 allure-behave-2.9.44/allure_behave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 20:24:23.000000 allure-behave-2.9.44/allure_behave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-09-29 20:24:23.000000 allure-behave-2.9.44/allure_behave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-09-29 20:24:23.000000 allure-behave-2.9.44/allure_behave.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:24.061609 allure-behave-2.9.44/features/
--rw-r--r--   0 runner    (1001) docker     (121)     1753 2021-09-29 20:24:05.000000 allure-behave-2.9.44/features/background.feature
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2021-09-29 20:24:05.000000 allure-behave-2.9.44/features/description.feature
--rw-r--r--   0 runner    (1001) docker     (121)     7425 2021-09-29 20:24:05.000000 allure-behave-2.9.44/features/hook.feature
--rw-r--r--   0 runner    (1001) docker     (121)      420 2021-09-29 20:24:05.000000 allure-behave-2.9.44/features/label.feature
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2021-09-29 20:24:05.000000 allure-behave-2.9.44/features/link.feature
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2021-09-29 20:24:05.000000 allure-behave-2.9.44/features/no_skipped.feature
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2021-09-29 20:24:05.000000 allure-behave-2.9.44/features/scenario.feature
--rw-r--r--   0 runner    (1001) docker     (121)     5438 2021-09-29 20:24:05.000000 allure-behave-2.9.44/features/scenario_outline.feature
--rw-r--r--   0 runner    (1001) docker     (121)     2158 2021-09-29 20:24:05.000000 allure-behave-2.9.44/features/severity.feature
--rw-r--r--   0 runner    (1001) docker     (121)     2766 2021-09-29 20:24:05.000000 allure-behave-2.9.44/features/step.feature
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:24.065609 allure-behave-2.9.44/features/steps/
--rw-r--r--   0 runner    (1001) docker     (121)     2526 2021-09-29 20:24:05.000000 allure-behave-2.9.44/features/steps/behave_steps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2021-09-29 20:24:05.000000 allure-behave-2.9.44/features/steps/dummy_steps.py
--rw-r--r--   0 runner    (1001) docker     (121)     6256 2021-09-29 20:24:05.000000 allure-behave-2.9.44/features/steps/report_steps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2021-09-29 20:24:05.000000 allure-behave-2.9.44/features/tag.feature
--rw-r--r--   0 runner    (1001) docker     (121)     3661 2021-09-29 20:24:05.000000 allure-behave-2.9.44/features/test_plan.feature
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2021-09-29 20:24:05.000000 allure-behave-2.9.44/features/unicode.feature
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-29 20:24:24.065609 allure-behave-2.9.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1808 2021-09-29 20:24:05.000000 allure-behave-2.9.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:24.065609 allure-behave-2.9.44/src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-behave-2.9.44/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2021-09-29 20:24:05.000000 allure-behave-2.9.44/src/formatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1977 2021-09-29 20:24:05.000000 allure-behave-2.9.44/src/hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     9753 2021-09-29 20:24:05.000000 allure-behave-2.9.44/src/listener.py
--rw-r--r--   0 runner    (1001) docker     (121)     4769 2021-09-29 20:24:05.000000 allure-behave-2.9.44/src/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2116 2021-09-29 20:24:05.000000 allure-behave-2.9.44/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:17.776848 allure-behave-2.9.45/
+-rw-r--r--   0 runner    (1001) docker     (121)     2141 2021-10-15 08:22:17.776848 allure-behave-2.9.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1186 2021-10-15 08:21:54.000000 allure-behave-2.9.45/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:17.772848 allure-behave-2.9.45/allure_behave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2141 2021-10-15 08:22:17.000000 allure-behave-2.9.45/allure_behave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      711 2021-10-15 08:22:17.000000 allure-behave-2.9.45/allure_behave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-15 08:22:17.000000 allure-behave-2.9.45/allure_behave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2021-10-15 08:22:17.000000 allure-behave-2.9.45/allure_behave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2021-10-15 08:22:17.000000 allure-behave-2.9.45/allure_behave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:17.772848 allure-behave-2.9.45/features/
+-rw-r--r--   0 runner    (1001) docker     (121)     1753 2021-10-15 08:21:54.000000 allure-behave-2.9.45/features/background.feature
+-rw-r--r--   0 runner    (1001) docker     (121)     1037 2021-10-15 08:21:54.000000 allure-behave-2.9.45/features/description.feature
+-rw-r--r--   0 runner    (1001) docker     (121)     7425 2021-10-15 08:21:54.000000 allure-behave-2.9.45/features/hook.feature
+-rw-r--r--   0 runner    (1001) docker     (121)      420 2021-10-15 08:21:54.000000 allure-behave-2.9.45/features/label.feature
+-rw-r--r--   0 runner    (1001) docker     (121)     2120 2021-10-15 08:21:54.000000 allure-behave-2.9.45/features/link.feature
+-rw-r--r--   0 runner    (1001) docker     (121)     1219 2021-10-15 08:21:54.000000 allure-behave-2.9.45/features/no_skipped.feature
+-rw-r--r--   0 runner    (1001) docker     (121)     1693 2021-10-15 08:21:54.000000 allure-behave-2.9.45/features/scenario.feature
+-rw-r--r--   0 runner    (1001) docker     (121)     5438 2021-10-15 08:21:54.000000 allure-behave-2.9.45/features/scenario_outline.feature
+-rw-r--r--   0 runner    (1001) docker     (121)     2158 2021-10-15 08:21:54.000000 allure-behave-2.9.45/features/severity.feature
+-rw-r--r--   0 runner    (1001) docker     (121)     2766 2021-10-15 08:21:54.000000 allure-behave-2.9.45/features/step.feature
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:17.772848 allure-behave-2.9.45/features/steps/
+-rw-r--r--   0 runner    (1001) docker     (121)     2526 2021-10-15 08:21:54.000000 allure-behave-2.9.45/features/steps/behave_steps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1184 2021-10-15 08:21:54.000000 allure-behave-2.9.45/features/steps/dummy_steps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6256 2021-10-15 08:21:54.000000 allure-behave-2.9.45/features/steps/report_steps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1377 2021-10-15 08:21:54.000000 allure-behave-2.9.45/features/tag.feature
+-rw-r--r--   0 runner    (1001) docker     (121)     3661 2021-10-15 08:21:54.000000 allure-behave-2.9.45/features/test_plan.feature
+-rw-r--r--   0 runner    (1001) docker     (121)     2177 2021-10-15 08:21:54.000000 allure-behave-2.9.45/features/unicode.feature
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-15 08:22:17.776848 allure-behave-2.9.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1808 2021-10-15 08:21:54.000000 allure-behave-2.9.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:17.776848 allure-behave-2.9.45/src/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-behave-2.9.45/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1561 2021-10-15 08:21:54.000000 allure-behave-2.9.45/src/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1977 2021-10-15 08:21:54.000000 allure-behave-2.9.45/src/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9753 2021-10-15 08:21:54.000000 allure-behave-2.9.45/src/listener.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4769 2021-10-15 08:21:54.000000 allure-behave-2.9.45/src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2116 2021-10-15 08:21:54.000000 allure-behave-2.9.45/tox.ini
```

### Comparing `allure-behave-2.9.44/PKG-INFO` & `allure-behave-2.9.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allure-behave
-Version: 2.9.44
+Version: 2.9.45
 Summary: Allure behave integration
 Home-page: https://github.com/allure-framework/allure-python
 Author: QAMetaSoftware, Stanislav Seliverstov
 Author-email: sseliverstov@qameta.io
 License: Apache-2.0
 Keywords: allure reporting behave
 Platform: UNKNOWN
```

### Comparing `allure-behave-2.9.44/README.rst` & `allure-behave-2.9.45/README.rst`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/allure_behave.egg-info/PKG-INFO` & `allure-behave-2.9.45/allure_behave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allure-behave
-Version: 2.9.44
+Version: 2.9.45
 Summary: Allure behave integration
 Home-page: https://github.com/allure-framework/allure-python
 Author: QAMetaSoftware, Stanislav Seliverstov
 Author-email: sseliverstov@qameta.io
 License: Apache-2.0
 Keywords: allure reporting behave
 Platform: UNKNOWN
```

### Comparing `allure-behave-2.9.44/allure_behave.egg-info/SOURCES.txt` & `allure-behave-2.9.45/allure_behave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/features/background.feature` & `allure-behave-2.9.45/features/background.feature`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/features/description.feature` & `allure-behave-2.9.45/features/description.feature`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/features/hook.feature` & `allure-behave-2.9.45/features/hook.feature`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/features/link.feature` & `allure-behave-2.9.45/features/link.feature`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/features/no_skipped.feature` & `allure-behave-2.9.45/features/no_skipped.feature`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/features/scenario.feature` & `allure-behave-2.9.45/features/scenario.feature`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/features/scenario_outline.feature` & `allure-behave-2.9.45/features/scenario_outline.feature`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/features/severity.feature` & `allure-behave-2.9.45/features/severity.feature`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/features/step.feature` & `allure-behave-2.9.45/features/step.feature`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/features/steps/behave_steps.py` & `allure-behave-2.9.45/features/steps/behave_steps.py`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/features/steps/dummy_steps.py` & `allure-behave-2.9.45/features/steps/dummy_steps.py`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/features/steps/report_steps.py` & `allure-behave-2.9.45/features/steps/report_steps.py`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/features/tag.feature` & `allure-behave-2.9.45/features/tag.feature`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/features/test_plan.feature` & `allure-behave-2.9.45/features/test_plan.feature`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/features/unicode.feature` & `allure-behave-2.9.45/features/unicode.feature`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/setup.py` & `allure-behave-2.9.45/setup.py`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/src/formatter.py` & `allure-behave-2.9.45/src/formatter.py`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/src/hooks.py` & `allure-behave-2.9.45/src/hooks.py`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/src/listener.py` & `allure-behave-2.9.45/src/listener.py`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/src/utils.py` & `allure-behave-2.9.45/src/utils.py`

 * *Files identical despite different names*

### Comparing `allure-behave-2.9.44/tox.ini` & `allure-behave-2.9.45/tox.ini`

 * *Files identical despite different names*

