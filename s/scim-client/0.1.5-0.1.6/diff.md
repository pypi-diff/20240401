# Comparing `tmp/scim_client-0.1.5.tar.gz` & `tmp/scim_client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scim_client-0.1.5.tar", last modified: Mon Apr  1 07:09:52 2024, max compression
+gzip compressed data, was "scim_client-0.1.6.tar", last modified: Mon Apr  1 11:01:38 2024, max compression
```

## Comparing `scim_client-0.1.5.tar` & `scim_client-0.1.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:09:52.247007 scim_client-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-01 07:09:48.000000 scim_client-0.1.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-01 07:09:48.000000 scim_client-0.1.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-01 07:09:48.000000 scim_client-0.1.5/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-01 07:09:48.000000 scim_client-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-01 07:09:48.000000 scim_client-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-01 07:09:52.247007 scim_client-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-01 07:09:48.000000 scim_client-0.1.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:09:52.243007 scim_client-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-01 07:09:48.000000 scim_client-0.1.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 07:09:48.000000 scim_client-0.1.5/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4842 2024-04-01 07:09:48.000000 scim_client-0.1.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 07:09:48.000000 scim_client-0.1.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 07:09:48.000000 scim_client-0.1.5/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-01 07:09:48.000000 scim_client-0.1.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-01 07:09:48.000000 scim_client-0.1.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-01 07:09:48.000000 scim_client-0.1.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-01 07:09:48.000000 scim_client-0.1.5/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-01 07:09:48.000000 scim_client-0.1.5/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:09:52.247007 scim_client-0.1.5/scim_client/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-01 07:09:48.000000 scim_client-0.1.5/scim_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 07:09:48.000000 scim_client-0.1.5/scim_client/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 07:09:48.000000 scim_client-0.1.5/scim_client/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-01 07:09:48.000000 scim_client-0.1.5/scim_client/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-01 07:09:48.000000 scim_client-0.1.5/scim_client/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-01 07:09:48.000000 scim_client-0.1.5/scim_client/scim_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-01 07:09:48.000000 scim_client-0.1.5/scim_client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:09:52.247007 scim_client-0.1.5/scim_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-01 07:09:52.000000 scim_client-0.1.5/scim_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-01 07:09:52.000000 scim_client-0.1.5/scim_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 07:09:52.000000 scim_client-0.1.5/scim_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 07:09:52.000000 scim_client-0.1.5/scim_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 07:09:52.000000 scim_client-0.1.5/scim_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-01 07:09:52.247007 scim_client-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-01 07:09:48.000000 scim_client-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:09:52.247007 scim_client-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-01 07:09:48.000000 scim_client-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-04-01 07:09:48.000000 scim_client-0.1.5/tests/test_scim_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:38.269898 scim_client-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-01 11:01:34.000000 scim_client-0.1.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-01 11:01:34.000000 scim_client-0.1.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-01 11:01:34.000000 scim_client-0.1.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-01 11:01:34.000000 scim_client-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-01 11:01:34.000000 scim_client-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-01 11:01:38.269898 scim_client-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-01 11:01:34.000000 scim_client-0.1.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:38.265898 scim_client-0.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4842 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:38.269898 scim_client-0.1.6/scim_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-01 11:01:34.000000 scim_client-0.1.6/scim_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 11:01:34.000000 scim_client-0.1.6/scim_client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 11:01:34.000000 scim_client-0.1.6/scim_client/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-01 11:01:34.000000 scim_client-0.1.6/scim_client/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-01 11:01:34.000000 scim_client-0.1.6/scim_client/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-01 11:01:34.000000 scim_client-0.1.6/scim_client/scim_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-01 11:01:34.000000 scim_client-0.1.6/scim_client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:38.269898 scim_client-0.1.6/scim_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-01 11:01:38.000000 scim_client-0.1.6/scim_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-01 11:01:38.000000 scim_client-0.1.6/scim_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:01:38.000000 scim_client-0.1.6/scim_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:01:38.000000 scim_client-0.1.6/scim_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 11:01:38.000000 scim_client-0.1.6/scim_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-01 11:01:38.269898 scim_client-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-01 11:01:34.000000 scim_client-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:38.269898 scim_client-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-01 11:01:34.000000 scim_client-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-01 11:01:34.000000 scim_client-0.1.6/tests/test_scim_client.py
```

### Comparing `scim_client-0.1.5/CONTRIBUTING.rst` & `scim_client-0.1.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.5/LICENSE` & `scim_client-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.5/PKG-INFO` & `scim_client-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scim_client
-Version: 0.1.5
+Version: 0.1.6
 Summary: SCIM v2 API client
 Home-page: https://github.com/Aplopio/python-scim-client
 Author: Mitratech Development Team
 Author-email: devs@mitratech.com
 License: MIT license
 Keywords: scim_client
 Classifier: Development Status :: 4 - Beta
