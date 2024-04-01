# Comparing `tmp/streamdal-0.1.8.tar.gz` & `tmp/streamdal-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamdal-0.1.8.tar", last modified: Fri Feb 16 15:49:15 2024, max compression
+gzip compressed data, was "streamdal-0.1.9.tar", last modified: Mon Feb 26 14:49:35 2024, max compression
```

## Comparing `streamdal-0.1.8.tar` & `streamdal-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 15:49:15.126340 streamdal-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11306 2024-02-16 15:49:10.000000 streamdal-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-02-16 15:49:15.126340 streamdal-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-02-16 15:49:10.000000 streamdal-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 15:49:15.126340 streamdal-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-02-16 15:49:11.000000 streamdal-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 15:49:15.122340 streamdal-0.1.8/streamdal/
--rw-r--r--   0 runner    (1001) docker     (127)    38231 2024-02-16 15:49:11.000000 streamdal-0.1.8/streamdal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 15:49:15.126340 streamdal-0.1.8/streamdal/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-02-16 15:49:10.000000 streamdal-0.1.8/streamdal/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 15:49:15.126340 streamdal-0.1.8/streamdal/hostfunc/
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-02-16 15:49:10.000000 streamdal-0.1.8/streamdal/hostfunc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 15:49:15.126340 streamdal-0.1.8/streamdal/kv/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-02-16 15:49:10.000000 streamdal-0.1.8/streamdal/kv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 15:49:15.126340 streamdal-0.1.8/streamdal/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-02-16 15:49:10.000000 streamdal-0.1.8/streamdal/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 15:49:15.126340 streamdal-0.1.8/streamdal/tail/
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-02-16 15:49:10.000000 streamdal-0.1.8/streamdal/tail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 15:49:15.126340 streamdal-0.1.8/streamdal/validation/
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-02-16 15:49:10.000000 streamdal-0.1.8/streamdal/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 15:49:15.126340 streamdal-0.1.8/streamdal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-02-16 15:49:15.000000 streamdal-0.1.8/streamdal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-16 15:49:15.000000 streamdal-0.1.8/streamdal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 15:49:15.000000 streamdal-0.1.8/streamdal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-02-16 15:49:15.000000 streamdal-0.1.8/streamdal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-16 15:49:15.000000 streamdal-0.1.8/streamdal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:49:35.002845 streamdal-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11306 2024-02-26 14:49:27.000000 streamdal-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-02-26 14:49:35.002845 streamdal-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-02-26 14:49:27.000000 streamdal-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 14:49:35.002845 streamdal-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-02-26 14:49:28.000000 streamdal-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:49:34.998845 streamdal-0.1.9/streamdal/
+-rw-r--r--   0 runner    (1001) docker     (127)    38231 2024-02-26 14:49:28.000000 streamdal-0.1.9/streamdal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:49:35.002845 streamdal-0.1.9/streamdal/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-02-26 14:49:27.000000 streamdal-0.1.9/streamdal/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:49:35.002845 streamdal-0.1.9/streamdal/hostfunc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-02-26 14:49:27.000000 streamdal-0.1.9/streamdal/hostfunc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:49:35.002845 streamdal-0.1.9/streamdal/kv/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-02-26 14:49:27.000000 streamdal-0.1.9/streamdal/kv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:49:35.002845 streamdal-0.1.9/streamdal/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-02-26 14:49:27.000000 streamdal-0.1.9/streamdal/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:49:35.002845 streamdal-0.1.9/streamdal/tail/
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-02-26 14:49:27.000000 streamdal-0.1.9/streamdal/tail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:49:35.002845 streamdal-0.1.9/streamdal/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-02-26 14:49:27.000000 streamdal-0.1.9/streamdal/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:49:35.002845 streamdal-0.1.9/streamdal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-02-26 14:49:34.000000 streamdal-0.1.9/streamdal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-26 14:49:34.000000 streamdal-0.1.9/streamdal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 14:49:34.000000 streamdal-0.1.9/streamdal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-02-26 14:49:34.000000 streamdal-0.1.9/streamdal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-26 14:49:34.000000 streamdal-0.1.9/streamdal.egg-info/top_level.txt
```

### Comparing `streamdal-0.1.8/LICENSE` & `streamdal-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `streamdal-0.1.8/PKG-INFO` & `streamdal-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdal
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python client SDK for Streamdal's open source observability server
 Home-page: https://github.com/streamdal/python-sdk
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `streamdal-0.1.8/README.md` & `streamdal-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `streamdal-0.1.8/setup.py` & `streamdal-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
     name="streamdal",
-    version='0.1.8',
+    version='0.1.9',
     description="Python client SDK for Streamdal's open source observability server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/streamdal/python-sdk",
     author="Streamdal.com",
     author_email="engineering@streamdal.com",
     license="MIT",
@@ -66,15 +66,15 @@
         "python-dateutil==2.8.2",
         "readme-renderer==42.0",
         "requests==2.31.0",
         "requests-toolbelt==1.0.0",
         "rfc3986==2.0.0",
         "rich==13.7.0",
         "six==1.16.0",
-        "streamdal-protos==0.1.21",
+        "streamdal-protos==0.1.27",
         "stringcase==1.2.0",
         "tf==1.0.0",
         "token-bucket==0.3.0",
         "twine==4.0.2",
         "urllib3==2.1.0",
         "wasmer==1.1.0",
         "wasmer-compiler-cranelift==1.1.0",
```

