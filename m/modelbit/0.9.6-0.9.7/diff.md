# Comparing `tmp/modelbit-0.9.6.tar.gz` & `tmp/modelbit-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelbit-0.9.6.tar", last modified: Wed Jun  8 21:34:10 2022, max compression
+gzip compressed data, was "modelbit-0.9.7.tar", last modified: Wed Jun  8 23:38:56 2022, max compression
```

## Comparing `modelbit-0.9.6.tar` & `modelbit-0.9.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-08 21:34:10.559111 modelbit-0.9.6/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2022-06-08 21:33:31.000000 modelbit-0.9.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      666 2022-06-08 21:34:10.558111 modelbit-0.9.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-08 21:33:31.000000 modelbit-0.9.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-08 21:34:10.555111 modelbit-0.9.6/modelbit/
--rw-rw-rw-   0 root         (0) root         (0)     6873 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1686 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    15885 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/cloud_kernel_client.py
--rw-rw-rw-   0 root         (0) root         (0)     2376 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)     1574 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/deployments.py
--rw-rw-rw-   0 root         (0) root         (0)     7817 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     4879 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/ipython_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4875 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/ipython_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10182 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/ipython_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     2249 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/ipython_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     5359 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/kernel.py
--rw-rw-rw-   0 root         (0) root         (0)     2806 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/logo-32x32.png
--rw-rw-rw-   0 root         (0) root         (0)     9200 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/logo-64x64.png
--rw-rw-rw-   0 root         (0) root         (0)     7839 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/model.py
--rw-rw-rw-   0 root         (0) root         (0)     6407 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/model_wrappers.py
--rw-rw-rw-   0 root         (0) root         (0)     4393 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/modelbit_core.py
--rw-rw-rw-   0 root         (0) root         (0)    17226 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/runtime.py
--rw-rw-rw-   0 root         (0) root         (0)     3207 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/secure_storage.py
--rw-rw-rw-   0 root         (0) root         (0)      274 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/session.py
--rw-rw-rw-   0 root         (0) root         (0)     3572 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/ux.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2022-06-08 21:33:31.000000 modelbit-0.9.6/modelbit/warehouses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-08 21:34:10.557111 modelbit-0.9.6/modelbit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      666 2022-06-08 21:34:09.000000 modelbit-0.9.6/modelbit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      760 2022-06-08 21:34:10.000000 modelbit-0.9.6/modelbit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-08 21:34:10.000000 modelbit-0.9.6/modelbit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2022-06-08 21:34:10.000000 modelbit-0.9.6/modelbit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-06-08 21:34:10.000000 modelbit-0.9.6/modelbit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-08 21:34:10.558111 modelbit-0.9.6/pyaes/
--rw-rw-rw-   0 root         (0) root         (0)     2136 2022-06-08 21:33:31.000000 modelbit-0.9.6/pyaes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    60325 2022-06-08 21:33:31.000000 modelbit-0.9.6/pyaes/aes.py
--rw-rw-rw-   0 root         (0) root         (0)     8138 2022-06-08 21:33:31.000000 modelbit-0.9.6/pyaes/blockfeeder.py
--rw-rw-rw-   0 root         (0) root         (0)     2065 2022-06-08 21:33:31.000000 modelbit-0.9.6/pyaes/util.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-08 21:34:10.559111 modelbit-0.9.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1121 2022-06-08 21:33:31.000000 modelbit-0.9.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-08 23:38:56.770669 modelbit-0.9.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2022-06-08 23:38:17.000000 modelbit-0.9.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      666 2022-06-08 23:38:56.770669 modelbit-0.9.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-08 23:38:17.000000 modelbit-0.9.7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-08 23:38:56.767669 modelbit-0.9.7/modelbit/
+-rw-rw-rw-   0 root         (0) root         (0)     6873 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15918 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/cloud_kernel_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2376 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)     1574 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/deployments.py
+-rw-rw-rw-   0 root         (0) root         (0)     7817 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4879 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/ipython_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4875 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/ipython_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10182 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/ipython_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2249 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/ipython_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     5359 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/kernel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2806 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/logo-32x32.png
+-rw-rw-rw-   0 root         (0) root         (0)     9200 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/logo-64x64.png
+-rw-rw-rw-   0 root         (0) root         (0)     7839 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     6407 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/model_wrappers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4393 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/modelbit_core.py
+-rw-rw-rw-   0 root         (0) root         (0)    17226 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/runtime.py
+-rw-rw-rw-   0 root         (0) root         (0)     3207 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/secure_storage.py
+-rw-rw-rw-   0 root         (0) root         (0)      274 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     3572 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/ux.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2022-06-08 23:38:17.000000 modelbit-0.9.7/modelbit/warehouses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-08 23:38:56.768669 modelbit-0.9.7/modelbit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      666 2022-06-08 23:38:56.000000 modelbit-0.9.7/modelbit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      760 2022-06-08 23:38:56.000000 modelbit-0.9.7/modelbit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-08 23:38:56.000000 modelbit-0.9.7/modelbit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2022-06-08 23:38:56.000000 modelbit-0.9.7/modelbit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-06-08 23:38:56.000000 modelbit-0.9.7/modelbit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-08 23:38:56.770669 modelbit-0.9.7/pyaes/
+-rw-rw-rw-   0 root         (0) root         (0)     2136 2022-06-08 23:38:17.000000 modelbit-0.9.7/pyaes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    60325 2022-06-08 23:38:17.000000 modelbit-0.9.7/pyaes/aes.py
+-rw-rw-rw-   0 root         (0) root         (0)     8138 2022-06-08 23:38:17.000000 modelbit-0.9.7/pyaes/blockfeeder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2022-06-08 23:38:17.000000 modelbit-0.9.7/pyaes/util.py
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-08 23:38:56.771669 modelbit-0.9.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2022-06-08 23:38:17.000000 modelbit-0.9.7/setup.py
```

### Comparing `modelbit-0.9.6/LICENSE` & `modelbit-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/PKG-INFO` & `modelbit-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelbit
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python package to connect Jupyter notebooks to Modelbit
 Home-page: https://www.modelbit.com
 Author: Modelbit
 Author-email: tom@modelbit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: IPython
