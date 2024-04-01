# Comparing `tmp/reach_commons-0.9.8.tar.gz` & `tmp/reach_commons-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reach_commons-0.9.8.tar", max compression
+gzip compressed data, was "reach_commons-0.9.9.tar", max compression
```

## Comparing `reach_commons-0.9.8.tar` & `reach_commons-0.9.9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0      777 2023-12-21 20:24:45.783379 reach_commons-0.9.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-10 19:38:10.823582 reach_commons-0.9.8/reach_commons/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 11:47:10.842448 reach_commons-0.9.8/reach_commons/clients/__init__.py
--rw-r--r--   0        0        0     1500 2023-11-03 21:04:42.233881 reach_commons-0.9.8/reach_commons/clients/api_client.py
--rw-r--r--   0        0        0     2879 2023-11-02 17:37:09.077861 reach_commons-0.9.8/reach_commons/clients/api_client_v2.py
--rw-r--r--   0        0        0     2535 2023-12-08 21:28:44.600341 reach_commons-0.9.8/reach_commons/clients/http_request_logger.py
--rw-r--r--   0        0        0     5057 2023-12-21 20:24:48.114705 reach_commons-0.9.8/reach_commons/clients/hubspot_client.py
--rw-r--r--   0        0        0     2125 2023-12-21 10:36:18.355330 reach_commons-0.9.8/reach_commons/custom_logger.py
--rw-r--r--   0        0        0        0 2023-10-22 11:55:48.290558 reach_commons-0.9.8/reach_commons/reach_aws/__init__.py
--rw-r--r--   0        0        0      158 2023-10-22 14:35:26.749016 reach_commons-0.9.8/reach_commons/reach_aws/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2023-11-07 20:06:23.009096 reach_commons-0.9.8/reach_commons/reach_aws/dynamo_db/__init__.py
--rw-r--r--   0        0        0      677 2023-12-08 14:34:56.152815 reach_commons-0.9.8/reach_commons/reach_aws/dynamo_db/client.py
--rw-r--r--   0        0        0        0 2023-10-22 11:55:59.136089 reach_commons-0.9.8/reach_commons/reach_aws/kms/__init__.py
--rw-r--r--   0        0        0     4374 2023-12-08 21:18:29.142549 reach_commons-0.9.8/reach_commons/reach_aws/kms/client.py
--rw-r--r--   0        0        0       48 2023-10-24 14:16:19.595924 reach_commons-0.9.8/reach_commons/reach_aws/kms/exceptions.py
--rw-r--r--   0        0        0        0 2023-10-22 11:55:59.136089 reach_commons-0.9.8/reach_commons/reach_aws/sqs/__init__.py
--rw-r--r--   0        0        0      162 2023-10-22 14:35:26.750014 reach_commons-0.9.8/reach_commons/reach_aws/sqs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3016 2023-10-22 20:15:24.286810 reach_commons-0.9.8/reach_commons/reach_aws/sqs/__pycache__/client.cpython-310.pyc
--rw-r--r--   0        0        0      586 2023-10-22 14:35:26.752017 reach_commons-0.9.8/reach_commons/reach_aws/sqs/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0     8683 2023-12-21 20:24:48.141234 reach_commons-0.9.8/reach_commons/reach_aws/sqs/client.py
--rw-r--r--   0        0        0      807 2023-10-31 17:25:49.068913 reach_commons-0.9.8/reach_commons/reach_aws/sqs/exceptions.py
--rw-r--r--   0        0        0     5121 2023-12-21 20:24:38.159988 reach_commons-0.9.8/reach_commons/utils.py
--rw-r--r--   0        0        0      948 2023-10-13 18:52:57.989376 reach_commons-0.9.8/README.md
--rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 reach_commons-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0      795 2023-12-24 17:49:17.514483 reach_commons-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-10-10 19:38:10.823582 reach_commons-0.9.9/reach_commons/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:47:10.842448 reach_commons-0.9.9/reach_commons/clients/__init__.py
+-rw-r--r--   0        0        0     1500 2023-11-03 21:04:42.233881 reach_commons-0.9.9/reach_commons/clients/api_client.py
+-rw-r--r--   0        0        0     2879 2023-11-02 17:37:09.077861 reach_commons-0.9.9/reach_commons/clients/api_client_v2.py
+-rw-r--r--   0        0        0     2535 2023-12-08 21:28:44.600341 reach_commons-0.9.9/reach_commons/clients/http_request_logger.py
+-rw-r--r--   0        0        0     5057 2023-12-24 17:49:22.336120 reach_commons-0.9.9/reach_commons/clients/hubspot_client.py
+-rw-r--r--   0        0        0     2125 2023-12-21 10:36:18.355330 reach_commons-0.9.9/reach_commons/custom_logger.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:55:48.290558 reach_commons-0.9.9/reach_commons/reach_aws/__init__.py
+-rw-r--r--   0        0        0      158 2023-10-22 14:35:26.749016 reach_commons-0.9.9/reach_commons/reach_aws/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2023-11-07 20:06:23.009096 reach_commons-0.9.9/reach_commons/reach_aws/dynamo_db/__init__.py
+-rw-r--r--   0        0        0      677 2023-12-08 14:34:56.152815 reach_commons-0.9.9/reach_commons/reach_aws/dynamo_db/client.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:55:59.136089 reach_commons-0.9.9/reach_commons/reach_aws/kms/__init__.py
+-rw-r--r--   0        0        0     4374 2023-12-08 21:18:29.142549 reach_commons-0.9.9/reach_commons/reach_aws/kms/client.py
+-rw-r--r--   0        0        0       48 2023-10-24 14:16:19.595924 reach_commons-0.9.9/reach_commons/reach_aws/kms/exceptions.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:55:59.136089 reach_commons-0.9.9/reach_commons/reach_aws/sqs/__init__.py
+-rw-r--r--   0        0        0      162 2023-10-22 14:35:26.750014 reach_commons-0.9.9/reach_commons/reach_aws/sqs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3016 2023-10-22 20:15:24.286810 reach_commons-0.9.9/reach_commons/reach_aws/sqs/__pycache__/client.cpython-310.pyc
+-rw-r--r--   0        0        0      586 2023-10-22 14:35:26.752017 reach_commons-0.9.9/reach_commons/reach_aws/sqs/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0     8683 2023-12-24 17:49:22.352981 reach_commons-0.9.9/reach_commons/reach_aws/sqs/client.py
+-rw-r--r--   0        0        0      807 2023-10-31 17:25:49.068913 reach_commons-0.9.9/reach_commons/reach_aws/sqs/exceptions.py
+-rw-r--r--   0        0        0     1896 2023-12-24 17:48:16.048370 reach_commons-0.9.9/reach_commons/redis_manager.py
+-rw-r--r--   0        0        0     5121 2023-12-21 20:24:38.159988 reach_commons-0.9.9/reach_commons/utils.py
+-rw-r--r--   0        0        0      948 2023-10-13 18:52:57.989376 reach_commons-0.9.9/README.md
+-rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 reach_commons-0.9.9/PKG-INFO
```

### Comparing `reach_commons-0.9.8/pyproject.toml` & `reach_commons-0.9.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # isort .; black .; poetry build; poetry publish
 [tool.poetry]
 name = "reach_commons"