```

### Comparing `scim_client-0.1.5/README.rst` & `scim_client-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.5/docs/Makefile` & `scim_client-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.5/docs/conf.py` & `scim_client-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.5/docs/installation.rst` & `scim_client-0.1.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.5/docs/make.bat` & `scim_client-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.5/scim_client/resources.py` & `scim_client-0.1.6/scim_client/resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Any, Optional, List
+from typing import Dict, Any, Optional, List, Union
 
 from .defaults import Sentinel
 from .utils import (
     _to_dict_without_not_given,
     _to_snake_cased,
     _get_extension_key,
     _to_snake_case_key,
@@ -70,14 +70,15 @@
     def __init__(self, **kwargs):
         for key, value in kwargs.items():
             setattr(self, key, value)
 
 
 class User(BaseResource):
     CORE_SCHEMA = "urn:ietf:params:scim:schemas:core:2.0:User"
+
     id: str
     external_id: str
     user_name: str
     display_name: str
     active: bool
     meta: Dict
     name: UserName
@@ -91,54 +92,58 @@
         *,
         id: str,
         external_id: str,
         user_name: str,
         active: bool,
         name: Dict,
         display_name: str,
-        emails: List[Dict[str, str | bool]],
-        schemas: List[str],
-        meta: Optional[Dict],
+        emails: List[Dict[str, Union[str, bool]]],
+        meta: Optional[Dict] = None,
+        schemas: Optional[List[str]] = None,
         timezone: Optional[str] = None,
         **kwargs
     ) -> None:
         self.user_name = user_name
         self.id = id
         self.external_id = external_id
         self.active = active
         self.name = UserName(**name)
         self.emails = [UserEmail(**e) for e in emails]
         self.display_name = display_name
         self.timezone = timezone
         self.meta = meta
-        self.schemas = schemas
+        self.schemas = schemas if schemas is not None else [self.CORE_SCHEMA]
         self.extra_fields = kwargs
 
         if len(self.schemas) > 1:
             for sc in self.schemas:
                 if sc != self.CORE_SCHEMA:
                     extension_key = _to_snake_case_key(_get_extension_key(sc))
                     setattr(
                         self,
                         extension_key,
                         UserExtension(**kwargs.get(extension_key, {})),
                     )
 
 
 class UserSearch(BaseResource):
+    CORE_SCHEMA = "urn:ietf:params:scim:api:messages:2.0:ListResponse"
+
     resources: List[User]
     total_results: int
     items_per_page: int
     start_index: int
-    schemas: List[str] = ["urn:ietf:params:scim:api:messages:2.0:ListResponse"]
+    schemas: List[str]
 
     def __init__(
         self,
         resources: List[Dict[str, Any]],
         total_results: int,
         items_per_page: int,
         start_index: int,
+        schemas: Optional[List[str]] = None,
     ):
         self.resources = [User(**r) for r in resources]
         self.total_results = total_results
         self.items_per_page = items_per_page
         self.start_index = start_index
