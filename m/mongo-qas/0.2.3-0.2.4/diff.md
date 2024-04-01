# Comparing `tmp/mongo-qas-0.2.3.tar.gz` & `tmp/mongo-qas-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo-qas-0.2.3.tar", last modified: Thu Dec  7 17:36:25 2023, max compression
+gzip compressed data, was "mongo-qas-0.2.4.tar", last modified: Mon Apr  1 15:58:01 2024, max compression
```

## Comparing `mongo-qas-0.2.3.tar` & `mongo-qas-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-12-07 17:36:25.685177 mongo-qas-0.2.3/
--rwxr-xr-x   0 giles     (1000) giles     (1000)      531 2023-12-07 17:36:25.684738 mongo-qas-0.2.3/PKG-INFO
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-12-07 17:36:25.683424 mongo-qas-0.2.3/mongo_qas.egg-info/
--rwxr-xr-x   0 giles     (1000) giles     (1000)      531 2023-12-07 17:36:25.000000 mongo-qas-0.2.3/mongo_qas.egg-info/PKG-INFO
--rwxr-xr-x   0 giles     (1000) giles     (1000)      324 2023-12-07 17:36:25.000000 mongo-qas-0.2.3/mongo_qas.egg-info/SOURCES.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)        1 2023-12-07 17:36:25.000000 mongo-qas-0.2.3/mongo_qas.egg-info/dependency_links.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       42 2023-12-07 17:36:25.000000 mongo-qas-0.2.3/mongo_qas.egg-info/entry_points.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       31 2023-12-07 17:36:25.000000 mongo-qas-0.2.3/mongo_qas.egg-info/requires.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)        5 2023-12-07 17:36:25.000000 mongo-qas-0.2.3/mongo_qas.egg-info/top_level.txt
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-12-07 17:36:25.681416 mongo-qas-0.2.3/mqas/
--rwxr-xr-x   0 giles     (1000) giles     (1000)      134 2021-06-23 22:20:30.000000 mongo-qas-0.2.3/mqas/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     4448 2022-01-08 18:33:59.000000 mongo-qas-0.2.3/mqas/job.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1618 2022-01-08 20:31:37.000000 mongo-qas-0.2.3/mqas/misc.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6093 2023-02-02 22:55:00.000000 mongo-qas-0.2.3/mqas/queue.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     9165 2023-12-07 17:35:40.000000 mongo-qas-0.2.3/mqas/script.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     2972 2023-12-07 17:22:13.000000 mongo-qas-0.2.3/mqas/utils.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     8470 2023-12-07 17:26:46.000000 mongo-qas-0.2.3/mqas/worker.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)       89 2021-06-24 10:46:56.000000 mongo-qas-0.2.3/pyproject.toml
--rwxr-xr-x   0 giles     (1000) giles     (1000)      685 2023-12-07 17:36:25.687145 mongo-qas-0.2.3/setup.cfg
+drwxrwxr-x   0 giles     (1000) giles     (1000)        0 2024-04-01 15:58:01.006196 mongo-qas-0.2.4/
+-rw-r--r--   0 giles     (1000) giles     (1000)      531 2024-04-01 15:58:01.006196 mongo-qas-0.2.4/PKG-INFO
+drwxrwxr-x   0 giles     (1000) giles     (1000)        0 2024-04-01 15:58:01.006196 mongo-qas-0.2.4/mongo_qas.egg-info/
+-rw-r--r--   0 giles     (1000) giles     (1000)      531 2024-04-01 15:58:01.000000 mongo-qas-0.2.4/mongo_qas.egg-info/PKG-INFO
+-rw-rw-r--   0 giles     (1000) giles     (1000)      324 2024-04-01 15:58:01.000000 mongo-qas-0.2.4/mongo_qas.egg-info/SOURCES.txt
+-rw-rw-r--   0 giles     (1000) giles     (1000)        1 2024-04-01 15:58:01.000000 mongo-qas-0.2.4/mongo_qas.egg-info/dependency_links.txt
+-rw-rw-r--   0 giles     (1000) giles     (1000)       42 2024-04-01 15:58:01.000000 mongo-qas-0.2.4/mongo_qas.egg-info/entry_points.txt
+-rw-rw-r--   0 giles     (1000) giles     (1000)       31 2024-04-01 15:58:01.000000 mongo-qas-0.2.4/mongo_qas.egg-info/requires.txt
+-rw-rw-r--   0 giles     (1000) giles     (1000)        5 2024-04-01 15:58:01.000000 mongo-qas-0.2.4/mongo_qas.egg-info/top_level.txt
+drwxrwxr-x   0 giles     (1000) giles     (1000)        0 2024-04-01 15:58:01.006196 mongo-qas-0.2.4/mqas/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      134 2023-12-07 18:12:42.000000 mongo-qas-0.2.4/mqas/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     4448 2023-12-07 18:12:42.000000 mongo-qas-0.2.4/mqas/job.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1618 2023-12-07 18:12:42.000000 mongo-qas-0.2.4/mqas/misc.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6093 2023-12-07 18:12:42.000000 mongo-qas-0.2.4/mqas/queue.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     9165 2023-12-07 18:12:42.000000 mongo-qas-0.2.4/mqas/script.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     2972 2023-12-07 18:12:42.000000 mongo-qas-0.2.4/mqas/utils.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     8597 2024-04-01 15:57:24.000000 mongo-qas-0.2.4/mqas/worker.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       89 2023-12-07 18:12:42.000000 mongo-qas-0.2.4/pyproject.toml
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      685 2024-04-01 15:58:01.006196 mongo-qas-0.2.4/setup.cfg
```

### Comparing `mongo-qas-0.2.3/PKG-INFO` & `mongo-qas-0.2.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo-qas
-Version: 0.2.3
+Version: 0.2.4
 Summary: A job queuing and scheduling library based on mongodb
 Home-page: https://github.com/giesekow/mongo-qas
 Author: Giles Tetteh
 Author-email: giles.tetteh@tum.de
 Keywords: mongo,queue,schedule,rq
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mongo-qas-0.2.3/mongo_qas.egg-info/PKG-INFO` & `mongo-qas-0.2.4/mongo_qas.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo-qas
-Version: 0.2.3
+Version: 0.2.4
 Summary: A job queuing and scheduling library based on mongodb
 Home-page: https://github.com/giesekow/mongo-qas
 Author: Giles Tetteh
 Author-email: giles.tetteh@tum.de
 Keywords: mongo,queue,schedule,rq
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mongo-qas-0.2.3/mqas/job.py` & `mongo-qas-0.2.4/mqas/job.py`

 * *Files identical despite different names*

### Comparing `mongo-qas-0.2.3/mqas/misc.py` & `mongo-qas-0.2.4/mqas/misc.py`

 * *Files identical despite different names*

### Comparing `mongo-qas-0.2.3/mqas/queue.py` & `mongo-qas-0.2.4/mqas/queue.py`

 * *Files identical despite different names*

### Comparing `mongo-qas-0.2.3/mqas/script.py` & `mongo-qas-0.2.4/mqas/script.py`

 * *Files identical despite different names*

### Comparing `mongo-qas-0.2.3/mqas/utils.py` & `mongo-qas-0.2.4/mqas/utils.py`

 * *Files identical despite different names*

### Comparing `mongo-qas-0.2.3/mqas/worker.py` & `mongo-qas-0.2.4/mqas/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,23 +36,27 @@
 
     if executable is None:
       executable = sys.executable
 
     if modulePaths is None:
       modulePaths = []
 
