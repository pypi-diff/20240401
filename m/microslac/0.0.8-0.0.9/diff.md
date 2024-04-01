# Comparing `tmp/microslac-0.0.8.tar.gz` & `tmp/microslac-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microslac-0.0.8.tar", max compression
+gzip compressed data, was "microslac-0.0.9.tar", max compression
```

## Comparing `microslac-0.0.8.tar` & `microslac-0.0.9.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0        0 2024-03-21 16:44:34.315125 microslac-0.0.8/README.md
--rw-r--r--   0        0        0     1109 2024-03-25 14:59:39.976900 microslac-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-21 16:45:59.737289 microslac-0.0.8/src/micro/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 16:45:59.737289 microslac-0.0.8/src/micro/fast/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 16:45:59.737289 microslac-0.0.8/src/micro/jango/__init__.py
--rw-r--r--   0        0        0       30 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/commands/__init__.py
--rw-r--r--   0        0        0       88 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/commands/base.py
--rw-r--r--   0        0        0       37 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/constants/__init__.py
--rw-r--r--   0        0        0      328 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/constants/base.py
--rw-r--r--   0        0        0       36 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/exceptions/__init__.py
--rw-r--r--   0        0        0      967 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/exceptions/exception.py
--rw-r--r--   0        0        0     1439 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/exceptions/handler.py
--rw-r--r--   0        0        0        0 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/middlewares/__init__.py
--rw-r--r--   0        0        0      670 2024-03-25 14:56:39.444948 microslac-0.0.8/src/micro/jango/middlewares/api.py
--rw-r--r--   0        0        0     1097 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/middlewares/authentication.py
--rw-r--r--   0        0        0      195 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/models/__init__.py
--rw-r--r--   0        0        0      439 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/models/fields.py
--rw-r--r--   0        0        0     1917 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/models/history.py
--rw-r--r--   0        0        0      205 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/models/manager.py
--rw-r--r--   0        0        0       79 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/models/queryset.py
--rw-r--r--   0        0        0      195 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/models/uuid.py
--rw-r--r--   0        0        0       33 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/permissions/__init__.py
--rw-r--r--   0        0        0      330 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/permissions/internal.py
--rw-r--r--   0        0        0       28 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/queues/__init__.py
--rw-r--r--   0        0        0     3155 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/queues/base.py
--rw-r--r--   0        0        0       35 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/renderers/__init__.py
--rw-r--r--   0        0        0      997 2024-03-25 14:48:46.861216 microslac-0.0.8/src/micro/jango/renderers/json.py
--rw-r--r--   0        0        0      103 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/serializers/__init__.py
--rw-r--r--   0        0        0      993 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/serializers/base.py
--rw-r--r--   0        0        0     1317 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/serializers/fields.py
--rw-r--r--   0        0        0       30 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/services/__init__.py
--rw-r--r--   0        0        0       59 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/services/base.py
--rw-r--r--   0        0        0       44 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/tests/__init__.py
--rw-r--r--   0        0        0     2094 2024-03-25 14:59:25.697212 microslac-0.0.8/src/micro/jango/tests/base.py
--rw-r--r--   0        0        0      874 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/utils/__init__.py
--rw-r--r--   0        0        0       62 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/views/__init__.py
--rw-r--r--   0        0        0      621 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/jango/views/base.py
--rw-r--r--   0        0        0        0 2024-03-21 16:45:59.737289 microslac-0.0.8/src/micro/patterns/__init__.py
--rw-r--r--   0        0        0     1242 2024-03-06 17:42:01.785756 microslac-0.0.8/src/micro/patterns/null.py
--rw-r--r--   0        0        0     2117 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/patterns/saga.py
--rw-r--r--   0        0        0        0 2024-03-21 16:45:59.737289 microslac-0.0.8/src/micro/services/__init__.py
--rw-r--r--   0        0        0     2738 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/services/base.py
--rw-r--r--   0        0        0      510 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/services/registry.py
--rw-r--r--   0        0        0        0 2024-03-21 16:45:59.737289 microslac-0.0.8/src/micro/utils/__init__.py
--rw-r--r--   0        0        0     3058 2024-03-25 14:01:51.479238 microslac-0.0.8/src/micro/utils/utils.py
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 microslac-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-21 16:44:34.315125 microslac-0.0.9/README.md
+-rw-r--r--   0        0        0     1051 2024-03-26 03:30:57.061874 microslac-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-21 16:45:59.737289 microslac-0.0.9/src/micro/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 16:45:59.737289 microslac-0.0.9/src/micro/fast/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 16:45:59.737289 microslac-0.0.9/src/micro/jango/__init__.py
+-rw-r--r--   0        0        0       30 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/commands/__init__.py
+-rw-r--r--   0        0        0       88 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/commands/base.py
+-rw-r--r--   0        0        0       37 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/constants/__init__.py
+-rw-r--r--   0        0        0      328 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/constants/base.py
+-rw-r--r--   0        0        0       36 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/exceptions/__init__.py
+-rw-r--r--   0        0        0      967 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/exceptions/exception.py
+-rw-r--r--   0        0        0     1439 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/exceptions/handler.py
+-rw-r--r--   0        0        0        0 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/middlewares/__init__.py
+-rw-r--r--   0        0        0      670 2024-03-25 14:56:39.444948 microslac-0.0.9/src/micro/jango/middlewares/api.py
+-rw-r--r--   0        0        0     1097 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/middlewares/authentication.py
+-rw-r--r--   0        0        0      195 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/models/__init__.py
+-rw-r--r--   0        0        0      439 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/models/fields.py
+-rw-r--r--   0        0        0     1917 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/models/history.py
+-rw-r--r--   0        0        0      205 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/models/manager.py
+-rw-r--r--   0        0        0       79 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/models/queryset.py
+-rw-r--r--   0        0        0      195 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/models/uuid.py
+-rw-r--r--   0        0        0       33 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/permissions/__init__.py
+-rw-r--r--   0        0        0      330 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/permissions/internal.py
+-rw-r--r--   0        0        0       28 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/queues/__init__.py
+-rw-r--r--   0        0        0     3155 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/queues/base.py
+-rw-r--r--   0        0        0       35 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/renderers/__init__.py
+-rw-r--r--   0        0        0      997 2024-03-25 14:48:46.861216 microslac-0.0.9/src/micro/jango/renderers/json.py
+-rw-r--r--   0        0        0      103 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/serializers/__init__.py
+-rw-r--r--   0        0        0      993 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/serializers/base.py
+-rw-r--r--   0        0        0     1317 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/serializers/fields.py
+-rw-r--r--   0        0        0       30 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/services/__init__.py
+-rw-r--r--   0        0        0       59 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/services/base.py
+-rw-r--r--   0        0        0       44 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/tests/__init__.py
+-rw-r--r--   0        0        0     2094 2024-03-25 14:59:25.697212 microslac-0.0.9/src/micro/jango/tests/base.py
+-rw-r--r--   0        0        0      874 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/utils/__init__.py
+-rw-r--r--   0        0        0      273 2024-03-26 03:18:56.286484 microslac-0.0.9/src/micro/jango/utils/utils.py
+-rw-r--r--   0        0        0       62 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/views/__init__.py
+-rw-r--r--   0        0        0      621 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/jango/views/base.py
+-rw-r--r--   0        0        0        0 2024-03-21 16:45:59.737289 microslac-0.0.9/src/micro/patterns/__init__.py
+-rw-r--r--   0        0        0     1242 2024-03-06 17:42:01.785756 microslac-0.0.9/src/micro/patterns/null.py
+-rw-r--r--   0        0        0     2117 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/patterns/saga.py
+-rw-r--r--   0        0        0        0 2024-03-21 16:45:59.737289 microslac-0.0.9/src/micro/services/__init__.py
+-rw-r--r--   0        0        0     2712 2024-03-26 03:25:27.216568 microslac-0.0.9/src/micro/services/base.py
+-rw-r--r--   0        0        0      510 2024-03-25 14:01:51.479238 microslac-0.0.9/src/micro/services/registry.py
+-rw-r--r--   0        0        0        0 2024-03-21 16:45:59.737289 microslac-0.0.9/src/micro/utils/__init__.py
+-rw-r--r--   0        0        0     2785 2024-03-26 03:19:03.670468 microslac-0.0.9/src/micro/utils/utils.py
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 microslac-0.0.9/PKG-INFO
```

### Comparing `microslac-0.0.8/pyproject.toml` & `microslac-0.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 [tool.poetry]
 name = "microslac"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["tanlda <ledinhanhtan.stack@gmail.com>"]
 packages = [{ include = "micro", from = "src" }]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
 shortuuid = "^1.0.13"