+        self.schemas = schemas if schemas is not None else [self.CORE_SCHEMA]
```

### Comparing `scim_client-0.1.5/scim_client/response.py` & `scim_client-0.1.6/scim_client/response.py`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.5/scim_client/scim_client.py` & `scim_client-0.1.6/scim_client/scim_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,22 +37,24 @@
     UserSearchCls: Type[UserSearch]
 
     def __init__(
         self,
         base_url: str,
         token: str,
         timeout: int = 30,
+        max_retries: int = 3,
         default_headers: Optional[Dict[str, str]] = None,
         logger: Optional[logging.Logger] = None,
     ):
         self.token = token
         self.timeout = timeout
         self.base_url = base_url
         self.default_headers = default_headers if default_headers else {}
         self.logger = logger if logger is not None else logging.getLogger(__name__)
+        self.max_retries = max_retries
 
     def search_users(self, q: str, count: int = 20, start_index: int = 0) -> UserSearch:
         """Search or filter users by query."""
 
         scim_response = self._make_request(
             method="GET",
             resource="Users",
@@ -123,30 +125,42 @@
 
         if data is not None:
             request_kwargs["data"] = json.dumps(data).encode("utf-8")
 
         if query_params is not None:
             url = url + "?" + urlencode(query_params)
 
-        while True:
+        retries_left = self.max_retries
+        http_error = None
+        while retries_left > 0:
             try:
                 request = Request(**request_kwargs, method=method)
                 with urllib.request.urlopen(request) as resp:
-                    resp.raise_for_status()
+                    if 500 <= resp.status < 600:
+                        raise HTTPError(
+                            url=url,
+                            code=resp.status,
+                            msg=f"{resp.status} Server Error",
+                            fp=resp,
+                            hdrs=resp.getheaders(),
+                        )
                     return SCIMResponse(
                         url=url,
-                        status_code=resp.status_code,
-                        raw_body=resp.content.decode("utf-8"),
+                        status_code=resp.status,
+                        raw_body=resp.read().decode("utf-8"),
                         headers=resp.headers,
                     )
             except HTTPError as he:
+                http_error = he
                 if he.code >= 500:
                     self.logger.warning(
                         "HTTP error url={} code={} reason={} headers={}".format(
                             he.url, he.code, he.reason, he.headers
                         )
                     )
-                    # add retry logic here
-                    time.sleep(2)
-                    continue
+                    time.sleep(self.max_retries - retries_left + 1)
+                    retries_left -= 1
                 else:
                     raise he
+
+        if http_error is not None:
+            raise http_error
```

### Comparing `scim_client-0.1.5/scim_client/utils.py` & `scim_client-0.1.6/scim_client/utils.py`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.5/scim_client.egg-info/PKG-INFO` & `scim_client-0.1.6/scim_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scim_client
-Version: 0.1.5
+Version: 0.1.6
 Summary: SCIM v2 API client
 Home-page: https://github.com/Aplopio/python-scim-client
 Author: Mitratech Development Team
 Author-email: devs@mitratech.com
 License: MIT license
 Keywords: scim_client
 Classifier: Development Status :: 4 - Beta
```

### Comparing `scim_client-0.1.5/scim_client.egg-info/SOURCES.txt` & `scim_client-0.1.6/scim_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.5/setup.py` & `scim_client-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.5/tests/test_scim_client.py` & `scim_client-0.1.6/tests/test_scim_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
             display_name="Raj Kumar",
             meta={
                 "resource_type": "User",
                 "created": "2024-01-19T00:03:02.634696",
                 "last_modified": "2024-01-19T00:03:02.634696",
                 "location": "%s/Users/23o4uoqiweu" % self.scim_base_url,
             },
-            schemas=["urn:ietf:params:scim:schemas:core:2.0:User"],
         )
 
     def get_resource_url(self, resource: str):
         return "%s/%s" % (self.scim_base_url, resource)
 
     def test_read_user(self) -> None:
         user_id = "3423yer89qw6d9"
```

