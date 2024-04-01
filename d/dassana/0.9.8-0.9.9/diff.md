# Comparing `tmp/dassana-0.9.8.tar.gz` & `tmp/dassana-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dassana-0.9.8.tar", last modified: Wed Sep 13 13:57:41 2023, max compression
+gzip compressed data, was "dassana-0.9.9.tar", last modified: Thu Sep 14 19:35:23 2023, max compression
```

## Comparing `dassana-0.9.8.tar` & `dassana-0.9.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 13:57:41.747372 dassana-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-09-13 13:57:41.747372 dassana-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-09-13 13:57:26.000000 dassana-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 13:57:41.743372 dassana-0.9.8/dassana/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-09-13 13:57:26.000000 dassana-0.9.8/dassana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18702 2023-09-13 13:57:26.000000 dassana-0.9.8/dassana/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2023-09-13 13:57:26.000000 dassana-0.9.8/dassana/dassana_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 13:57:41.743372 dassana-0.9.8/dassana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-09-13 13:57:41.000000 dassana-0.9.8/dassana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-09-13 13:57:41.000000 dassana-0.9.8/dassana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-13 13:57:41.000000 dassana-0.9.8/dassana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-13 13:57:41.000000 dassana-0.9.8/dassana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-09-13 13:57:41.000000 dassana-0.9.8/dassana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-13 13:57:41.000000 dassana-0.9.8/dassana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-13 13:57:41.747372 dassana-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      518 2023-09-13 13:57:26.000000 dassana-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 19:35:23.186218 dassana-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2023-09-14 19:35:23.186218 dassana-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2023-09-14 19:35:13.000000 dassana-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 19:35:23.186218 dassana-0.9.9/dassana/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-09-14 19:35:13.000000 dassana-0.9.9/dassana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18588 2023-09-14 19:35:13.000000 dassana-0.9.9/dassana/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2023-09-14 19:35:13.000000 dassana-0.9.9/dassana/dassana_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 19:35:23.186218 dassana-0.9.9/dassana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2023-09-14 19:35:23.000000 dassana-0.9.9/dassana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2023-09-14 19:35:23.000000 dassana-0.9.9/dassana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-14 19:35:23.000000 dassana-0.9.9/dassana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-14 19:35:23.000000 dassana-0.9.9/dassana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2023-09-14 19:35:23.000000 dassana-0.9.9/dassana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-14 19:35:23.000000 dassana-0.9.9/dassana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-14 19:35:23.186218 dassana-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2023-09-14 19:35:13.000000 dassana-0.9.9/setup.py
```

### Comparing `dassana-0.9.8/dassana/common.py` & `dassana-0.9.9/dassana/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,16 +262,14 @@
             custom_file = open(file_name, 'a')
             self.custom_file_dict[file_name] = custom_file
         custom_file.flush()
         json.dump(json_object, custom_file)
         custom_file.write('\n')
 
     def upload_to_cloud(self, file_name):
-        if self.client is None and self.is_internal_auth:
-            raise ValueError("Client not initialized.")
 
         if not self.is_internal_auth:
             self.upload_to_signed_url()
         elif self.storage_service == 'gcp':
             self.upload_to_gcp(file_name)
         elif self.storage_service == 'aws':
             self.upload_to_aws(file_name)
```

### Comparing `dassana-0.9.8/dassana/dassana_env.py` & `dassana-0.9.9/dassana/dassana_env.py`

 * *Files identical despite different names*

### Comparing `dassana-0.9.8/setup.py` & `dassana-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="dassana",
-    version="0.9.8",
+    version="0.9.9",
     description="Dassana common data ingestion utilities",
     long_description="Dassana common data ingestion utilities",
     url="https://github.com/dassana-io/dassana-python",
     author="Dassana",
     author_email="support@dassana.io",
     license="MIT",
     packages=["dassana"],
```

