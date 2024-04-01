# Comparing `tmp/qibo_client-0.0.3.tar.gz` & `tmp/qibo_client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibo_client-0.0.3.tar", max compression
+gzip compressed data, was "qibo_client-0.0.4.tar", max compression
```

## Comparing `qibo_client-0.0.3.tar` & `qibo_client-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-02-29 09:51:49.940630 qibo_client-0.0.3/LICENSE
--rw-r--r--   0        0        0     1280 2024-02-29 09:51:49.940630 qibo_client-0.0.3/README.md
--rw-r--r--   0        0        0     1357 2024-02-29 09:51:49.940630 qibo_client-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      132 2024-02-29 09:51:49.940630 qibo_client-0.0.3/src/qibo_client/__init__.py
--rw-r--r--   0        0        0      750 2024-02-29 09:51:49.940630 qibo_client-0.0.3/src/qibo_client/config.py
--rw-r--r--   0        0        0      257 2024-02-29 09:51:49.940630 qibo_client-0.0.3/src/qibo_client/config_logging.py
--rw-r--r--   0        0        0      245 2024-02-29 09:51:49.940630 qibo_client-0.0.3/src/qibo_client/constants.py
--rw-r--r--   0        0        0     8085 2024-02-29 09:51:49.940630 qibo_client-0.0.3/src/qibo_client/qibo_client.py
--rw-r--r--   0        0        0      520 2024-02-29 09:51:49.940630 qibo_client-0.0.3/src/qibo_client/tii.py
--rw-r--r--   0        0        0     2037 1970-01-01 00:00:00.000000 qibo_client-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-01 10:19:46.253145 qibo_client-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1280 2024-04-01 10:19:46.253145 qibo_client-0.0.4/README.md
+-rw-r--r--   0        0        0     1357 2024-04-01 10:19:46.253145 qibo_client-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      132 2024-04-01 10:19:46.253145 qibo_client-0.0.4/src/qibo_client/__init__.py
+-rw-r--r--   0        0        0      750 2024-04-01 10:19:46.253145 qibo_client-0.0.4/src/qibo_client/config.py
+-rw-r--r--   0        0        0      257 2024-04-01 10:19:46.253145 qibo_client-0.0.4/src/qibo_client/config_logging.py
+-rw-r--r--   0        0        0      245 2024-04-01 10:19:46.253145 qibo_client-0.0.4/src/qibo_client/constants.py
+-rw-r--r--   0        0        0     8085 2024-04-01 10:19:46.253145 qibo_client-0.0.4/src/qibo_client/qibo_client.py
+-rw-r--r--   0        0        0      366 2024-04-01 10:19:46.253145 qibo_client-0.0.4/src/qibo_client/tii.py
+-rw-r--r--   0        0        0     2037 1970-01-01 00:00:00.000000 qibo_client-0.0.4/PKG-INFO
```

### Comparing `qibo_client-0.0.3/LICENSE` & `qibo_client-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qibo_client-0.0.3/README.md` & `qibo_client-0.0.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ## Quick start
 
 Once installed, the provider allows to run quantum circuit computations on the
 TiiQ remote server.
 
 :warning: Note: to run jobs on the remote cluster it is mandatory to own a
 validated account.
-Please, sign up to [this link](https://www.qrccluster.com) to
+Please, sign up to [this link](https://cloud.qibo.science) to
 obtain the needed token to run computations on the cluster.
 
 The following snippet provides a basic usage example.
 Replace the `your-tii-qrc-token` string with your user token received during the
 registration process.
 
 ```python
```

### Comparing `qibo_client-0.0.3/pyproject.toml` & `qibo_client-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qibo-client"
-version = "0.0.3"
+version = "0.0.4"
 description = "Qibo client interface."
 authors = ["The Qibo team"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://qibo.science/"
 repository = "https://github.com/qiboteam/qibo-client/"
 documentation = "https://qibo.science/qibo-client/stable"
```

### Comparing `qibo_client-0.0.3/src/qibo_client/config.py` & `qibo_client-0.0.4/src/qibo_client/config.py`

 * *Files identical despite different names*

### Comparing `qibo_client-0.0.3/src/qibo_client/qibo_client.py` & `qibo_client-0.0.4/src/qibo_client/qibo_client.py`

 * *Files identical despite different names*

### Comparing `qibo_client-0.0.3/PKG-INFO` & `qibo_client-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qibo-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: Qibo client interface.
 Home-page: https://qibo.science/
 License: Apache-2.0
 Author: The Qibo team
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -44,15 +44,15 @@
 ## Quick start
 
 Once installed, the provider allows to run quantum circuit computations on the
 TiiQ remote server.
 
 :warning: Note: to run jobs on the remote cluster it is mandatory to own a
 validated account.
-Please, sign up to [this link](https://www.qrccluster.com) to
+Please, sign up to [this link](https://cloud.qibo.science) to
 obtain the needed token to run computations on the cluster.
 
 The following snippet provides a basic usage example.
 Replace the `your-tii-qrc-token` string with your user token received during the
 registration process.
 
 ```python
```

