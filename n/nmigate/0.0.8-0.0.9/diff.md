# Comparing `tmp/nmigate-0.0.8.tar.gz` & `tmp/nmigate-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmigate-0.0.8.tar", last modified: Wed Nov 29 18:27:41 2023, max compression
+gzip compressed data, was "nmigate-0.0.9.tar", last modified: Thu Nov 30 07:46:31 2023, max compression
```

## Comparing `nmigate-0.0.8.tar` & `nmigate-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2023-11-29 18:27:41.700832 nmigate-0.0.8/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1073 2023-11-17 18:23:09.000000 nmigate-0.0.8/LICENSE
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     6337 2023-11-29 18:27:41.700605 nmigate-0.0.8/PKG-INFO
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     5963 2023-11-27 17:41:11.000000 nmigate-0.0.8/README.md
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      495 2023-11-29 18:27:35.000000 nmigate-0.0.8/pyproject.toml
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       38 2023-11-29 18:27:41.700876 nmigate-0.0.8/setup.cfg
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2023-11-29 18:27:41.697272 nmigate-0.0.8/src/
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2023-11-29 18:27:41.698020 nmigate-0.0.8/src/nmigate/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2023-11-23 23:38:01.000000 nmigate-0.0.8/src/nmigate/__init__.py
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2023-11-29 18:27:41.699454 nmigate-0.0.8/src/nmigate/lib/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     2582 2023-11-17 18:23:39.000000 nmigate-0.0.8/src/nmigate/lib/billing.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1648 2023-11-23 23:02:04.000000 nmigate-0.0.8/src/nmigate/lib/customer_vault.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      110 2023-11-16 22:38:58.000000 nmigate-0.0.8/src/nmigate/lib/nmi.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     3411 2023-11-17 18:23:36.000000 nmigate-0.0.8/src/nmigate/lib/plans.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     4962 2023-11-29 18:25:49.000000 nmigate-0.0.8/src/nmigate/lib/subscriptions.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1838 2023-11-28 19:56:13.000000 nmigate-0.0.8/src/nmigate/lib/transactions.py
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2023-11-29 18:27:41.699586 nmigate-0.0.8/src/nmigate/util/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     2444 2023-11-29 18:26:20.000000 nmigate-0.0.8/src/nmigate/util/wrappers.py
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2023-11-29 18:27:41.700318 nmigate-0.0.8/src/nmigate.egg-info/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     6337 2023-11-29 18:27:41.000000 nmigate-0.0.8/src/nmigate.egg-info/PKG-INFO
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      499 2023-11-29 18:27:41.000000 nmigate-0.0.8/src/nmigate.egg-info/SOURCES.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        1 2023-11-29 18:27:41.000000 nmigate-0.0.8/src/nmigate.egg-info/dependency_links.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        8 2023-11-29 18:27:41.000000 nmigate-0.0.8/src/nmigate.egg-info/top_level.txt
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2023-11-29 18:27:41.700142 nmigate-0.0.8/test/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1511 2023-11-17 18:23:36.000000 nmigate-0.0.8/test/test_customer_vault.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     2678 2023-11-17 18:23:36.000000 nmigate-0.0.8/test/test_plans.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     2502 2023-11-29 18:24:43.000000 nmigate-0.0.8/test/test_subscriptions.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1409 2023-11-23 22:59:08.000000 nmigate-0.0.8/test/test_transactions.py
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2023-11-30 07:46:31.531447 nmigate-0.0.9/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1073 2023-11-17 18:23:09.000000 nmigate-0.0.9/LICENSE
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     6337 2023-11-30 07:46:31.531220 nmigate-0.0.9/PKG-INFO
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     5963 2023-11-30 05:59:35.000000 nmigate-0.0.9/README.md
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      495 2023-11-30 07:46:25.000000 nmigate-0.0.9/pyproject.toml
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       38 2023-11-30 07:46:31.531487 nmigate-0.0.9/setup.cfg
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2023-11-30 07:46:31.528130 nmigate-0.0.9/src/
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2023-11-30 07:46:31.528852 nmigate-0.0.9/src/nmigate/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2023-11-23 23:38:01.000000 nmigate-0.0.9/src/nmigate/__init__.py
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2023-11-30 07:46:31.530147 nmigate-0.0.9/src/nmigate/lib/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     2582 2023-11-17 18:23:39.000000 nmigate-0.0.9/src/nmigate/lib/billing.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1995 2023-11-30 07:45:20.000000 nmigate-0.0.9/src/nmigate/lib/customer_vault.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      110 2023-11-16 22:38:58.000000 nmigate-0.0.9/src/nmigate/lib/nmi.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     3411 2023-11-17 18:23:36.000000 nmigate-0.0.9/src/nmigate/lib/plans.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     4962 2023-11-29 18:25:49.000000 nmigate-0.0.9/src/nmigate/lib/subscriptions.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1838 2023-11-28 19:56:13.000000 nmigate-0.0.9/src/nmigate/lib/transactions.py
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2023-11-30 07:46:31.530278 nmigate-0.0.9/src/nmigate/util/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     2444 2023-11-29 18:26:20.000000 nmigate-0.0.9/src/nmigate/util/wrappers.py
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2023-11-30 07:46:31.530956 nmigate-0.0.9/src/nmigate.egg-info/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     6337 2023-11-30 07:46:31.000000 nmigate-0.0.9/src/nmigate.egg-info/PKG-INFO
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      499 2023-11-30 07:46:31.000000 nmigate-0.0.9/src/nmigate.egg-info/SOURCES.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        1 2023-11-30 07:46:31.000000 nmigate-0.0.9/src/nmigate.egg-info/dependency_links.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        8 2023-11-30 07:46:31.000000 nmigate-0.0.9/src/nmigate.egg-info/top_level.txt
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2023-11-30 07:46:31.530781 nmigate-0.0.9/test/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1511 2023-11-17 18:23:36.000000 nmigate-0.0.9/test/test_customer_vault.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     2678 2023-11-17 18:23:36.000000 nmigate-0.0.9/test/test_plans.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     2502 2023-11-29 18:24:43.000000 nmigate-0.0.9/test/test_subscriptions.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1409 2023-11-23 22:59:08.000000 nmigate-0.0.9/test/test_transactions.py
```

### Comparing `nmigate-0.0.8/LICENSE` & `nmigate-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nmigate-0.0.8/PKG-INFO` & `nmigate-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmigate
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Nmi library for python
 Author-email: Gustavo <gustavo.gordillo.giron@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nmigate-0.0.8/README.md` & `nmigate-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nmigate-0.0.8/src/nmigate/lib/billing.py` & `nmigate-0.0.9/src/nmigate/lib/billing.py`

 * *Files identical despite different names*

### Comparing `nmigate-0.0.8/src/nmigate/lib/customer_vault.py` & `nmigate-0.0.9/src/nmigate/lib/customer_vault.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,14 +21,28 @@
         }
         data.update(vault_request['billing_info']) 
         response = requests.post(url="https://secure.nmi.com/api/transact.php", data=data)
         return {"response": response, "type": 'create_customer_vault'}
 
 
     @postProcessXml
