# Comparing `tmp/vysion-1.0.8.tar.gz` & `tmp/vysion-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vysion-1.0.8.tar", max compression
+gzip compressed data, was "vysion-1.0.9.tar", max compression
```

## Comparing `vysion-1.0.8.tar` & `vysion-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11356 2023-04-12 11:01:34.010455 vysion-1.0.8/LICENSE
--rw-r--r--   0        0        0     1049 2023-06-01 15:09:56.590723 vysion-1.0.8/README.md
--rw-r--r--   0        0        0      977 2023-10-24 07:52:57.449642 vysion-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      664 2023-06-01 15:09:56.590723 vysion-1.0.8/vysion/__init__.py
--rw-r--r--   0        0        0      630 2023-06-01 15:09:56.590723 vysion-1.0.8/vysion/client/__init__.py
--rw-r--r--   0        0        0     9512 2023-09-06 09:19:33.218356 vysion-1.0.8/vysion/client/client.py
--rw-r--r--   0        0        0     1176 2023-04-12 11:01:34.010455 vysion-1.0.8/vysion/client/error.py
--rw-r--r--   0        0        0      605 2023-04-12 11:01:34.010455 vysion-1.0.8/vysion/dto/__init__.py
--rw-r--r--   0        0        0     6953 2023-10-24 08:40:42.258200 vysion-1.0.8/vysion/dto/dto.py
--rw-r--r--   0        0        0     1488 2023-09-06 09:19:33.218356 vysion-1.0.8/vysion/dto/tag.py
--rw-r--r--   0        0        0     4456 2023-10-24 07:40:56.018519 vysion-1.0.8/vysion/dto/util.py
--rw-r--r--   0        0        0      627 2023-06-01 15:09:56.590723 vysion-1.0.8/vysion/model/__init__.py
--rw-r--r--   0        0        0      690 2023-06-01 15:09:56.590723 vysion-1.0.8/vysion/model/enum/__init__.py
--rw-r--r--   0        0        0     4205 2023-09-06 09:19:33.218356 vysion-1.0.8/vysion/model/enum/languages.py
--rw-r--r--   0        0        0      789 2023-04-12 11:01:34.010455 vysion-1.0.8/vysion/model/enum/networks.py
--rw-r--r--   0        0        0     1527 2023-04-12 11:01:34.010455 vysion-1.0.8/vysion/model/enum/ransom_groups.py
--rw-r--r--   0        0        0     5569 2023-04-12 11:01:34.010455 vysion-1.0.8/vysion/model/enum/services.py
--rw-r--r--   0        0        0     4778 2023-09-06 09:19:33.218356 vysion-1.0.8/vysion/model/model.py
--rw-r--r--   0        0        0      635 2023-06-01 15:09:56.590723 vysion-1.0.8/vysion/taxonomy/__init__.py
--rw-r--r--   0        0        0     2347 2023-04-12 11:01:34.010455 vysion-1.0.8/vysion/taxonomy/flavours.py
--rw-r--r--   0        0        0    12264 2023-09-06 09:19:33.218356 vysion-1.0.8/vysion/taxonomy/taxonomy.py
--rw-r--r--   0        0        0      610 2023-09-06 09:19:33.218356 vysion-1.0.8/vysion/version.py
--rw-r--r--   0        0        0     2090 1970-01-01 00:00:00.000000 vysion-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-12-01 08:02:25.765185 vysion-1.0.9/LICENSE
+-rw-r--r--   0        0        0     1428 2023-12-11 12:05:33.856081 vysion-1.0.9/README.md
+-rw-r--r--   0        0        0      977 2023-12-19 12:46:55.190555 vysion-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      664 2023-12-01 08:02:25.769185 vysion-1.0.9/vysion/__init__.py
+-rw-r--r--   0        0        0      630 2023-12-01 08:02:25.769185 vysion-1.0.9/vysion/client/__init__.py
+-rw-r--r--   0        0        0     9747 2023-12-11 12:05:33.856081 vysion-1.0.9/vysion/client/client.py
+-rw-r--r--   0        0        0     1176 2023-12-01 08:02:25.769185 vysion-1.0.9/vysion/client/error.py
+-rw-r--r--   0        0        0      605 2023-12-01 08:02:25.769185 vysion-1.0.9/vysion/dto/__init__.py
+-rw-r--r--   0        0        0     6953 2023-12-01 08:02:25.769185 vysion-1.0.9/vysion/dto/dto.py
+-rw-r--r--   0        0        0     1488 2023-12-01 08:02:25.769185 vysion-1.0.9/vysion/dto/tag.py
+-rw-r--r--   0        0        0     4456 2023-12-01 08:02:25.769185 vysion-1.0.9/vysion/dto/util.py
+-rw-r--r--   0        0        0      627 2023-12-01 08:02:25.769185 vysion-1.0.9/vysion/model/__init__.py
+-rw-r--r--   0        0        0      690 2023-12-01 08:02:25.769185 vysion-1.0.9/vysion/model/enum/__init__.py
+-rw-r--r--   0        0        0     4205 2023-12-01 08:02:25.769185 vysion-1.0.9/vysion/model/enum/languages.py
+-rw-r--r--   0        0        0      789 2023-12-01 08:02:25.769185 vysion-1.0.9/vysion/model/enum/networks.py
+-rw-r--r--   0        0        0     1527 2023-12-01 08:02:25.769185 vysion-1.0.9/vysion/model/enum/ransom_groups.py
+-rw-r--r--   0        0        0     5569 2023-12-01 08:02:25.769185 vysion-1.0.9/vysion/model/enum/services.py
+-rw-r--r--   0        0        0     4778 2023-12-01 08:02:25.773185 vysion-1.0.9/vysion/model/model.py
+-rw-r--r--   0        0        0      635 2023-12-01 08:02:25.773185 vysion-1.0.9/vysion/taxonomy/__init__.py
+-rw-r--r--   0        0        0     2347 2023-12-01 08:02:25.773185 vysion-1.0.9/vysion/taxonomy/flavours.py
+-rw-r--r--   0        0        0    12264 2023-12-01 08:02:25.773185 vysion-1.0.9/vysion/taxonomy/taxonomy.py
+-rw-r--r--   0        0        0      610 2023-12-01 08:02:25.773185 vysion-1.0.9/vysion/version.py
+-rw-r--r--   0        0        0     2371 1970-01-01 00:00:00.000000 vysion-1.0.9/PKG-INFO
```

### Comparing `vysion-1.0.8/LICENSE` & `vysion-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/README.md` & `vysion-1.0.9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,20 @@
+# Vysion-PY
 
