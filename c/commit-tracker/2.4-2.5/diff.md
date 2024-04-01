# Comparing `tmp/commit-tracker-2.4.tar.gz` & `tmp/commit-tracker-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commit-tracker-2.4.tar", last modified: Mon Apr  1 09:58:39 2024, max compression
+gzip compressed data, was "commit-tracker-2.5.tar", last modified: Mon Apr  1 21:43:55 2024, max compression
```

## Comparing `commit-tracker-2.4.tar` & `commit-tracker-2.5.tar`

### file list

```diff
@@ -1,28 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:58:39.708581 commit-tracker-2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-01 09:58:33.000000 commit-tracker-2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-01 09:58:39.708581 commit-tracker-2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-01 09:58:33.000000 commit-tracker-2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:58:39.708581 commit-tracker-2.4/commit_tracker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-01 09:58:39.000000 commit-tracker-2.4/commit_tracker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-01 09:58:39.000000 commit-tracker-2.4/commit_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 09:58:39.000000 commit-tracker-2.4/commit_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 09:58:39.000000 commit-tracker-2.4/commit_tracker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-01 09:58:39.000000 commit-tracker-2.4/commit_tracker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 09:58:39.000000 commit-tracker-2.4/commit_tracker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:58:39.708581 commit-tracker-2.4/committracker/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-01 09:58:33.000000 commit-tracker-2.4/committracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-01 09:58:33.000000 commit-tracker-2.4/committracker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-01 09:58:33.000000 commit-tracker-2.4/committracker/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-01 09:58:33.000000 commit-tracker-2.4/committracker/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-01 09:58:33.000000 commit-tracker-2.4/committracker/plugin_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-01 09:58:33.000000 commit-tracker-2.4/committracker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-01 09:58:33.000000 commit-tracker-2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 09:58:39.708581 commit-tracker-2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:58:39.708581 commit-tracker-2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-01 09:58:33.000000 commit-tracker-2.4/tests/test_branch_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-01 09:58:33.000000 commit-tracker-2.4/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-01 09:58:33.000000 commit-tracker-2.4/tests/test_commit_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-01 09:58:33.000000 commit-tracker-2.4/tests/test_commit_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-01 09:58:33.000000 commit-tracker-2.4/tests/test_contributors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-01 09:58:33.000000 commit-tracker-2.4/tests/test_git_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-01 09:58:33.000000 commit-tracker-2.4/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:43:55.155969 commit-tracker-2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-01 21:43:50.000000 commit-tracker-2.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-01 21:43:55.155969 commit-tracker-2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-01 21:43:50.000000 commit-tracker-2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:43:55.155969 commit-tracker-2.5/commit_tracker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-01 21:43:55.000000 commit-tracker-2.5/commit_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-01 21:43:55.000000 commit-tracker-2.5/commit_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:43:55.000000 commit-tracker-2.5/commit_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 21:43:55.000000 commit-tracker-2.5/commit_tracker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-01 21:43:55.000000 commit-tracker-2.5/commit_tracker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 21:43:55.000000 commit-tracker-2.5/commit_tracker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:43:55.151969 commit-tracker-2.5/committracker/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-01 21:43:50.000000 commit-tracker-2.5/committracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-01 21:43:50.000000 commit-tracker-2.5/committracker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-01 21:43:50.000000 commit-tracker-2.5/committracker/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-01 21:43:50.000000 commit-tracker-2.5/committracker/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-01 21:43:50.000000 commit-tracker-2.5/committracker/plugin_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:43:55.151969 commit-tracker-2.5/committracker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:43:50.000000 commit-tracker-2.5/committracker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-01 21:43:50.000000 commit-tracker-2.5/committracker/plugins/branch_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-01 21:43:50.000000 commit-tracker-2.5/committracker/plugins/code_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-01 21:43:50.000000 commit-tracker-2.5/committracker/plugins/commit_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-01 21:43:50.000000 commit-tracker-2.5/committracker/plugins/commit_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-01 21:43:50.000000 commit-tracker-2.5/committracker/plugins/contributors_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-01 21:43:50.000000 commit-tracker-2.5/committracker/plugins/git_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-01 21:43:50.000000 commit-tracker-2.5/committracker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-01 21:43:50.000000 commit-tracker-2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:43:55.155969 commit-tracker-2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:43:55.155969 commit-tracker-2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-01 21:43:50.000000 commit-tracker-2.5/tests/test_branch_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-01 21:43:50.000000 commit-tracker-2.5/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-01 21:43:50.000000 commit-tracker-2.5/tests/test_commit_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-01 21:43:50.000000 commit-tracker-2.5/tests/test_commit_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-01 21:43:50.000000 commit-tracker-2.5/tests/test_contributors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-01 21:43:50.000000 commit-tracker-2.5/tests/test_git_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-01 21:43:50.000000 commit-tracker-2.5/tests/test_main.py
```

### Comparing `commit-tracker-2.4/LICENSE.txt` & `commit-tracker-2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `commit-tracker-2.4/PKG-INFO` & `commit-tracker-2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commit-tracker
-Version: 2.4
+Version: 2.5
 Summary: Commit Tracker analyzes Git repositories to present comprehensive statistics.
 Author-email: "André F. Costa" <afmcosta@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andrecosta99/ct-final
 Project-URL: Documentation, https://github.com/andrecosta99/ct-final#readme
 Project-URL: Repository, https://github.com/andrecosta99/ct-final
 Keywords: git,analysis,commit,education
```