+    def validate_customer_vault(self, user_id:str):
+        url = "https://secure.networkmerchants.com/api/transact.php"
+        query = {
+            "security_key": self.security_token,
+            "customer_vault_id": user_id,
+            "amount": "0.00",
+            "type": "validate"
+        }
+        response = requests.post(url=url, data=query)        
+        return response 
+
+
+
+    @postProcessXml
     def get_billing_info_by_transaction_id(self, transaction_id):
         url = "https://secure.nmi.com/api/query.php"
         query = {
             "security_key": self.security_token,
             "transaction_id": transaction_id,
         }
         response = requests.post(url=url, data=query)        
@@ -39,10 +53,9 @@
     def get_customer_info(self, id):
         url = "https://secure.nmi.com/api/query.php"
         query = {
             "report_type": "customer_vault",
             "security_key": self.security_token,
             "customer_vault_id": id
         }
-        # response = asyncio.create_task(self.post(url, query))
         response = requests.post(url=url, data=query)        
         return response
```

### Comparing `nmigate-0.0.8/src/nmigate/lib/plans.py` & `nmigate-0.0.9/src/nmigate/lib/plans.py`

 * *Files identical despite different names*

### Comparing `nmigate-0.0.8/src/nmigate/lib/subscriptions.py` & `nmigate-0.0.9/src/nmigate/lib/subscriptions.py`

 * *Files identical despite different names*

### Comparing `nmigate-0.0.8/src/nmigate/lib/transactions.py` & `nmigate-0.0.9/src/nmigate/lib/transactions.py`

 * *Files identical despite different names*

### Comparing `nmigate-0.0.8/src/nmigate/util/wrappers.py` & `nmigate-0.0.9/src/nmigate/util/wrappers.py`

 * *Files identical despite different names*

### Comparing `nmigate-0.0.8/src/nmigate.egg-info/PKG-INFO` & `nmigate-0.0.9/src/nmigate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmigate
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Nmi library for python
 Author-email: Gustavo <gustavo.gordillo.giron@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nmigate-0.0.8/test/test_customer_vault.py` & `nmigate-0.0.9/test/test_customer_vault.py`

 * *Files identical despite different names*

### Comparing `nmigate-0.0.8/test/test_plans.py` & `nmigate-0.0.9/test/test_plans.py`

 * *Files identical despite different names*

### Comparing `nmigate-0.0.8/test/test_subscriptions.py` & `nmigate-0.0.9/test/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `nmigate-0.0.8/test/test_transactions.py` & `nmigate-0.0.9/test/test_transactions.py`

 * *Files identical despite different names*