-# References
+Welcome to the open source repository for vysion-py, our implementation as a Python library to use the Vysion tool. 
 
+You can request a demo or an api-key on our [website](https://byronlabs.io) or at [vysion.ai](https://vysion.ai).
+
+Latest version: [1.0.8](https://pypi.org/project/vysion/)
+
+
+## References
+
+- https://pypi.org/project/vysion/
+- https://developers.vysion.ai?python
 - https://pydantic-docs.helpmanual.io/
 - https://python-patterns.guide/
 - https://docs.pytest.org/en/7.1.x/getting-started.html#get-started
 - https://github.com/samuelcolvin/pydantic
 - https://python-poetry.org/docs/pyproject
 - https://github.com/wemake-services/wemake-python-package
```

### Comparing `vysion-1.0.8/pyproject.toml` & `vysion-1.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vysion"
-version = "1.0.8"
+version = "1.0.9"
 description = "The official Python client library for Vysion"
 homepage = "https://vysion.ai"
 repository = "https://gitlab.com/byronlabs/vysion/vysion-py"
 documentation = "https://developers.vysion.ai"
 authors = [
   "Javier Junquera-Sánchez <javier.junquera@byronlabs.io>"
 ]
@@ -14,18 +14,18 @@
    "Programming Language :: Python :: 3",
    "License :: OSI Approved :: Apache Software License",
    "Operating System :: OS Independent"
 ]
 # packages = [vysion', 'vysion.client', 'vysion.model',  'vysion.dto', 'vysion.taxonomy'],
 
 [tool.poetry.dependencies]
-python = "^3.7.0"
+python = "^3.8.0"
 
 pydantic = "^2.0.1"
-pymisp = "2.4.159"
+pymisp = "2.4.175"
 softenum = "1.0.1"
 requests = "^2.28.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "7.1.2"
 python-dotenv = "0.19.2"
```

### Comparing `vysion-1.0.8/vysion/__init__.py` & `vysion-1.0.9/vysion/__init__.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/vysion/client/__init__.py` & `vysion-1.0.9/vysion/client/__init__.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/vysion/client/client.py` & `vysion-1.0.9/vysion/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,22 +26,20 @@
 import requests
 
 import vysion.dto as dto
 from vysion.client.error import APIError
 from vysion.dto import VysionError
 from vysion.version import __version__ as vysion_version
 
-_API_HOST = "https://api.vysion.ai"
+import os
 
 # All API endpoints start with this prefix, you don't need to include the
 # prefix in the paths you request as it's prepended automatically.
 _ENDPOINT_PREFIX = "/api/v1/"
 
-_BASE_API = urljoin(_API_HOST, _ENDPOINT_PREFIX)
-
 LOGGER = logging.getLogger("vysion-py")
 LOGGER.setLevel(logging.INFO)
 
 # __all__ = []
 
 
 class BaseClient:
@@ -77,17 +75,30 @@
 
             self._session: requests.Session = requests.Session()
             self._session.headers.update(headers)
             self._session.proxies = self.proxy
 
         return self._session
 
+    def _get_api_host(self):
+
+        if os.getenv("API_HOST") is not None:
+            api_host = os.getenv("API_HOST")
+
+        else:
+            api_host = "https://api.vysion.ai"
+
+        return api_host
+    
+
     def _build_api_url__(self, endpoint, param, **query_params):
 
         param = quote(param, safe='')
+        _API_HOST = self._get_api_host()
+        _BASE_API = urljoin(_API_HOST, _ENDPOINT_PREFIX)
         base = urljoin(_BASE_API, f"{endpoint}/{param}")
 
         query_params_initialzed = query_params.copy()
 
         keys = list(query_params.keys())
         keys.sort()
 
@@ -349,8 +360,8 @@
         pages = (end_time - start_time).days
 
         for page in range(pages):
             url = self._build_api_url__("feed", "ransomware", days=days, page=page + 1)
             yield self._make_request(url)
 
 
-# TODO /api/v1/feeds
+# TODO /api/v1/feeds
```

### Comparing `vysion-1.0.8/vysion/client/error.py` & `vysion-1.0.9/vysion/client/error.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/vysion/dto/__init__.py` & `vysion-1.0.9/vysion/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/vysion/dto/dto.py` & `vysion-1.0.9/vysion/dto/dto.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/vysion/dto/tag.py` & `vysion-1.0.9/vysion/dto/tag.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/vysion/dto/util.py` & `vysion-1.0.9/vysion/dto/util.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/vysion/model/__init__.py` & `vysion-1.0.9/vysion/model/__init__.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/vysion/model/enum/__init__.py` & `vysion-1.0.9/vysion/model/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/vysion/model/enum/languages.py` & `vysion-1.0.9/vysion/model/enum/languages.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/vysion/model/enum/networks.py` & `vysion-1.0.9/vysion/model/enum/networks.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/vysion/model/enum/ransom_groups.py` & `vysion-1.0.9/vysion/model/enum/ransom_groups.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/vysion/model/enum/services.py` & `vysion-1.0.9/vysion/model/enum/services.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/vysion/model/model.py` & `vysion-1.0.9/vysion/model/model.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/vysion/taxonomy/__init__.py` & `vysion-1.0.9/vysion/taxonomy/__init__.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/vysion/taxonomy/flavours.py` & `vysion-1.0.9/vysion/taxonomy/flavours.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/vysion/taxonomy/taxonomy.py` & `vysion-1.0.9/vysion/taxonomy/taxonomy.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/vysion/version.py` & `vysion-1.0.9/vysion/version.py`

 * *Files identical despite different names*

### Comparing `vysion-1.0.8/PKG-INFO` & `vysion-1.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 Metadata-Version: 2.1
 Name: vysion
-Version: 1.0.8
+Version: 1.0.9
 Summary: The official Python client library for Vysion
 Home-page: https://vysion.ai
 License: Apache-2.0
 Author: Javier Junquera-Sánchez
 Author-email: javier.junquera@byronlabs.io
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: pydantic (>=2.0.1,<3.0.0)
-Requires-Dist: pymisp (==2.4.159)
+Requires-Dist: pymisp (==2.4.175)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: softenum (==1.0.1)
 Project-URL: Documentation, https://developers.vysion.ai
 Project-URL: Repository, https://gitlab.com/byronlabs/vysion/vysion-py
 Description-Content-Type: text/markdown
 
+# Vysion-PY
+
+Welcome to the open source repository for vysion-py, our implementation as a Python library to use the Vysion tool. 
+
+You can request a demo or an api-key on our [website](https://byronlabs.io) or at [vysion.ai](https://vysion.ai).
+
+Latest version: [1.0.8](https://pypi.org/project/vysion/)
+
 
-# References
+## References
 
+- https://pypi.org/project/vysion/
+- https://developers.vysion.ai?python
 - https://pydantic-docs.helpmanual.io/
 - https://python-patterns.guide/
 - https://docs.pytest.org/en/7.1.x/getting-started.html#get-started
 - https://github.com/samuelcolvin/pydantic
 - https://python-poetry.org/docs/pyproject
 - https://github.com/wemake-services/wemake-python-package
```