-    with tempfile.NamedTemporaryFile(delete=True, suffix=".json") as tmp_file:
-      data = {"function_name": function_name, "args": args, "kwargs": kwargs, "stdout": stdout, "modules": modulePaths + [os.getcwd(),], "output": tmp_file.name}
+    with tempfile.TemporaryDirectory() as tmp_dir:
+      tmp_file_name = os.path.join(tmp_dir, "job_results.json")
+
+      data = {"function_name": function_name, "args": args, "kwargs": kwargs, "stdout": stdout, "modules": modulePaths + [os.getcwd(),], "output": tmp_file_name}
 
       if self.as_subprocess:
         subprocess.run([executable, "-c", executionCodeSubProcess], input=str.encode(json.dumps(data, default=json_util.default)))
       else:
         exec(executionCodeExec, {"payload": data})
 
-      self.output = json.load(tmp_file)
+      if os.path.exists(tmp_file):
+        with open(tmp_file_name, 'r') as tmp_file:
+          self.output = json.load(tmp_file)
   
   def get_output(self):
     return self.output
 
   def get_job(self):
     return self.job
```

### Comparing `mongo-qas-0.2.3/setup.cfg` & `mongo-qas-0.2.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mongo-qas
-version = 0.2.3
+version = 0.2.4
 author = Giles Tetteh
 author_email = giles.tetteh@tum.de
 description = A job queuing and scheduling library based on mongodb
 url = https://github.com/giesekow/mongo-qas
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

