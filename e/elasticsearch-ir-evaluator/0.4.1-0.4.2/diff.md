# Comparing `tmp/elasticsearch_ir_evaluator-0.4.1.tar.gz` & `tmp/elasticsearch_ir_evaluator-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elasticsearch_ir_evaluator-0.4.1.tar", last modified: Fri Mar 29 08:58:37 2024, max compression
+gzip compressed data, was "elasticsearch_ir_evaluator-0.4.2.tar", last modified: Mon Apr  1 13:25:54 2024, max compression
```

## Comparing `elasticsearch_ir_evaluator-0.4.1.tar` & `elasticsearch_ir_evaluator-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 hinatades   (501) staff       (20)        0 2024-03-29 08:58:37.019495 elasticsearch_ir_evaluator-0.4.1/
--rw-r--r--   0 hinatades   (501) staff       (20)    11357 2023-12-30 14:43:03.000000 elasticsearch_ir_evaluator-0.4.1/LICENSE
--rw-r--r--   0 hinatades   (501) staff       (20)     6232 2024-03-29 08:58:37.019335 elasticsearch_ir_evaluator-0.4.1/PKG-INFO
--rw-r--r--   0 hinatades   (501) staff       (20)     5814 2024-03-29 04:54:06.000000 elasticsearch_ir_evaluator-0.4.1/README.md
-drwxr-xr-x   0 hinatades   (501) staff       (20)        0 2024-03-29 08:58:37.017603 elasticsearch_ir_evaluator-0.4.1/elasticsearch_ir_evaluator/
--rw-r--r--   0 hinatades   (501) staff       (20)       83 2024-01-01 18:30:57.000000 elasticsearch_ir_evaluator-0.4.1/elasticsearch_ir_evaluator/__init__.py
--rw-r--r--   0 hinatades   (501) staff       (20)    29407 2024-03-29 08:56:15.000000 elasticsearch_ir_evaluator-0.4.1/elasticsearch_ir_evaluator/evaluator.py
--rw-r--r--   0 hinatades   (501) staff       (20)     2429 2024-03-28 17:34:09.000000 elasticsearch_ir_evaluator-0.4.1/elasticsearch_ir_evaluator/types.py
-drwxr-xr-x   0 hinatades   (501) staff       (20)        0 2024-03-29 08:58:37.018533 elasticsearch_ir_evaluator-0.4.1/elasticsearch_ir_evaluator.egg-info/
--rw-r--r--   0 hinatades   (501) staff       (20)     6232 2024-03-29 08:58:36.000000 elasticsearch_ir_evaluator-0.4.1/elasticsearch_ir_evaluator.egg-info/PKG-INFO
--rw-r--r--   0 hinatades   (501) staff       (20)      432 2024-03-29 08:58:36.000000 elasticsearch_ir_evaluator-0.4.1/elasticsearch_ir_evaluator.egg-info/SOURCES.txt
--rw-r--r--   0 hinatades   (501) staff       (20)        1 2024-03-29 08:58:36.000000 elasticsearch_ir_evaluator-0.4.1/elasticsearch_ir_evaluator.egg-info/dependency_links.txt
--rw-r--r--   0 hinatades   (501) staff       (20)       40 2024-03-29 08:58:36.000000 elasticsearch_ir_evaluator-0.4.1/elasticsearch_ir_evaluator.egg-info/requires.txt
--rw-r--r--   0 hinatades   (501) staff       (20)       33 2024-03-29 08:58:36.000000 elasticsearch_ir_evaluator-0.4.1/elasticsearch_ir_evaluator.egg-info/top_level.txt
--rw-r--r--   0 hinatades   (501) staff       (20)       38 2024-03-29 08:58:37.019544 elasticsearch_ir_evaluator-0.4.1/setup.cfg
--rw-r--r--   0 hinatades   (501) staff       (20)      675 2024-03-29 08:51:43.000000 elasticsearch_ir_evaluator-0.4.1/setup.py
-drwxr-xr-x   0 hinatades   (501) staff       (20)        0 2024-03-29 08:58:37.018779 elasticsearch_ir_evaluator-0.4.1/tests/
--rw-r--r--   0 hinatades   (501) staff       (20)        0 2024-01-01 15:00:06.000000 elasticsearch_ir_evaluator-0.4.1/tests/__init__.py
--rw-r--r--   0 hinatades   (501) staff       (20)     2157 2024-03-28 17:34:09.000000 elasticsearch_ir_evaluator-0.4.1/tests/test_evaluator.py
+drwxr-xr-x   0 hinatades   (501) staff       (20)        0 2024-04-01 13:25:54.442769 elasticsearch_ir_evaluator-0.4.2/
+-rw-r--r--   0 hinatades   (501) staff       (20)    11357 2023-12-30 14:43:03.000000 elasticsearch_ir_evaluator-0.4.2/LICENSE
+-rw-r--r--   0 hinatades   (501) staff       (20)     6232 2024-04-01 13:25:54.442612 elasticsearch_ir_evaluator-0.4.2/PKG-INFO
+-rw-r--r--   0 hinatades   (501) staff       (20)     5814 2024-03-29 04:54:06.000000 elasticsearch_ir_evaluator-0.4.2/README.md
+drwxr-xr-x   0 hinatades   (501) staff       (20)        0 2024-04-01 13:25:54.441101 elasticsearch_ir_evaluator-0.4.2/elasticsearch_ir_evaluator/
+-rw-r--r--   0 hinatades   (501) staff       (20)       83 2024-01-01 18:30:57.000000 elasticsearch_ir_evaluator-0.4.2/elasticsearch_ir_evaluator/__init__.py
+-rw-r--r--   0 hinatades   (501) staff       (20)    29481 2024-04-01 13:21:04.000000 elasticsearch_ir_evaluator-0.4.2/elasticsearch_ir_evaluator/evaluator.py
+-rw-r--r--   0 hinatades   (501) staff       (20)     2429 2024-03-28 17:34:09.000000 elasticsearch_ir_evaluator-0.4.2/elasticsearch_ir_evaluator/types.py
+drwxr-xr-x   0 hinatades   (501) staff       (20)        0 2024-04-01 13:25:54.441991 elasticsearch_ir_evaluator-0.4.2/elasticsearch_ir_evaluator.egg-info/
+-rw-r--r--   0 hinatades   (501) staff       (20)     6232 2024-04-01 13:25:54.000000 elasticsearch_ir_evaluator-0.4.2/elasticsearch_ir_evaluator.egg-info/PKG-INFO
+-rw-r--r--   0 hinatades   (501) staff       (20)      432 2024-04-01 13:25:54.000000 elasticsearch_ir_evaluator-0.4.2/elasticsearch_ir_evaluator.egg-info/SOURCES.txt
+-rw-r--r--   0 hinatades   (501) staff       (20)        1 2024-04-01 13:25:54.000000 elasticsearch_ir_evaluator-0.4.2/elasticsearch_ir_evaluator.egg-info/dependency_links.txt
+-rw-r--r--   0 hinatades   (501) staff       (20)       40 2024-04-01 13:25:54.000000 elasticsearch_ir_evaluator-0.4.2/elasticsearch_ir_evaluator.egg-info/requires.txt
+-rw-r--r--   0 hinatades   (501) staff       (20)       33 2024-04-01 13:25:54.000000 elasticsearch_ir_evaluator-0.4.2/elasticsearch_ir_evaluator.egg-info/top_level.txt
+-rw-r--r--   0 hinatades   (501) staff       (20)       38 2024-04-01 13:25:54.442816 elasticsearch_ir_evaluator-0.4.2/setup.cfg
+-rw-r--r--   0 hinatades   (501) staff       (20)      675 2024-04-01 13:21:19.000000 elasticsearch_ir_evaluator-0.4.2/setup.py
+drwxr-xr-x   0 hinatades   (501) staff       (20)        0 2024-04-01 13:25:54.442237 elasticsearch_ir_evaluator-0.4.2/tests/
+-rw-r--r--   0 hinatades   (501) staff       (20)        0 2024-01-01 15:00:06.000000 elasticsearch_ir_evaluator-0.4.2/tests/__init__.py
+-rw-r--r--   0 hinatades   (501) staff       (20)     2157 2024-03-28 17:34:09.000000 elasticsearch_ir_evaluator-0.4.2/tests/test_evaluator.py
```

### Comparing `elasticsearch_ir_evaluator-0.4.1/LICENSE` & `elasticsearch_ir_evaluator-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `elasticsearch_ir_evaluator-0.4.1/PKG-INFO` & `elasticsearch_ir_evaluator-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticsearch_ir_evaluator
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Python package for easily calculating information retrieval (IR) accuracy metrics using Elasticsearch and datasets.
 Home-page: https://github.com/hinatades/elasticsearch-ir-evaluator
 Author: Taisuke Hinata
 Author-email: hnttisk@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `elasticsearch_ir_evaluator-0.4.1/README.md` & `elasticsearch_ir_evaluator-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `elasticsearch_ir_evaluator-0.4.1/elasticsearch_ir_evaluator/evaluator.py` & `elasticsearch_ir_evaluator-0.4.2/elasticsearch_ir_evaluator/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
             "last_checkpoint_timestamp": datetime.now().isoformat(),
         }
         with open(self.log_file_path, "w") as log_file:
             json.dump(log_data, log_file, indent=2)
 
     def load_progress_log(self):
         if os.path.exists(self.log_file_path):
+            self.logger.info(f"Detected log files: {self.log_file_path}")
             with open(self.log_file_path, "r") as log_file:
                 log_data = json.load(log_file)
                 self.last_processed_id = log_data.get("last_processed_id")
                 self.index_name = log_data.get("index_name")
                 self.processed_count = log_data.get("processed_count")
```

