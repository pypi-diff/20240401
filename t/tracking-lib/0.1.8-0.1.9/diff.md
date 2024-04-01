# Comparing `tmp/tracking_lib-0.1.8.tar.gz` & `tmp/tracking_lib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracking_lib-0.1.8.tar", last modified: Thu Feb 15 11:20:38 2024, max compression
+gzip compressed data, was "tracking_lib-0.1.9.tar", last modified: Thu Feb 15 13:26:43 2024, max compression
```

## Comparing `tracking_lib-0.1.8.tar` & `tracking_lib-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 11:20:38.556977 tracking_lib-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-15 11:20:38.552977 tracking_lib-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-15 11:20:09.000000 tracking_lib-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 11:20:38.556977 tracking_lib-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-02-15 11:20:09.000000 tracking_lib-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 11:20:38.552977 tracking_lib-0.1.8/tracking_lib/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-15 11:20:09.000000 tracking_lib-0.1.8/tracking_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 11:20:38.552977 tracking_lib-0.1.8/tracking_lib/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 11:20:09.000000 tracking_lib-0.1.8/tracking_lib/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-02-15 11:20:09.000000 tracking_lib-0.1.8/tracking_lib/adapters/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-15 11:20:09.000000 tracking_lib-0.1.8/tracking_lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 11:20:38.552977 tracking_lib-0.1.8/tracking_lib/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 11:20:09.000000 tracking_lib-0.1.8/tracking_lib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-02-15 11:20:09.000000 tracking_lib-0.1.8/tracking_lib/models/transaction_status_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-02-15 11:20:09.000000 tracking_lib-0.1.8/tracking_lib/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 11:20:38.552977 tracking_lib-0.1.8/tracking_lib/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 11:20:09.000000 tracking_lib-0.1.8/tracking_lib/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-02-15 11:20:09.000000 tracking_lib-0.1.8/tracking_lib/unit_tests/cloud_function_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-15 11:20:09.000000 tracking_lib-0.1.8/tracking_lib/unit_tests/fastapi_app_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-02-15 11:20:09.000000 tracking_lib-0.1.8/tracking_lib/unit_tests/flask_app_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-02-15 11:20:09.000000 tracking_lib-0.1.8/tracking_lib/unit_tests/transaction_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 11:20:38.552977 tracking_lib-0.1.8/tracking_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-15 11:20:38.000000 tracking_lib-0.1.8/tracking_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-02-15 11:20:38.000000 tracking_lib-0.1.8/tracking_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 11:20:38.000000 tracking_lib-0.1.8/tracking_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-15 11:20:38.000000 tracking_lib-0.1.8/tracking_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-15 11:20:38.000000 tracking_lib-0.1.8/tracking_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:26:43.536543 tracking_lib-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-15 13:26:43.536543 tracking_lib-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-15 13:26:17.000000 tracking_lib-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 13:26:43.536543 tracking_lib-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-02-15 13:26:17.000000 tracking_lib-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:26:43.536543 tracking_lib-0.1.9/tracking_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-15 13:26:17.000000 tracking_lib-0.1.9/tracking_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:26:43.536543 tracking_lib-0.1.9/tracking_lib/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 13:26:17.000000 tracking_lib-0.1.9/tracking_lib/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-15 13:26:17.000000 tracking_lib-0.1.9/tracking_lib/adapters/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-15 13:26:17.000000 tracking_lib-0.1.9/tracking_lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:26:43.536543 tracking_lib-0.1.9/tracking_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 13:26:17.000000 tracking_lib-0.1.9/tracking_lib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-02-15 13:26:17.000000 tracking_lib-0.1.9/tracking_lib/models/transaction_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-02-15 13:26:17.000000 tracking_lib-0.1.9/tracking_lib/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:26:43.536543 tracking_lib-0.1.9/tracking_lib/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 13:26:17.000000 tracking_lib-0.1.9/tracking_lib/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-02-15 13:26:17.000000 tracking_lib-0.1.9/tracking_lib/unit_tests/cloud_function_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-02-15 13:26:17.000000 tracking_lib-0.1.9/tracking_lib/unit_tests/fastapi_app_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-02-15 13:26:17.000000 tracking_lib-0.1.9/tracking_lib/unit_tests/flask_app_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-02-15 13:26:17.000000 tracking_lib-0.1.9/tracking_lib/unit_tests/transaction_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:26:43.536543 tracking_lib-0.1.9/tracking_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-15 13:26:43.000000 tracking_lib-0.1.9/tracking_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-02-15 13:26:43.000000 tracking_lib-0.1.9/tracking_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 13:26:43.000000 tracking_lib-0.1.9/tracking_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-15 13:26:43.000000 tracking_lib-0.1.9/tracking_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-15 13:26:43.000000 tracking_lib-0.1.9/tracking_lib.egg-info/top_level.txt
```

### Comparing `tracking_lib-0.1.8/setup.py` & `tracking_lib-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='tracking_lib',
-    version='0.1.8',
+    version='0.1.9',
     url='https://github.com/thinkdigitalgroupprojectagora/team-moc-tracking-lib',
     author='Damianos Damianidis',
     author_email='damianosd@projectagora.com',
     description='A library for tracking transactions in Flask and FastAPI applications.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `tracking_lib-0.1.8/tracking_lib/adapters/pubsub.py` & `tracking_lib-0.1.9/tracking_lib/adapters/pubsub.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from google.cloud import pubsub_v1