### Comparing `streamdal-0.1.8/streamdal/__init__.py` & `streamdal-0.1.9/streamdal/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -590,15 +590,15 @@
         self.grpc_channel.close()
         self.log.debug("Heartbeat thread exiting")
 
     def _gen_client_info(self) -> protos.ClientInfo:
         return protos.ClientInfo(
             client_type=protos.ClientType(self.cfg.client_type),
             library_name="python-sdk",
-            library_version="0.1.8",
+            library_version="0.1.9",
             language="python",
             arch=platform.processor(),
             os=platform.system(),
         )
 
     def _gen_register_request(self) -> protos.RegisterRequest:
         req = protos.RegisterRequest(
```

### Comparing `streamdal-0.1.8/streamdal/common/__init__.py` & `streamdal-0.1.9/streamdal/common/__init__.py`

 * *Files identical despite different names*

### Comparing `streamdal-0.1.8/streamdal/hostfunc/__init__.py` & `streamdal-0.1.9/streamdal/hostfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `streamdal-0.1.8/streamdal/kv/__init__.py` & `streamdal-0.1.9/streamdal/kv/__init__.py`

 * *Files identical despite different names*

### Comparing `streamdal-0.1.8/streamdal/metrics/__init__.py` & `streamdal-0.1.9/streamdal/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `streamdal-0.1.8/streamdal/tail/__init__.py` & `streamdal-0.1.9/streamdal/tail/__init__.py`

 * *Files identical despite different names*

### Comparing `streamdal-0.1.8/streamdal/validation/__init__.py` & `streamdal-0.1.9/streamdal/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `streamdal-0.1.8/streamdal.egg-info/PKG-INFO` & `streamdal-0.1.9/streamdal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdal
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python client SDK for Streamdal's open source observability server
 Home-page: https://github.com/streamdal/python-sdk
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `streamdal-0.1.8/streamdal.egg-info/requires.txt` & `streamdal-0.1.9/streamdal.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 python-dateutil==2.8.2
 readme-renderer==42.0
 requests-toolbelt==1.0.0
 requests==2.31.0
 rfc3986==2.0.0
 rich==13.7.0
 six==1.16.0
-streamdal-protos==0.1.21
+streamdal-protos==0.1.27
 stringcase==1.2.0
 tf==1.0.0
 token-bucket==0.3.0
 twine==4.0.2
 urllib3==2.1.0
 wasmer-compiler-cranelift==1.1.0
 wasmer==1.1.0
```

