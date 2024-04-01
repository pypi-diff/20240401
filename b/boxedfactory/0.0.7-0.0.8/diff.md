# Comparing `tmp/boxedfactory-0.0.7.tar.gz` & `tmp/boxedfactory-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxedfactory-0.0.7.tar", last modified: Sat Oct 21 14:31:02 2023, max compression
+gzip compressed data, was "boxedfactory-0.0.8.tar", last modified: Sat Oct 21 14:55:27 2023, max compression
```

## Comparing `boxedfactory-0.0.7.tar` & `boxedfactory-0.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:31:02.263048 boxedfactory-0.0.7/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2023-10-21 12:55:50.000000 boxedfactory-0.0.7/LICENSE
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       62 2023-10-21 12:59:33.000000 boxedfactory-0.0.7/MANIFEST.in
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      977 2023-10-21 14:31:02.259048 boxedfactory-0.0.7/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        7 2023-10-21 12:59:33.000000 boxedfactory-0.0.7/README.md
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2023-10-21 12:55:50.000000 boxedfactory-0.0.7/pyproject.toml
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       80 2023-10-21 12:55:50.000000 boxedfactory-0.0.7/requirements.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2023-10-21 14:31:02.263048 boxedfactory-0.0.7/setup.cfg
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1217 2023-10-21 12:59:33.000000 boxedfactory-0.0.7/setup.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:31:02.243048 boxedfactory-0.0.7/src/
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:31:02.243048 boxedfactory-0.0.7/src/boxedfactory/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 12:55:50.000000 boxedfactory-0.0.7/src/boxedfactory/__init__.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:31:02.255047 boxedfactory-0.0.7/src/boxedfactory/core/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 12:55:50.000000 boxedfactory-0.0.7/src/boxedfactory/core/__init__.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:31:02.259048 boxedfactory-0.0.7/src/boxedfactory/core/common/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 12:55:50.000000 boxedfactory-0.0.7/src/boxedfactory/core/common/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1772 2023-10-21 12:55:50.000000 boxedfactory-0.0.7/src/boxedfactory/core/common/configurations.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       54 2023-10-21 12:55:50.000000 boxedfactory-0.0.7/src/boxedfactory/core/common/cryptography.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1392 2023-10-21 14:30:35.000000 boxedfactory-0.0.7/src/boxedfactory/core/common/data.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       92 2023-10-21 12:55:50.000000 boxedfactory-0.0.7/src/boxedfactory/core/common/environment.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      643 2023-10-21 12:55:50.000000 boxedfactory-0.0.7/src/boxedfactory/core/common/http.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1512 2023-10-21 14:30:35.000000 boxedfactory-0.0.7/src/boxedfactory/core/common/queue.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     3007 2023-10-21 14:30:35.000000 boxedfactory-0.0.7/src/boxedfactory/core/common/storage.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      348 2023-10-21 12:55:50.000000 boxedfactory-0.0.7/src/boxedfactory/core/test_worker.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2847 2023-10-21 13:47:15.000000 boxedfactory-0.0.7/src/boxedfactory/core/worker.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1426 2023-10-21 12:55:50.000000 boxedfactory-0.0.7/src/boxedfactory/core/worker_manager.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:31:02.251047 boxedfactory-0.0.7/src/boxedfactory.egg-info/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      977 2023-10-21 14:31:02.000000 boxedfactory-0.0.7/src/boxedfactory.egg-info/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      782 2023-10-21 14:31:02.000000 boxedfactory-0.0.7/src/boxedfactory.egg-info/SOURCES.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2023-10-21 14:31:02.000000 boxedfactory-0.0.7/src/boxedfactory.egg-info/dependency_links.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       81 2023-10-21 14:31:02.000000 boxedfactory-0.0.7/src/boxedfactory.egg-info/requires.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       13 2023-10-21 14:31:02.000000 boxedfactory-0.0.7/src/boxedfactory.egg-info/top_level.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2023-10-21 14:30:35.000000 boxedfactory-0.0.7/version.txt
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:55:27.187866 boxedfactory-0.0.8/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/LICENSE
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       62 2023-10-21 12:59:33.000000 boxedfactory-0.0.8/MANIFEST.in
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      977 2023-10-21 14:55:27.187866 boxedfactory-0.0.8/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        7 2023-10-21 12:59:33.000000 boxedfactory-0.0.8/README.md
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/pyproject.toml
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       80 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/requirements.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2023-10-21 14:55:27.191866 boxedfactory-0.0.8/setup.cfg
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1217 2023-10-21 12:59:33.000000 boxedfactory-0.0.8/setup.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:55:27.179866 boxedfactory-0.0.8/src/
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:55:27.183866 boxedfactory-0.0.8/src/boxedfactory/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/src/boxedfactory/__init__.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:55:27.187866 boxedfactory-0.0.8/src/boxedfactory/core/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/src/boxedfactory/core/__init__.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:55:27.187866 boxedfactory-0.0.8/src/boxedfactory/core/common/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/src/boxedfactory/core/common/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1791 2023-10-21 14:54:58.000000 boxedfactory-0.0.8/src/boxedfactory/core/common/configurations.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       54 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/src/boxedfactory/core/common/cryptography.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1392 2023-10-21 14:30:35.000000 boxedfactory-0.0.8/src/boxedfactory/core/common/data.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       99 2023-10-21 14:54:58.000000 boxedfactory-0.0.8/src/boxedfactory/core/common/environment.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      643 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/src/boxedfactory/core/common/http.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1512 2023-10-21 14:30:35.000000 boxedfactory-0.0.8/src/boxedfactory/core/common/queue.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     3007 2023-10-21 14:30:35.000000 boxedfactory-0.0.8/src/boxedfactory/core/common/storage.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      348 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/src/boxedfactory/core/test_worker.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2847 2023-10-21 13:47:15.000000 boxedfactory-0.0.8/src/boxedfactory/core/worker.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1426 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/src/boxedfactory/core/worker_manager.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:55:27.187866 boxedfactory-0.0.8/src/boxedfactory.egg-info/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      977 2023-10-21 14:55:27.000000 boxedfactory-0.0.8/src/boxedfactory.egg-info/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      782 2023-10-21 14:55:27.000000 boxedfactory-0.0.8/src/boxedfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2023-10-21 14:55:27.000000 boxedfactory-0.0.8/src/boxedfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       81 2023-10-21 14:55:27.000000 boxedfactory-0.0.8/src/boxedfactory.egg-info/requires.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       13 2023-10-21 14:55:27.000000 boxedfactory-0.0.8/src/boxedfactory.egg-info/top_level.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2023-10-21 14:54:58.000000 boxedfactory-0.0.8/version.txt
```

### Comparing `boxedfactory-0.0.7/LICENSE` & `boxedfactory-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `boxedfactory-0.0.7/PKG-INFO` & `boxedfactory-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxedfactory
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library with rabbit, mongo and azure
 Home-page: https://github.com/LostSavannah/boxed-factory
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/boxed-factory/issues
 Project-URL: Documentation, https://dev.moradev.dev/boxed-factory/documentation
 Project-URL: Examples, https://dev.moradev.dev/boxed-factory/examples
```