-from config import Config
+from ..config import Config
 
 class PubSubAdapter():
 
     project_id = Config.control_channel_project_id
     topic_id = Config.control_channel_topic_id
```

### Comparing `tracking_lib-0.1.8/tracking_lib/models/transaction_status_update.py` & `tracking_lib-0.1.9/tracking_lib/models/transaction_status_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os, json
 import time
 
 class TransactionStatusUpdate():
 
     def __init__(self, transaction_id, src_event_name):
         self.transaction_id=transaction_id
         self.src_event_name=src_event_name
```

### Comparing `tracking_lib-0.1.8/tracking_lib/transaction.py` & `tracking_lib-0.1.9/tracking_lib/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 from fastapi import FastAPI, Request
 from flask import Flask, g
-from adapters.pubsub import PubSubAdapter
-from models.transaction_status_update import TransactionStatusUpdate
+from .adapters.pubsub import PubSubAdapter
+from .models.transaction_status_update import TransactionStatusUpdate
 
 class Transaction:
 
     @classmethod
     def find_object_of_type(cls, obj_type):
         frame = inspect.currentframe()
         while frame:
```

### Comparing `tracking_lib-0.1.8/tracking_lib/unit_tests/cloud_function_test.py` & `tracking_lib-0.1.9/tracking_lib/unit_tests/cloud_function_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Add the parent directory to PATH
 sys.path.append(parent_dir)
 
 import time
 import requests
 import subprocess
 import pytest
-from transaction import Transaction
+from tracking_lib.transaction import Transaction
 
 def interactor_runc():
     #print(f"transaction_id in interactor func: {Transaction.read_transaction_id()}")
     return Transaction.read_transaction_id()
 
 def hello_world(request):
     request_args = request.args
```

### Comparing `tracking_lib-0.1.8/tracking_lib/unit_tests/fastapi_app_test.py` & `tracking_lib-0.1.9/tracking_lib/unit_tests/fastapi_app_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Add the parent directory to PATH
 sys.path.append(parent_dir)
 
 from fastapi import FastAPI, Request
 from fastapi.testclient import TestClient
 import pytest
-from transaction import Transaction
+from tracking_lib.transaction import Transaction
 
 app = FastAPI()
 
 def interactor_runc():
     #print(f"transaction_id in interactor func: {Transaction.read_transaction_id()}")
     return Transaction.read_transaction_id()
```

### Comparing `tracking_lib-0.1.8/tracking_lib/unit_tests/flask_app_test.py` & `tracking_lib-0.1.9/tracking_lib/unit_tests/flask_app_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 parent_dir = os.path.dirname(current_dir)
 
 # Add the parent directory to PATH
 sys.path.append(parent_dir)
 from unittest.mock import patch, MagicMock
 from flask import Flask, jsonify
 import pytest
-from transaction import Transaction
-from models.transaction_status_update import TransactionStatusUpdate
-from adapters.pubsub import PubSubAdapter
+from tracking_lib.transaction import Transaction
+from tracking_lib.models.transaction_status_update import TransactionStatusUpdate
+from tracking_lib.adapters.pubsub import PubSubAdapter
 
 app = Flask(__name__)
 
 def interactor_runc():
     #print(f"transaction_id in interactor func: {Transaction.read_transaction_id()}")
     return Transaction.read_transaction_id()
```

### Comparing `tracking_lib-0.1.8/tracking_lib/unit_tests/transaction_test.py` & `tracking_lib-0.1.9/tracking_lib/unit_tests/transaction_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 # Get the parent directory
 parent_dir = os.path.dirname(current_dir)
 
 # Add the parent directory to PATH
 sys.path.append(parent_dir)
 
-from transaction import Transaction
-from models.transaction_status_update import TransactionStatusUpdate
-from adapters.pubsub import PubSubAdapter
+from tracking_lib.transaction import Transaction
+from tracking_lib.models.transaction_status_update import TransactionStatusUpdate
+from tracking_lib.adapters.pubsub import PubSubAdapter
 
 # Unit test
 def test_set_transaction_status_success():
     Transaction.read_transaction_id = MagicMock(return_value="123456")
     with patch.object(TransactionStatusUpdate, 'set_status_failure', new=MagicMock()) as mock_method:
         Transaction.set_transaction_status(src_event_name="AN_SRC_EVENT_NAME")
         mock_method.assert_not_called()
```

### Comparing `tracking_lib-0.1.8/tracking_lib.egg-info/SOURCES.txt` & `tracking_lib-0.1.9/tracking_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

