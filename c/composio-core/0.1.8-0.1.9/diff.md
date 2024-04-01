# Comparing `tmp/composio_core-0.1.8.tar.gz` & `tmp/composio_core-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.8.tar", last modified: Tue Mar 19 19:45:17 2024, max compression
+gzip compressed data, was "composio_core-0.1.9.tar", last modified: Tue Mar 19 19:55:20 2024, max compression
```

## Comparing `composio_core-0.1.8.tar` & `composio_core-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-03-19 19:45:17.205568 composio_core-0.1.8/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.8/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      740 2024-03-19 19:45:17.205361 composio_core-0.1.8/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.8/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-03-19 19:45:17.203359 composio_core-0.1.8/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      161 2024-03-19 19:38:35.000000 composio_core-0.1.8/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)     6030 2024-03-19 15:05:39.000000 composio_core-0.1.8/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-03-19 19:45:17.204298 composio_core-0.1.8/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       70 2024-03-19 19:42:55.000000 composio_core-0.1.8/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     3160 2024-03-19 19:44:08.000000 composio_core-0.1.8/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     3926 2024-03-19 12:33:19.000000 composio_core-0.1.8/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     8725 2024-03-19 19:43:38.000000 composio_core-0.1.8/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     1264 2024-03-16 12:05:30.000000 composio_core-0.1.8/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     1614 2024-03-19 16:11:07.000000 composio_core-0.1.8/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-03-19 19:45:17.205168 composio_core-0.1.8/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      740 2024-03-19 19:45:17.000000 composio_core-0.1.8/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-03-19 19:45:17.000000 composio_core-0.1.8/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-03-19 19:45:17.000000 composio_core-0.1.8/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-03-19 19:45:17.000000 composio_core-0.1.8/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       77 2024-03-19 19:45:17.000000 composio_core-0.1.8/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-03-19 19:45:17.000000 composio_core-0.1.8/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      488 2024-03-19 12:07:26.000000 composio_core-0.1.8/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       75 2024-03-19 10:13:31.000000 composio_core-0.1.8/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-03-19 19:45:17.205613 composio_core-0.1.8/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1157 2024-03-19 19:45:10.000000 composio_core-0.1.8/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-03-19 19:55:20.130721 composio_core-0.1.9/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.9/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)      740 2024-03-19 19:55:20.130501 composio_core-0.1.9/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.9/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-03-19 19:55:20.127779 composio_core-0.1.9/composio/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      161 2024-03-19 19:38:35.000000 composio_core-0.1.9/composio/__init__.py
+-rwxr-xr-x   0 utkarsh    (501) staff       (20)     6030 2024-03-19 15:05:39.000000 composio_core-0.1.9/composio/composio_cli.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-03-19 19:55:20.129181 composio_core-0.1.9/composio/sdk/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       70 2024-03-19 19:42:55.000000 composio_core-0.1.9/composio/sdk/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3160 2024-03-19 19:44:08.000000 composio_core-0.1.9/composio/sdk/core.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3926 2024-03-19 12:33:19.000000 composio_core-0.1.9/composio/sdk/enums.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     8727 2024-03-19 19:54:11.000000 composio_core-0.1.9/composio/sdk/sdk.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1264 2024-03-16 12:05:30.000000 composio_core-0.1.9/composio/sdk/storage.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1614 2024-03-19 16:11:07.000000 composio_core-0.1.9/composio/sdk/utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-03-19 19:55:20.130243 composio_core-0.1.9/composio_core.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      740 2024-03-19 19:55:20.000000 composio_core-0.1.9/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-03-19 19:55:20.000000 composio_core-0.1.9/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-03-19 19:55:20.000000 composio_core-0.1.9/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-03-19 19:55:20.000000 composio_core-0.1.9/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       77 2024-03-19 19:55:20.000000 composio_core-0.1.9/composio_core.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-03-19 19:55:20.000000 composio_core-0.1.9/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      488 2024-03-19 12:07:26.000000 composio_core-0.1.9/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       75 2024-03-19 10:13:31.000000 composio_core-0.1.9/requirements.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-03-19 19:55:20.130763 composio_core-0.1.9/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1157 2024-03-19 19:55:09.000000 composio_core-0.1.9/setup.py
```

### Comparing `composio_core-0.1.8/PKG-INFO` & `composio_core-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.8
+Version: 0.1.9
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.8/composio/composio_cli.py` & `composio_core-0.1.9/composio/composio_cli.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.8/composio/sdk/core.py` & `composio_core-0.1.9/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.8/composio/sdk/enums.py` & `composio_core-0.1.9/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.8/composio/sdk/sdk.py` & `composio_core-0.1.9/composio/sdk/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     OPENAI = "openai"
     DEFAULT = "default"
 
 class ConnectionRequest(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
     connectionStatus: str
     connectedAccountId: str
-    redirectUrl: str
+    redirectUrl: Optional[str] = None
 
     sdk_instance: 'Composio' = None
 
     def __init__(self, sdk_instance: 'Composio', **data):
         super().__init__(**data)
         self.sdk_instance = sdk_instance
 
@@ -134,18 +134,18 @@
 
     sdk_instance: 'Composio' = None  # type: ignore
 
     def __init__(self, sdk_instance: 'Composio', **data):
         super().__init__(**data)
         self.sdk_instance = sdk_instance
     
-    def initiate_connection(self, user_uuid: str = None) -> ConnectionRequest:
-        connector_id = f"test-{self.appName}-connector"
+    def initiate_connection(self, user_uuid: str = None, params: dict = {}) -> ConnectionRequest:
         resp = self.sdk_instance.http_client.post(f"{self.sdk_instance.base_url}/v1/connectedAccounts", json={
-            "integrationId": connector_id,
+            "integrationId": self.id,
+            "data": params
         })
         if resp.status_code == 200:
             return ConnectionRequest(self.sdk_instance, **resp.json())
         
         raise Exception("Failed to create connection")
     
     def get_required_variables(self):
```

### Comparing `composio_core-0.1.8/composio/sdk/storage.py` & `composio_core-0.1.9/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.8/composio/sdk/utils.py` & `composio_core-0.1.9/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.8/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.9/composio_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.8
+Version: 0.1.9
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.8/setup.py` & `composio_core-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class InstallCommandMiddleware(install):
     """Customized setuptools install command."""
     def run(self):
         install.run(self)
         
 setup(
     name = 'composio_core',
-    version = '0.1.8',
+    version = '0.1.9',
     author = 'Utkarsh',
     author_email = 'utkarsh@composio.dev',
     description = 'Core package to act as a bridge between composio platform and other services.',
     long_description = open(readme_path).read(),
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/SamparkAI/composio_sdk',
     classifiers = [
```

