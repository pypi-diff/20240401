# Comparing `tmp/ctfd_sdk-0.2.1.tar.gz` & `tmp/ctfd_sdk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctfd_sdk-0.2.1.tar", max compression
+gzip compressed data, was "ctfd_sdk-0.2.2.tar", max compression
```

## Comparing `ctfd_sdk-0.2.1.tar` & `ctfd_sdk-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      103 2024-03-02 13:18:24.629737 ctfd_sdk-0.2.1/README.md
--rw-r--r--   0        0        0       33 2024-03-07 08:36:18.279058 ctfd_sdk-0.2.1/ctfd_sdk/__init__.py
--rw-r--r--   0        0        0    18458 2024-03-07 14:01:57.252101 ctfd_sdk-0.2.1/ctfd_sdk/api.py
--rw-r--r--   0        0        0      304 2024-03-01 14:57:33.013442 ctfd_sdk-0.2.1/ctfd_sdk/settings.py
--rw-r--r--   0        0        0      543 2024-03-07 14:02:14.396309 ctfd_sdk-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 ctfd_sdk-0.2.1/setup.py
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 ctfd_sdk-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      103 2024-03-02 13:18:24.629737 ctfd_sdk-0.2.2/README.md
+-rw-r--r--   0        0        0       70 2024-04-01 14:31:26.410675 ctfd_sdk-0.2.2/ctfd_sdk/__init__.py
+-rw-r--r--   0        0        0    20961 2024-04-01 14:30:17.821536 ctfd_sdk-0.2.2/ctfd_sdk/api.py
+-rw-r--r--   0        0        0      304 2024-03-01 14:57:33.013442 ctfd_sdk-0.2.2/ctfd_sdk/settings.py
+-rw-r--r--   0        0        0      543 2024-04-01 14:31:57.631185 ctfd_sdk-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 ctfd_sdk-0.2.2/setup.py
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 ctfd_sdk-0.2.2/PKG-INFO
```

### Comparing `ctfd_sdk-0.2.1/ctfd_sdk/api.py` & `ctfd_sdk-0.2.2/ctfd_sdk/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from ctfd_sdk import settings
 
 
 class CTFdException(Exception):
     pass
 
 
+class CTFdRequestException(Exception):
+    pass
+
+
 class CtfdConnector:
     def __init__(self, admin_token: str, host: str):
         admin_token = admin_token or settings.CTFD_ADMIN_TOKEN
         assert admin_token is not None, 'To use ctfd you need to define "CTFD_ADMIN_TOKEN"'
         self.admin_token = admin_token
         host = host or settings.CTFD_HOST
         assert host is not None, 'To use ctfd you need to define "CTFD_HOST"'
@@ -54,57 +58,92 @@
 
         return inner
 
     @aassign_host
     async def aget(self, url, *args, **kwargs):
         async with httpx.AsyncClient() as client:
             response = await client.get(url, *args, **kwargs)
+        if response.status_code not in [200, 201]:
+            self.logger.warning(f'Unable to get response in method get from url {url}  in CTFd: {response.text}')
+            raise CTFdRequestException(f'Unable to get response in method get from url {url}  in CTFd: {response.text}')
         return response
 
     @aassign_host
     async def apost(self, url, *args, **kwargs):
         async with httpx.AsyncClient() as client:
             response = await client.post(url, *args, **kwargs)
-            # response.status_code = 1
+        if response.status_code not in [200, 201]:
+            self.logger.warning(f'Unable to get response in method post from url {url}  in CTFd: {response.text}')
+            raise CTFdRequestException(
+                f'Unable to get response in method post from url {url}  in CTFd: {response.text}'
+            )
         return response
 
     @aassign_host
     async def apatch(self, url, *args, **kwargs):
         async with httpx.AsyncClient() as client:
             response = await client.patch(url, *args, **kwargs)
+        if response.status_code not in [200, 201]:
+            self.logger.warning(f'Unable to get response in method patch from url {url}  in CTFd: {response.text}')
+            raise CTFdRequestException(
+                f'Unable to get response in method patch from url {url}  in CTFd: {response.text}'
+            )
         return response
 
     @aassign_host
     async def adelete(self, url, *args, **kwargs):
         async with httpx.AsyncClient() as client:
             response = await client.delete(url, *args, **kwargs)
+        if response.status_code not in [200, 201]:
+            self.logger.warning(f'Unable to get response in method delete from url {url}  in CTFd: {response.text}')
+            raise CTFdRequestException(
+                f'Unable to get response in method delete from url {url}  in CTFd: {response.text}'
+            )
         return response
 
     @assign_host
     def get(self, url, *args, **kwargs):
         with httpx.Client() as client:
             response = client.get(url, *args, **kwargs)
+        if response.status_code not in [200, 201]:
+            self.logger.warning(f'Unable to get response in method get from url {url}  in CTFd: {response.text}')
+            raise CTFdRequestException(f'Unable to get response in method get from url {url}  in CTFd: {response.text}')
         return response
 
     @assign_host
     def post(self, url, *args, **kwargs):
         with httpx.Client() as client:
             response = client.post(url, *args, **kwargs)
+        if response.status_code not in [200, 201]:
+            self.logger.warning(f'Unable to get response in method post from url {url}  in CTFd: {response.text}')
+            raise CTFdRequestException(
+                f'Unable to get response in method post from url {url}  in CTFd: {response.text}'
+            )
         return response
 
     @assign_host
     def patch(self, url, *args, **kwargs):
         with httpx.Client() as client:
             response = client.patch(url, *args, **kwargs)
+        if response.status_code not in [200, 201]:
+            self.logger.warning(f'Unable to get response in method patch from url {url}  in CTFd: {response.text}')
+            raise CTFdRequestException(
+                f'Unable to get response in method patch from url {url}  in CTFd: {response.text}'
+            )
         return response
 
     @assign_host
     def delete(self, url, *args, **kwargs):
         with httpx.Client() as client:
             response = client.delete(url, *args, **kwargs)
+        if response.status_code not in [200, 201]:
+            self.logger.warning(f'Unable to get response in method delete from url {url}  in CTFd: {response.text}')
+            raise CTFdRequestException(
+                f'Unable to get response in method delete from url {url}  in CTFd: {response.text}'
+            )
         return response
 
 
 class Storage:
     def __init__(self, storage_path: str | Path):
         storage_path = storage_path or settings.CTFD_STORAGE
         assert storage_path is not None, 'To use ctfd you need to define "CTFD_STORAGE"'
```

### Comparing `ctfd_sdk-0.2.1/pyproject.toml` & `ctfd_sdk-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctfd-sdk"
-version = "0.2.1"
+version = "0.2.2"
 description = "Python SDK for CTFd REST API"
 authors = ["Simon Plhak <plhak.s@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ctfd_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `ctfd_sdk-0.2.1/setup.py` & `ctfd_sdk-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['httpx>=0.27.0,<0.28.0', 'python-dotenv>=1.0.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'ctfd-sdk',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Python SDK for CTFd REST API',
     'long_description': '# CTFd SDK for Python\n\n## Setup\n\n```bash\npython -m venv env\nsource env/bin/activate\npoetry install\n```\n',
     'author': 'Simon Plhak',
     'author_email': 'plhak.s@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ctfd_sdk-0.2.1/PKG-INFO` & `ctfd_sdk-0.2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctfd-sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python SDK for CTFd REST API
 Author: Simon Plhak
 Author-email: plhak.s@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

