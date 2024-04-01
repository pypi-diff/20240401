# Comparing `tmp/botasaurus_server-4.0.8.tar.gz` & `tmp/botasaurus_server-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus_server-4.0.8.tar", last modified: Sat Mar 16 15:39:41 2024, max compression
+gzip compressed data, was "botasaurus_server-4.0.9.tar", last modified: Mon Mar 18 07:29:22 2024, max compression
```

## Comparing `botasaurus_server-4.0.8.tar` & `botasaurus_server-4.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-03-16 15:39:41.060999 botasaurus_server-4.0.8/
--rw-rw-rw-   0        0        0     1094 2024-03-09 09:26:05.000000 botasaurus_server-4.0.8/LICENSE
--rw-rw-rw-   0        0        0     1277 2024-03-16 15:39:41.060999 botasaurus_server-4.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       19 2024-03-14 07:59:17.000000 botasaurus_server-4.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-16 15:39:41.021786 botasaurus_server-4.0.8/botasaurus_server/
--rw-rw-rw-   0        0        0       34 2024-03-09 12:33:35.000000 botasaurus_server-4.0.8/botasaurus_server/__init__.py
--rw-rw-rw-   0        0        0      477 2024-03-14 10:24:59.000000 botasaurus_server-4.0.8/botasaurus_server/app.py
--rw-rw-rw-   0        0        0     1617 2024-03-09 12:29:43.000000 botasaurus_server-4.0.8/botasaurus_server/apply_offset_limit.py
--rw-rw-rw-   0        0        0     1249 2024-03-16 15:04:23.000000 botasaurus_server-4.0.8/botasaurus_server/cache_utils.py
--rw-rw-rw-   0        0        0     1051 2024-03-09 12:29:43.000000 botasaurus_server-4.0.8/botasaurus_server/cleaners.py
--rw-rw-rw-   0        0        0      227 2024-03-10 07:15:49.000000 botasaurus_server-4.0.8/botasaurus_server/config.py
--rw-rw-rw-   0        0        0      661 2024-03-10 07:21:57.000000 botasaurus_server-4.0.8/botasaurus_server/controls_adapter.py
--rw-rw-rw-   0        0        0     1465 2024-02-26 09:26:05.000000 botasaurus_server-4.0.8/botasaurus_server/convert_to_english.py
--rw-rw-rw-   0        0        0      666 2024-03-14 10:24:39.000000 botasaurus_server-4.0.8/botasaurus_server/db_setup.py
--rw-rw-rw-   0        0        0     2361 2024-02-26 09:45:11.000000 botasaurus_server-4.0.8/botasaurus_server/download.py
--rw-rw-rw-   0        0        0      767 2024-03-09 11:03:01.000000 botasaurus_server-4.0.8/botasaurus_server/errors.py
--rw-rw-rw-   0        0        0      323 2024-03-14 10:24:59.000000 botasaurus_server-4.0.8/botasaurus_server/executor.py
--rw-rw-rw-   0        0        0    10753 2024-03-14 10:24:59.000000 botasaurus_server-4.0.8/botasaurus_server/filters.py
--rw-rw-rw-   0        0        0     2528 2024-03-14 10:24:59.000000 botasaurus_server-4.0.8/botasaurus_server/k8s.py
--rw-rw-rw-   0        0        0     2262 2024-03-16 11:59:44.000000 botasaurus_server-4.0.8/botasaurus_server/master_executor.py
--rw-rw-rw-   0        0        0      772 2024-03-14 10:24:59.000000 botasaurus_server-4.0.8/botasaurus_server/master_routes.py
--rw-rw-rw-   0        0        0    10744 2024-03-16 15:05:01.000000 botasaurus_server-4.0.8/botasaurus_server/models.py
--rw-rw-rw-   0        0        0     1482 2024-03-16 14:36:37.000000 botasaurus_server-4.0.8/botasaurus_server/run_server.py
--rw-rw-rw-   0        0        0       70 2024-01-17 07:53:15.000000 botasaurus_server-4.0.8/botasaurus_server/scraper_type.py
--rw-rw-rw-   0        0        0    10891 2024-03-16 14:32:15.000000 botasaurus_server-4.0.8/botasaurus_server/server.py
--rw-rw-rw-   0        0        0     7047 2024-03-16 14:10:16.000000 botasaurus_server-4.0.8/botasaurus_server/sorts.py
--rw-rw-rw-   0        0        0     8766 2024-03-16 15:05:01.000000 botasaurus_server-4.0.8/botasaurus_server/task_executor.py
--rw-rw-rw-   0        0        0    29013 2024-03-16 15:05:01.000000 botasaurus_server-4.0.8/botasaurus_server/task_routes.py
--rw-rw-rw-   0        0        0      707 2024-03-14 10:24:59.000000 botasaurus_server-4.0.8/botasaurus_server/ui.py
--rw-rw-rw-   0        0        0    10238 2024-02-26 09:49:12.000000 botasaurus_server-4.0.8/botasaurus_server/views.py
--rw-rw-rw-   0        0        0     2551 2024-03-16 11:59:44.000000 botasaurus_server-4.0.8/botasaurus_server/worker_executor.py
--rw-rw-rw-   0        0        0      315 2024-03-14 10:24:59.000000 botasaurus_server-4.0.8/botasaurus_server/worker_routes.py
-drwxrwxrwx   0        0        0        0 2024-03-16 15:39:41.058865 botasaurus_server-4.0.8/botasaurus_server.egg-info/
--rw-rw-rw-   0        0        0     1277 2024-03-16 15:39:40.000000 botasaurus_server-4.0.8/botasaurus_server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1088 2024-03-16 15:39:40.000000 botasaurus_server-4.0.8/botasaurus_server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-16 15:39:40.000000 botasaurus_server-4.0.8/botasaurus_server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2024-03-16 15:39:40.000000 botasaurus_server-4.0.8/botasaurus_server.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-03-16 15:39:40.000000 botasaurus_server-4.0.8/botasaurus_server.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-03-16 15:39:41.063001 botasaurus_server-4.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1739 2024-03-16 15:39:39.000000 botasaurus_server-4.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-18 07:29:22.503092 botasaurus_server-4.0.9/
+-rw-rw-rw-   0        0        0     1094 2024-03-09 09:26:05.000000 botasaurus_server-4.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1277 2024-03-18 07:29:22.502085 botasaurus_server-4.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2024-03-14 07:59:17.000000 botasaurus_server-4.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-18 07:29:22.466598 botasaurus_server-4.0.9/botasaurus_server/
+-rw-rw-rw-   0        0        0       34 2024-03-09 12:33:35.000000 botasaurus_server-4.0.9/botasaurus_server/__init__.py
+-rw-rw-rw-   0        0        0      477 2024-03-14 10:24:59.000000 botasaurus_server-4.0.9/botasaurus_server/app.py
+-rw-rw-rw-   0        0        0     1617 2024-03-09 12:29:43.000000 botasaurus_server-4.0.9/botasaurus_server/apply_offset_limit.py
+-rw-rw-rw-   0        0        0     1249 2024-03-16 15:04:23.000000 botasaurus_server-4.0.9/botasaurus_server/cache_utils.py
+-rw-rw-rw-   0        0        0     1051 2024-03-09 12:29:43.000000 botasaurus_server-4.0.9/botasaurus_server/cleaners.py
+-rw-rw-rw-   0        0        0      227 2024-03-10 07:15:49.000000 botasaurus_server-4.0.9/botasaurus_server/config.py
+-rw-rw-rw-   0        0        0      661 2024-03-10 07:21:57.000000 botasaurus_server-4.0.9/botasaurus_server/controls_adapter.py
+-rw-rw-rw-   0        0        0     1465 2024-02-26 09:26:05.000000 botasaurus_server-4.0.9/botasaurus_server/convert_to_english.py
+-rw-rw-rw-   0        0        0      666 2024-03-14 10:24:39.000000 botasaurus_server-4.0.9/botasaurus_server/db_setup.py
+-rw-rw-rw-   0        0        0     2361 2024-02-26 09:45:11.000000 botasaurus_server-4.0.9/botasaurus_server/download.py
+-rw-rw-rw-   0        0        0      767 2024-03-09 11:03:01.000000 botasaurus_server-4.0.9/botasaurus_server/errors.py
+-rw-rw-rw-   0        0        0      323 2024-03-14 10:24:59.000000 botasaurus_server-4.0.9/botasaurus_server/executor.py
+-rw-rw-rw-   0        0        0    10753 2024-03-14 10:24:59.000000 botasaurus_server-4.0.9/botasaurus_server/filters.py
+-rw-rw-rw-   0        0        0     2528 2024-03-14 10:24:59.000000 botasaurus_server-4.0.9/botasaurus_server/k8s.py
+-rw-rw-rw-   0        0        0     2262 2024-03-16 11:59:44.000000 botasaurus_server-4.0.9/botasaurus_server/master_executor.py
+-rw-rw-rw-   0        0        0      772 2024-03-14 10:24:59.000000 botasaurus_server-4.0.9/botasaurus_server/master_routes.py
+-rw-rw-rw-   0        0        0    10744 2024-03-16 15:05:01.000000 botasaurus_server-4.0.9/botasaurus_server/models.py
+-rw-rw-rw-   0        0        0     1606 2024-03-18 07:29:04.000000 botasaurus_server-4.0.9/botasaurus_server/run_server.py
+-rw-rw-rw-   0        0        0       70 2024-01-17 07:53:15.000000 botasaurus_server-4.0.9/botasaurus_server/scraper_type.py
+-rw-rw-rw-   0        0        0    10891 2024-03-16 14:32:15.000000 botasaurus_server-4.0.9/botasaurus_server/server.py
+-rw-rw-rw-   0        0        0     7047 2024-03-16 14:10:16.000000 botasaurus_server-4.0.9/botasaurus_server/sorts.py
+-rw-rw-rw-   0        0        0     8766 2024-03-16 15:05:01.000000 botasaurus_server-4.0.9/botasaurus_server/task_executor.py
+-rw-rw-rw-   0        0        0    29013 2024-03-16 15:05:01.000000 botasaurus_server-4.0.9/botasaurus_server/task_routes.py
+-rw-rw-rw-   0        0        0      707 2024-03-14 10:24:59.000000 botasaurus_server-4.0.9/botasaurus_server/ui.py
+-rw-rw-rw-   0        0        0    10245 2024-03-18 06:31:05.000000 botasaurus_server-4.0.9/botasaurus_server/views.py
+-rw-rw-rw-   0        0        0     2551 2024-03-16 11:59:44.000000 botasaurus_server-4.0.9/botasaurus_server/worker_executor.py
+-rw-rw-rw-   0        0        0      315 2024-03-14 10:24:59.000000 botasaurus_server-4.0.9/botasaurus_server/worker_routes.py
+drwxrwxrwx   0        0        0        0 2024-03-18 07:29:22.501079 botasaurus_server-4.0.9/botasaurus_server.egg-info/
+-rw-rw-rw-   0        0        0     1277 2024-03-18 07:29:22.000000 botasaurus_server-4.0.9/botasaurus_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1088 2024-03-18 07:29:22.000000 botasaurus_server-4.0.9/botasaurus_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-18 07:29:22.000000 botasaurus_server-4.0.9/botasaurus_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-03-18 07:29:22.000000 botasaurus_server-4.0.9/botasaurus_server.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-03-18 07:29:22.000000 botasaurus_server-4.0.9/botasaurus_server.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-03-18 07:29:22.505744 botasaurus_server-4.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1739 2024-03-18 07:29:21.000000 botasaurus_server-4.0.9/setup.py
```

### Comparing `botasaurus_server-4.0.8/LICENSE` & `botasaurus_server-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/PKG-INFO` & `botasaurus_server-4.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus_server
-Version: 4.0.8
+Version: 4.0.9
 Summary: Botasaurus Server allows you to transform your scrapers into APIs or scale them using Kubernetes.
 Home-page: https://github.com/omkarcloud/botasaurus
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Keywords: botasaurus,botasaurus_server
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `botasaurus_server-4.0.8/botasaurus_server/apply_offset_limit.py` & `botasaurus_server-4.0.9/botasaurus_server/apply_offset_limit.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/cache_utils.py` & `botasaurus_server-4.0.9/botasaurus_server/cache_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/cleaners.py` & `botasaurus_server-4.0.9/botasaurus_server/cleaners.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/controls_adapter.py` & `botasaurus_server-4.0.9/botasaurus_server/controls_adapter.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/convert_to_english.py` & `botasaurus_server-4.0.9/botasaurus_server/convert_to_english.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/db_setup.py` & `botasaurus_server-4.0.9/botasaurus_server/db_setup.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/download.py` & `botasaurus_server-4.0.9/botasaurus_server/download.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/errors.py` & `botasaurus_server-4.0.9/botasaurus_server/errors.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/filters.py` & `botasaurus_server-4.0.9/botasaurus_server/filters.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/k8s.py` & `botasaurus_server-4.0.9/botasaurus_server/k8s.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/master_executor.py` & `botasaurus_server-4.0.9/botasaurus_server/master_executor.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/master_routes.py` & `botasaurus_server-4.0.9/botasaurus_server/master_routes.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/models.py` & `botasaurus_server-4.0.9/botasaurus_server/models.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/run_server.py` & `botasaurus_server-4.0.9/botasaurus_server/run_server.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 import subprocess
 import os
 from threading import Thread
 import sys
 from .app import run_backend
 
-def run_frontend():
-    # Change to frontend directory
-    frontend_dir = os.path.join(os.getcwd(), "frontend")
-    # Run frontend server
-    subprocess.check_call("npm run start", shell=True, cwd=frontend_dir)
-    # subprocess.check_call("npm run dev", shell=True, cwd=frontend_dir)
 
 def install():
     print("Installing frontend dependencies...")
-    frontend_dir = os.path.join(os.getcwd(), 'frontend')
+    frontend_dir = os.path.join(os.getcwd(), "frontend")
     subprocess.check_call("npm install && npm run build", shell=True, cwd=frontend_dir)
 
+
+def start_frontend():
+    frontend_dir = os.path.join(os.getcwd(), "frontend")
+    subprocess.check_call("npm run start", shell=True, cwd=frontend_dir)
+
+def run_frontend():
+    # Change to frontend directory
+    try:
+        start_frontend()
+    except subprocess.CalledProcessError as e:
+        # Resolve Errors, When user forgets to install frontend
+        install()
+        start_frontend()
+
 def run_server():
     if len(sys.argv) == 1:
         # No arguments provided, run both backend and frontend
         Thread(target=run_backend, daemon=True).start()
         run_frontend()
     elif sys.argv[1] == "backend":
         # Argument "backend" provided, run only backend
@@ -35,9 +43,10 @@
     elif sys.argv[1] == "prod":
         # Argument "prod" provided, run only backend
         run_backend()
     else:
         # Unknown argument provided, raise an exception with the argument
         raise Exception(f"Unknown argument: {sys.argv[1]}")
 
+
 if __name__ == "__main__":
     run_server()
```