### Comparing `commit-tracker-2.4/README.md` & `commit-tracker-2.5/README.md`

 * *Files identical despite different names*

### Comparing `commit-tracker-2.4/commit_tracker.egg-info/PKG-INFO` & `commit-tracker-2.5/commit_tracker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commit-tracker
-Version: 2.4
+Version: 2.5
 Summary: Commit Tracker analyzes Git repositories to present comprehensive statistics.
 Author-email: "André F. Costa" <afmcosta@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andrecosta99/ct-final
 Project-URL: Documentation, https://github.com/andrecosta99/ct-final#readme
 Project-URL: Repository, https://github.com/andrecosta99/ct-final
 Keywords: git,analysis,commit,education
```

### Comparing `commit-tracker-2.4/committracker/__main__.py` & `commit-tracker-2.5/committracker/__main__.py`

 * *Files identical despite different names*

### Comparing `commit-tracker-2.4/committracker/callbacks.py` & `commit-tracker-2.5/committracker/callbacks.py`

 * *Files identical despite different names*

### Comparing `commit-tracker-2.4/committracker/layout.py` & `commit-tracker-2.5/committracker/layout.py`

 * *Files identical despite different names*

### Comparing `commit-tracker-2.4/committracker/plugin_loader.py` & `commit-tracker-2.5/committracker/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `commit-tracker-2.4/committracker/utils.py` & `commit-tracker-2.5/committracker/utils.py`

 * *Files identical despite different names*

### Comparing `commit-tracker-2.4/pyproject.toml` & `commit-tracker-2.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "commit-tracker"
-version = "2.4"
+version = "2.5"
 description = "Commit Tracker analyzes Git repositories to present comprehensive statistics."
 authors = [{name = "André F. Costa", email = "afmcosta@gmail.com"}]
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
 keywords = ["git", "analysis", "commit", "education"]
 classifiers = [
@@ -61,15 +61,18 @@
 
 [project.urls]
 Homepage = "https://github.com/andrecosta99/ct-final"
 Documentation = "https://github.com/andrecosta99/ct-final#readme"
 Repository = "https://github.com/andrecosta99/ct-final"
 
 [tool.setuptools]
-packages = ["committracker"]
+packages = [
+    "committracker",
+    "committracker.plugins",
+]
 
 [tool.pytest.ini_options]
 minversion = "8.0"
 addopts = "--doctest-modules"
 testpaths = ["tests"]
 
 [tool.black]
```

### Comparing `commit-tracker-2.4/tests/test_branch_information.py` & `commit-tracker-2.5/tests/test_branch_information.py`

 * *Files identical despite different names*

### Comparing `commit-tracker-2.4/tests/test_callbacks.py` & `commit-tracker-2.5/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `commit-tracker-2.4/tests/test_commit_graph.py` & `commit-tracker-2.5/tests/test_commit_graph.py`

 * *Files identical despite different names*

### Comparing `commit-tracker-2.4/tests/test_commit_type.py` & `commit-tracker-2.5/tests/test_commit_type.py`

 * *Files identical despite different names*

### Comparing `commit-tracker-2.4/tests/test_contributors.py` & `commit-tracker-2.5/tests/test_contributors.py`

 * *Files identical despite different names*

### Comparing `commit-tracker-2.4/tests/test_git_statistics.py` & `commit-tracker-2.5/tests/test_git_statistics.py`

 * *Files identical despite different names*

### Comparing `commit-tracker-2.4/tests/test_main.py` & `commit-tracker-2.5/tests/test_main.py`

 * *Files identical despite different names*