### Comparing `elasticsearch_ir_evaluator-0.4.1/elasticsearch_ir_evaluator/types.py` & `elasticsearch_ir_evaluator-0.4.2/elasticsearch_ir_evaluator/types.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_ir_evaluator-0.4.1/elasticsearch_ir_evaluator.egg-info/PKG-INFO` & `elasticsearch_ir_evaluator-0.4.2/elasticsearch_ir_evaluator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticsearch-ir-evaluator
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Python package for easily calculating information retrieval (IR) accuracy metrics using Elasticsearch and datasets.
 Home-page: https://github.com/hinatades/elasticsearch-ir-evaluator
 Author: Taisuke Hinata
 Author-email: hnttisk@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `elasticsearch_ir_evaluator-0.4.1/setup.py` & `elasticsearch_ir_evaluator-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="elasticsearch_ir_evaluator",
-    version="0.4.1",
+    version="0.4.2",
     description="A Python package for easily calculating information retrieval (IR) accuracy metrics using Elasticsearch and datasets.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     python_requires=">=3.8",
     url="https://github.com/hinatades/elasticsearch-ir-evaluator",
     author="Taisuke Hinata",
     author_email="hnttisk@gmail.com",
```

### Comparing `elasticsearch_ir_evaluator-0.4.1/tests/test_evaluator.py` & `elasticsearch_ir_evaluator-0.4.2/tests/test_evaluator.py`

 * *Files identical despite different names*