-pytest = "^8.1.1"
-faker = "^24.3.0"
-pre-commit = "^3.6.2"
 pyjwt = "^2.8.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `microslac-0.0.8/src/micro/jango/exceptions/exception.py` & `microslac-0.0.9/src/micro/jango/exceptions/exception.py`

 * *Files identical despite different names*

### Comparing `microslac-0.0.8/src/micro/jango/exceptions/handler.py` & `microslac-0.0.9/src/micro/jango/exceptions/handler.py`

 * *Files identical despite different names*

### Comparing `microslac-0.0.8/src/micro/jango/middlewares/api.py` & `microslac-0.0.9/src/micro/jango/middlewares/api.py`

 * *Files identical despite different names*

### Comparing `microslac-0.0.8/src/micro/jango/middlewares/authentication.py` & `microslac-0.0.9/src/micro/jango/middlewares/authentication.py`

 * *Files identical despite different names*

### Comparing `microslac-0.0.8/src/micro/jango/models/history.py` & `microslac-0.0.9/src/micro/jango/models/history.py`

 * *Files identical despite different names*

### Comparing `microslac-0.0.8/src/micro/jango/queues/base.py` & `microslac-0.0.9/src/micro/jango/queues/base.py`

 * *Files identical despite different names*

### Comparing `microslac-0.0.8/src/micro/jango/renderers/json.py` & `microslac-0.0.9/src/micro/jango/renderers/json.py`

 * *Files identical despite different names*