### Comparing `boxedfactory-0.0.7/setup.py` & `boxedfactory-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `boxedfactory-0.0.7/src/boxedfactory/core/common/configurations.py` & `boxedfactory-0.0.8/src/boxedfactory/core/common/configurations.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,16 +19,16 @@
         self.root = {}
         self.load()
 
     def load(self):
         try:
             with open(self.location, 'r') as fi:
                 self.root = json.load(fi)
-        except:
-            pass
+        except Exception as e:
+            print(e)
 
     def get_value(self, path:str, node:dict[str, str] = None, default_value = None, path_description:str = None) -> Obj:
         path_description = path_description or path
         if node == None:
             if self.behaviour.always_reload:
                 self.load()
             return self.get_value(path, self.root, default_value, path_description)
```

### Comparing `boxedfactory-0.0.7/src/boxedfactory/core/common/data.py` & `boxedfactory-0.0.8/src/boxedfactory/core/common/data.py`

 * *Files identical despite different names*

### Comparing `boxedfactory-0.0.7/src/boxedfactory/core/common/http.py` & `boxedfactory-0.0.8/src/boxedfactory/core/common/http.py`

 * *Files identical despite different names*

### Comparing `boxedfactory-0.0.7/src/boxedfactory/core/common/queue.py` & `boxedfactory-0.0.8/src/boxedfactory/core/common/queue.py`

 * *Files identical despite different names*

### Comparing `boxedfactory-0.0.7/src/boxedfactory/core/common/storage.py` & `boxedfactory-0.0.8/src/boxedfactory/core/common/storage.py`

 * *Files identical despite different names*

### Comparing `boxedfactory-0.0.7/src/boxedfactory/core/worker.py` & `boxedfactory-0.0.8/src/boxedfactory/core/worker.py`

 * *Files identical despite different names*

### Comparing `boxedfactory-0.0.7/src/boxedfactory/core/worker_manager.py` & `boxedfactory-0.0.8/src/boxedfactory/core/worker_manager.py`

 * *Files identical despite different names*

### Comparing `boxedfactory-0.0.7/src/boxedfactory.egg-info/PKG-INFO` & `boxedfactory-0.0.8/src/boxedfactory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxedfactory
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library with rabbit, mongo and azure
 Home-page: https://github.com/LostSavannah/boxed-factory
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/boxed-factory/issues
 Project-URL: Documentation, https://dev.moradev.dev/boxed-factory/documentation
 Project-URL: Examples, https://dev.moradev.dev/boxed-factory/examples
```

### Comparing `boxedfactory-0.0.7/src/boxedfactory.egg-info/SOURCES.txt` & `boxedfactory-0.0.8/src/boxedfactory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