-version = "0.9.8"
+version = "0.9.9"
 description = "Uma descrição curta da biblioteca"
 authors = ["Wilson Moraes <wmoraes@getreach.ai>"]
 license = "MIT"
 readme = "README.md"
 
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -24,11 +24,12 @@
 
 [tool.poetry.dev-dependencies]
 black = "23.10.0"
 isort = "5.12.0"
 requests = "2.31.0"
 boto3 = "1.28.68"
 botocore = "^1.31.68"
+redis = "^4.1.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `reach_commons-0.9.8/reach_commons/clients/api_client.py` & `reach_commons-0.9.9/reach_commons/clients/api_client.py`

 * *Files identical despite different names*

### Comparing `reach_commons-0.9.8/reach_commons/clients/api_client_v2.py` & `reach_commons-0.9.9/reach_commons/clients/api_client_v2.py`

 * *Files identical despite different names*

### Comparing `reach_commons-0.9.8/reach_commons/clients/http_request_logger.py` & `reach_commons-0.9.9/reach_commons/clients/http_request_logger.py`

 * *Files identical despite different names*

### Comparing `reach_commons-0.9.8/reach_commons/clients/hubspot_client.py` & `reach_commons-0.9.9/reach_commons/clients/hubspot_client.py`

 * *Files identical despite different names*

### Comparing `reach_commons-0.9.8/reach_commons/custom_logger.py` & `reach_commons-0.9.9/reach_commons/custom_logger.py`

 * *Files identical despite different names*

### Comparing `reach_commons-0.9.8/reach_commons/reach_aws/dynamo_db/client.py` & `reach_commons-0.9.9/reach_commons/reach_aws/dynamo_db/client.py`

 * *Files identical despite different names*

### Comparing `reach_commons-0.9.8/reach_commons/reach_aws/kms/client.py` & `reach_commons-0.9.9/reach_commons/reach_aws/kms/client.py`

 * *Files identical despite different names*

### Comparing `reach_commons-0.9.8/reach_commons/reach_aws/sqs/__pycache__/client.cpython-310.pyc` & `reach_commons-0.9.9/reach_commons/reach_aws/sqs/__pycache__/client.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `reach_commons-0.9.8/reach_commons/reach_aws/sqs/__pycache__/exceptions.cpython-310.pyc` & `reach_commons-0.9.9/reach_commons/reach_aws/sqs/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `reach_commons-0.9.8/reach_commons/reach_aws/sqs/client.py` & `reach_commons-0.9.9/reach_commons/reach_aws/sqs/client.py`

 * *Files identical despite different names*

### Comparing `reach_commons-0.9.8/reach_commons/reach_aws/sqs/exceptions.py` & `reach_commons-0.9.9/reach_commons/reach_aws/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `reach_commons-0.9.8/reach_commons/utils.py` & `reach_commons-0.9.9/reach_commons/utils.py`

 * *Files identical despite different names*

### Comparing `reach_commons-0.9.8/README.md` & `reach_commons-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `reach_commons-0.9.8/PKG-INFO` & `reach_commons-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reach_commons
-Version: 0.9.8
+Version: 0.9.9
 Summary: Uma descrição curta da biblioteca
 License: MIT
 Author: Wilson Moraes
 Author-email: wmoraes@getreach.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

