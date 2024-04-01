# Comparing `tmp/user-context-remote-0.0.65.tar.gz` & `tmp/user-context-remote-0.0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user-context-remote-0.0.65.tar", last modified: Mon Apr  1 19:52:34 2024, max compression
+gzip compressed data, was "user-context-remote-0.0.66.tar", last modified: Mon Apr  1 19:58:19 2024, max compression
```

## Comparing `user-context-remote-0.0.65.tar` & `user-context-remote-0.0.66.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:52:34.444853 user-context-remote-0.0.65/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-01 19:52:34.444853 user-context-remote-0.0.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-01 19:52:16.000000 user-context-remote-0.0.65/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-01 19:52:16.000000 user-context-remote-0.0.65/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 19:52:34.444853 user-context-remote-0.0.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-01 19:52:16.000000 user-context-remote-0.0.65/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:52:34.440853 user-context-remote-0.0.65/user_context_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:52:34.444853 user-context-remote-0.0.65/user_context_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:52:16.000000 user-context-remote-0.0.65/user_context_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18994 2024-04-01 19:52:16.000000 user-context-remote-0.0.65/user_context_remote/src/user_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:52:34.444853 user-context-remote-0.0.65/user_context_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-01 19:52:34.000000 user-context-remote-0.0.65/user_context_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-01 19:52:34.000000 user-context-remote-0.0.65/user_context_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:52:34.000000 user-context-remote-0.0.65/user_context_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-01 19:52:34.000000 user-context-remote-0.0.65/user_context_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 19:52:34.000000 user-context-remote-0.0.65/user_context_remote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:58:19.994881 user-context-remote-0.0.66/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-01 19:58:19.994881 user-context-remote-0.0.66/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-01 19:58:07.000000 user-context-remote-0.0.66/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-01 19:58:07.000000 user-context-remote-0.0.66/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 19:58:19.994881 user-context-remote-0.0.66/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-01 19:58:07.000000 user-context-remote-0.0.66/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:58:19.990881 user-context-remote-0.0.66/user_context_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:58:19.994881 user-context-remote-0.0.66/user_context_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:58:07.000000 user-context-remote-0.0.66/user_context_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18994 2024-04-01 19:58:07.000000 user-context-remote-0.0.66/user_context_remote/src/user_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:58:19.994881 user-context-remote-0.0.66/user_context_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-01 19:58:19.000000 user-context-remote-0.0.66/user_context_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-01 19:58:19.000000 user-context-remote-0.0.66/user_context_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:58:19.000000 user-context-remote-0.0.66/user_context_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-01 19:58:19.000000 user-context-remote-0.0.66/user_context_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 19:58:19.000000 user-context-remote-0.0.66/user_context_remote.egg-info/top_level.txt
```

### Comparing `user-context-remote-0.0.65/PKG-INFO` & `user-context-remote-0.0.66/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.65
+Version: 0.0.66
 Summary: PyPI Package for Circles User Context Local/Remote Python
-Home-page: https://github.com/circles/user-context-remote-python-package
+Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: language-remote>=0.0.15
```

### Comparing `user-context-remote-0.0.65/README.md` & `user-context-remote-0.0.66/README.md`

 * *Files identical despite different names*

### Comparing `user-context-remote-0.0.65/pyproject.toml` & `user-context-remote-0.0.66/pyproject.toml`

 * *Files identical despite different names*

### Comparing `user-context-remote-0.0.65/setup.py` & `user-context-remote-0.0.66/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 PACKAGE_NAME = "user-context-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name='user-context-remote',
-    version='0.0.65',  # https://pypi.org/project/user-context-remote/
+    version='0.0.66',  # https://pypi.org/project/user-context-remote/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles User Context Local/Remote Python",
     long_description="This is a package for sharing common user-context-remote functions used in different repositories",
     long_description_content_type="text/markdown",
-    url=f"https://github.com/circles/{PACKAGE_NAME}-python-package",
+    url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
```

### Comparing `user-context-remote-0.0.65/user_context_remote/src/user_context.py` & `user-context-remote-0.0.66/user_context_remote/src/user_context.py`

 * *Files identical despite different names*

### Comparing `user-context-remote-0.0.65/user_context_remote.egg-info/PKG-INFO` & `user-context-remote-0.0.66/user_context_remote.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.65
+Version: 0.0.66
 Summary: PyPI Package for Circles User Context Local/Remote Python
-Home-page: https://github.com/circles/user-context-remote-python-package
+Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: language-remote>=0.0.15
```