### Comparing `botasaurus_server-4.0.8/botasaurus_server/server.py` & `botasaurus_server-4.0.9/botasaurus_server/server.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/sorts.py` & `botasaurus_server-4.0.9/botasaurus_server/sorts.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/task_executor.py` & `botasaurus_server-4.0.9/botasaurus_server/task_executor.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/task_routes.py` & `botasaurus_server-4.0.9/botasaurus_server/task_routes.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/ui.py` & `botasaurus_server-4.0.9/botasaurus_server/ui.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server/views.py` & `botasaurus_server-4.0.9/botasaurus_server/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         }
 
     def _flatten_fields(self, fields):
         flat_list = []
         for field in fields:
             if isinstance(field, (Field, CustomField)):
                 # Wrap field.key in a dict with a 'key' attribute
-                flat_list.append({"key": field.key,})
+                flat_list.append({"key": field.output_key,})
             elif isinstance(field, (ExpandDictField, ExpandListField)):
                 # Only add nested fields without adding the key of the ExpandDictField or ExpandListField itself
                 flat_list.extend(self._flatten_fields(field.fields))
         return flat_list
 
 
 def created_nested_field_values(record, field):
```

### Comparing `botasaurus_server-4.0.8/botasaurus_server/worker_executor.py` & `botasaurus_server-4.0.9/botasaurus_server/worker_executor.py`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/botasaurus_server.egg-info/PKG-INFO` & `botasaurus_server-4.0.9/botasaurus_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus_server
-Version: 4.0.8
+Version: 4.0.9
 Summary: Botasaurus Server allows you to transform your scrapers into APIs or scale them using Kubernetes.
 Home-page: https://github.com/omkarcloud/botasaurus
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Keywords: botasaurus,botasaurus_server
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `botasaurus_server-4.0.8/botasaurus_server.egg-info/SOURCES.txt` & `botasaurus_server-4.0.9/botasaurus_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botasaurus_server-4.0.8/setup.py` & `botasaurus_server-4.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         return long_description
     except:
         return None
 
 
 setup(
     name="botasaurus_server",
-    version='4.0.8',
+    version='4.0.9',
     author="Chetan Jain",
     author_email="chetan@omkar.cloud",
     description="Botasaurus Server allows you to transform your scrapers into APIs or scale them using Kubernetes.",
     license="MIT",
     keywords=["botasaurus", "botasaurus_server"],
     url="https://github.com/omkarcloud/botasaurus",
     packages=["botasaurus_server"],
```