```

### Comparing `modelbit-0.9.6/modelbit/__init__.py` & `modelbit-0.9.7/modelbit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.6"
+__version__ = "0.9.7"
 __author__ = 'Modelbit'
 
 import os, sys, zipimport
 from typing import cast, Union, Callable, Any, Dict, List
 
 from . import modelbit_core
 from . import datasets
```

### Comparing `modelbit-0.9.6/modelbit/__main__.py` & `modelbit-0.9.7/modelbit/__main__.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/cloud_kernel_client.py` & `modelbit-0.9.7/modelbit/cloud_kernel_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 icbIAiz9IJToB30/kNXvZsCGKngO3Z5/+ab5OSkDnMnap9zfWWEaug7QkQ0slWGF
 l31eh5lyIV51a9/qWPvR8NCkDnaGdiOq8EIjrDsnUIHu4NWQL0UsE3EJA2inqksf
 qwQn1TahV1l6EzhjM/ryga+vBniKxVePwc4ZZKtvWnwuOPPu9q57ZFGiKg==
 -----END CERTIFICATE-----"""
 
 def caCert():
   cert = bytes(os.environ.get("MODELBIT_CA_CERT", PROD_CA_CERT), 'utf-8')
-  if cert == "":
-      cert = PROD_CA_CERT
+  if len(cert) == 0:
+      cert = bytes(PROD_CA_CERT, 'utf-8')
   return cert
 
 
 class StateInfo(NamedTuple):
   expectedTimeSeconds: Optional[int]
   htmlFormatString: str
 
@@ -287,15 +287,15 @@
     req.inspect.detail_level = detail_level
     return await self._runCmd(req)
 
   async def _checkpoint(self) -> Dict[str, Any]:
     if self.stateDispId is not None:
       self.clearMessage(self.stateDispId)
       self.stateDispId = None
-    self.stateDispId = self.sendHtml("", None)
+    self.stateDispId = self.sendHtml("Starting Checkpoint", None)
     await self.do_shutdown(False, True)
     return {"status":"ok", "execution_count":0 }
 
   async def _runCmd(self, req:NotebookRequest) -> Dict[str, Any]:
     if self.stateDispId is not None:
       self.clearMessage(self.stateDispId)
       self.stateDispId = None
@@ -318,30 +318,30 @@
       self._processMbMessage(resp.msg_type, json.loads(resp.content))
     else:
       logging.info("Got message type '%s' content: %s", resp.msg_type, resp.content)
     return None
 
   def _processMbMessage(self, msgType:str, msgData: Dict[str, Any]) -> None:
     if msgType == "state_change":
-      newState = msgData.get("newState")
+      newState = msgData.get("new_state", msgData.get("newState"))
       if newState:
         self._setState(newState)
     elif msgType == "state_progress":
       self._processStateProgress(msgData)
 
   def _processStateProgress(self, msgData: Dict[str, Any]) -> None:
     if hasattr(StateMap, self.state):
       stateInfo: StateInfo = getattr(StateMap, self.state)
       maxProgress = msgData.get('max_progress', stateInfo.expectedTimeSeconds)
-      currentProgress = maxProgress - msgData['current_progress'] if maxProgress else msgData['current_progress']
-      progressMessage = f": {currentProgress} {msgData['progress_unit']}" if currentProgress >= 5 else "." * (1+(msgData['current_progress'] % 3))
+      currentProgress = maxProgress - msgData['progress'] if maxProgress else msgData['progress']
+      progressMessage = f": {currentProgress} {msgData['progress_unit']}" if currentProgress >= 5 else "." * (1+(msgData['progress'] % 3))
       self.stateDispId = self.sendHtml(stateInfo.htmlFormatString + progressMessage, self.stateDispId)
 
   def _waitForKernelProgress(self, seconds:int) -> None:
-    self._processStateProgress({"current_progress":seconds, "progress_unit":"s"})
+    self._processStateProgress({"progress":seconds, "progress_unit":"s"})
 
 
 class ModelbitApiClient:
   kernelId = ""
   remoteAddress = ""
 
   def __init__(self, setState:Callable[[str], None], sendStatusHtml:Callable[[str], None], progressCb:Callable[[int], None]):
```

### Comparing `modelbit-0.9.6/modelbit/datasets.py` & `modelbit-0.9.7/modelbit/datasets.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/deployments.py` & `modelbit-0.9.7/modelbit/deployments.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/helpers.py` & `modelbit-0.9.7/modelbit/helpers.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/ipython_pb2.py` & `modelbit-0.9.7/modelbit/ipython_pb2.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/ipython_pb2.pyi` & `modelbit-0.9.7/modelbit/ipython_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/ipython_pb2_grpc.py` & `modelbit-0.9.7/modelbit/ipython_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/ipython_pb2_grpc.pyi` & `modelbit-0.9.7/modelbit/ipython_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/kernel.py` & `modelbit-0.9.7/modelbit/kernel.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/logo-32x32.png` & `modelbit-0.9.7/modelbit/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/logo-64x64.png` & `modelbit-0.9.7/modelbit/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/model.py` & `modelbit-0.9.7/modelbit/model.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/model_wrappers.py` & `modelbit-0.9.7/modelbit/model_wrappers.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/modelbit_core.py` & `modelbit-0.9.7/modelbit/modelbit_core.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/runtime.py` & `modelbit-0.9.7/modelbit/runtime.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/secure_storage.py` & `modelbit-0.9.7/modelbit/secure_storage.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/utils.py` & `modelbit-0.9.7/modelbit/utils.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/ux.py` & `modelbit-0.9.7/modelbit/ux.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit/warehouses.py` & `modelbit-0.9.7/modelbit/warehouses.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/modelbit.egg-info/PKG-INFO` & `modelbit-0.9.7/modelbit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelbit
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python package to connect Jupyter notebooks to Modelbit
 Home-page: https://www.modelbit.com
 Author: Modelbit
 Author-email: tom@modelbit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: IPython
```

### Comparing `modelbit-0.9.6/modelbit.egg-info/SOURCES.txt` & `modelbit-0.9.7/modelbit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/pyaes/__init__.py` & `modelbit-0.9.7/pyaes/__init__.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/pyaes/aes.py` & `modelbit-0.9.7/pyaes/aes.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/pyaes/blockfeeder.py` & `modelbit-0.9.7/pyaes/blockfeeder.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/pyaes/util.py` & `modelbit-0.9.7/pyaes/util.py`

 * *Files identical despite different names*

### Comparing `modelbit-0.9.6/setup.py` & `modelbit-0.9.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup  # type: ignore
 
 setup(
     name='modelbit',
-    version='0.9.6',
+    version='0.9.7',
     description='Python package to connect Jupyter notebooks to Modelbit',
     url='https://www.modelbit.com',
     author='Modelbit',
     author_email='tom@modelbit.com',
     license='MIT',
     packages=['modelbit', 'pyaes'],
     setup_requires=['jupyter-client', 'ipython'],
```