### Comparing `microslac-0.0.8/src/micro/jango/serializers/base.py` & `microslac-0.0.9/src/micro/jango/serializers/base.py`

 * *Files identical despite different names*

### Comparing `microslac-0.0.8/src/micro/jango/serializers/fields.py` & `microslac-0.0.9/src/micro/jango/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `microslac-0.0.8/src/micro/jango/tests/base.py` & `microslac-0.0.9/src/micro/jango/tests/base.py`

 * *Files identical despite different names*

### Comparing `microslac-0.0.8/src/micro/jango/tests/conftest.py` & `microslac-0.0.9/src/micro/jango/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `microslac-0.0.8/src/micro/jango/views/base.py` & `microslac-0.0.9/src/micro/jango/views/base.py`

 * *Files identical despite different names*

### Comparing `microslac-0.0.8/src/micro/patterns/null.py` & `microslac-0.0.9/src/micro/patterns/null.py`

 * *Files identical despite different names*

### Comparing `microslac-0.0.8/src/micro/patterns/saga.py` & `microslac-0.0.9/src/micro/patterns/saga.py`

 * *Files identical despite different names*

### Comparing `microslac-0.0.8/src/micro/services/base.py` & `microslac-0.0.9/src/micro/services/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         data: dict,
         internal: bool = True,
         key: str = None,
         keys: list[str] = None,
         objectify: bool = False,
         raise_for_status: bool = True,
         **kwargs,
-    ) -> dict | SimpleNamespace:
+    ):
         data = data or {}
         url = cls.get_url(path)
         headers = kwargs.pop("headers", {})
         base_headers = cls.get_base_headers(internal=internal)
         response = requests.post(url=url, json=data, headers={**headers, **base_headers}, **kwargs)
         if raise_for_status:
             response.raise_for_status()
```

### Comparing `microslac-0.0.8/src/micro/utils/utils.py` & `microslac-0.0.9/src/micro/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from datetime import datetime
 from itertools import filterfalse, tee, zip_longest
 from operator import methodcaller
 from string import ascii_uppercase, digits
 from types import SimpleNamespace
 from typing import Any, Iterable, List, Literal
 
-from django.db.models import QuerySet
 from shortuuid import ShortUUID
 
 
 class unset:
     pass
 
 
@@ -27,21 +26,14 @@
             val = max(val, min_)
         if max_ is not None:
             val = min(val, max_)
         return int(val)
     return default
 
 
-def queryset_iterator(queryset: QuerySet, chunk_size: int = 1000):
-    total = queryset.count()
-    for start in range(0, total, chunk_size):
-        end = min(start + chunk_size, total)
-        yield queryset[start:end], start, end
-
-
 def extract(params: dict, *keys, default: any = unset, how: Literal["get", "pop"] = "get") -> tuple:
     assert how in ["get", "pop"], f"how must be one of ['get', 'pop'], got {how}."
 
     if default is not unset:
         if not isinstance(default, (list, tuple, set)):
             default = [default] * len(keys)
         pairs = zip_longest(keys, default, fillvalue=None)
```

### Comparing `microslac-0.0.8/PKG-INFO` & `microslac-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: microslac
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: tanlda
 Author-email: ledinhanhtan.stack@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: faker (>=24.3.0,<25.0.0)
-Requires-Dist: pre-commit (>=3.6.2,<4.0.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
-Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: shortuuid (>=1.0.13,<2.0.0)
 Description-Content-Type: text/markdown
```

