# Comparing `tmp/gmalglib-0.1.3.tar.gz` & `tmp/gmalglib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmalglib-0.1.3.tar", last modified: Mon Apr  1 13:11:00 2024, max compression
+gzip compressed data, was "gmalglib-0.1.4.tar", last modified: Mon Apr  1 13:26:25 2024, max compression
```

## Comparing `gmalglib-0.1.3.tar` & `gmalglib-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:11:00.445806 gmalglib-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-01 13:10:54.000000 gmalglib-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-01 13:11:00.445806 gmalglib-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-01 13:10:54.000000 gmalglib-0.1.3/README.en.md
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-01 13:10:54.000000 gmalglib-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-01 13:10:54.000000 gmalglib-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:11:00.445806 gmalglib-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-01 13:10:54.000000 gmalglib-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:11:00.441805 gmalglib-0.1.3/sm3/
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-01 13:10:54.000000 gmalglib-0.1.3/sm3/sm3.c
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-01 13:10:54.000000 gmalglib-0.1.3/sm3/sm3.h
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-01 13:10:54.000000 gmalglib-0.1.3/sm3/sm3module.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:11:00.441805 gmalglib-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:11:00.441805 gmalglib-0.1.3/src/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-01 13:10:54.000000 gmalglib-0.1.3/src/gmalglib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-01 13:10:54.000000 gmalglib-0.1.3/src/gmalglib/sm3.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:11:00.445806 gmalglib-0.1.3/src/gmalglib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-01 13:11:00.000000 gmalglib-0.1.3/src/gmalglib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-01 13:11:00.000000 gmalglib-0.1.3/src/gmalglib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:11:00.000000 gmalglib-0.1.3/src/gmalglib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 13:11:00.000000 gmalglib-0.1.3/src/gmalglib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:26:25.169298 gmalglib-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-01 13:26:16.000000 gmalglib-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-01 13:26:25.169298 gmalglib-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-01 13:26:16.000000 gmalglib-0.1.4/README.en.md
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-01 13:26:16.000000 gmalglib-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-01 13:26:16.000000 gmalglib-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:26:25.169298 gmalglib-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-01 13:26:16.000000 gmalglib-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:26:25.165298 gmalglib-0.1.4/sm3/
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-01 13:26:16.000000 gmalglib-0.1.4/sm3/sm3.c
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-01 13:26:16.000000 gmalglib-0.1.4/sm3/sm3.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-01 13:26:16.000000 gmalglib-0.1.4/sm3/sm3module.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:26:25.165298 gmalglib-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:26:25.165298 gmalglib-0.1.4/src/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-01 13:26:16.000000 gmalglib-0.1.4/src/gmalglib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-01 13:26:16.000000 gmalglib-0.1.4/src/gmalglib/sm3.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:26:25.165298 gmalglib-0.1.4/src/gmalglib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-01 13:26:25.000000 gmalglib-0.1.4/src/gmalglib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-01 13:26:25.000000 gmalglib-0.1.4/src/gmalglib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:26:25.000000 gmalglib-0.1.4/src/gmalglib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 13:26:25.000000 gmalglib-0.1.4/src/gmalglib.egg-info/top_level.txt
```

### Comparing `gmalglib-0.1.3/LICENSE` & `gmalglib-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gmalglib-0.1.3/PKG-INFO` & `gmalglib-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.1.3
+Version: 0.1.4
 Summary: GM algorithms C extension for python.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gmalglib-0.1.3/pyproject.toml` & `gmalglib-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmalglib-0.1.3/sm3/sm3.c` & `gmalglib-0.1.4/sm3/sm3.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.1.3/sm3/sm3.h` & `gmalglib-0.1.4/sm3/sm3.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.1.3/sm3/sm3module.c` & `gmalglib-0.1.4/sm3/sm3module.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.1.3/src/gmalglib/sm3.pyi` & `gmalglib-0.1.4/src/gmalglib/sm3.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.1.3/src/gmalglib.egg-info/PKG-INFO` & `gmalglib-0.1.4/src/gmalglib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.1.3
+Version: 0.1.4
 Summary: GM algorithms C extension for python.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

