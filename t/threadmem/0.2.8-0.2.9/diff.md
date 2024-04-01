# Comparing `tmp/threadmem-0.2.8.tar.gz` & `tmp/threadmem-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threadmem-0.2.8.tar", max compression
+gzip compressed data, was "threadmem-0.2.9.tar", max compression
```

## Comparing `threadmem-0.2.8.tar` & `threadmem-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1069 2024-03-20 16:37:21.259969 threadmem-0.2.8/LICENSE
--rw-r--r--   0        0        0     1535 2024-04-01 02:28:59.834280 threadmem-0.2.8/README.md
--rw-r--r--   0        0        0      750 2024-04-01 15:10:30.138340 threadmem-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      202 2024-04-01 02:41:59.362656 threadmem-0.2.8/threadmem/__init__.py
--rw-r--r--   0        0        0       23 2024-03-26 21:35:27.218837 threadmem-0.2.8/threadmem/auth/default.py
--rw-r--r--   0        0        0     2661 2024-03-31 17:51:41.938971 threadmem-0.2.8/threadmem/auth/key.py
--rw-r--r--   0        0        0     3930 2024-03-31 17:51:41.939305 threadmem-0.2.8/threadmem/auth/provider.py
--rw-r--r--   0        0        0      735 2024-03-26 21:36:15.906190 threadmem-0.2.8/threadmem/auth/transport.py
--rw-r--r--   0        0        0     2204 2024-03-26 21:36:24.545356 threadmem-0.2.8/threadmem/auth/user.py
--rw-r--r--   0        0        0     1862 2024-03-20 16:37:21.260985 threadmem-0.2.8/threadmem/db/conn.py
--rw-r--r--   0        0        0     1947 2024-04-01 01:50:49.121883 threadmem-0.2.8/threadmem/db/models.py
--rw-r--r--   0        0        0       41 2024-03-26 21:54:29.100650 threadmem-0.2.8/threadmem/env.py
--rw-r--r--   0        0        0    29766 2024-04-01 15:10:03.303133 threadmem-0.2.8/threadmem/role.py
--rw-r--r--   0        0        0     1178 2024-03-26 22:46:58.504986 threadmem-0.2.8/threadmem/server/app.py
--rw-r--r--   0        0        0     1510 2024-04-01 01:56:13.889604 threadmem-0.2.8/threadmem/server/models.py
--rw-r--r--   0        0        0     4391 2024-03-31 17:51:41.948190 threadmem-0.2.8/threadmem/server/routes.py
--rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 threadmem-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-20 16:37:21.259969 threadmem-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1535 2024-04-01 02:28:59.834280 threadmem-0.2.9/README.md
+-rw-r--r--   0        0        0      750 2024-04-01 15:51:00.916516 threadmem-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      202 2024-04-01 02:41:59.362656 threadmem-0.2.9/threadmem/__init__.py
+-rw-r--r--   0        0        0       23 2024-03-26 21:35:27.218837 threadmem-0.2.9/threadmem/auth/default.py
+-rw-r--r--   0        0        0     2661 2024-03-31 17:51:41.938971 threadmem-0.2.9/threadmem/auth/key.py
+-rw-r--r--   0        0        0     3930 2024-03-31 17:51:41.939305 threadmem-0.2.9/threadmem/auth/provider.py
+-rw-r--r--   0        0        0      735 2024-03-26 21:36:15.906190 threadmem-0.2.9/threadmem/auth/transport.py
+-rw-r--r--   0        0        0     2204 2024-03-26 21:36:24.545356 threadmem-0.2.9/threadmem/auth/user.py
+-rw-r--r--   0        0        0     1862 2024-03-20 16:37:21.260985 threadmem-0.2.9/threadmem/db/conn.py
+-rw-r--r--   0        0        0     1947 2024-04-01 01:50:49.121883 threadmem-0.2.9/threadmem/db/models.py
+-rw-r--r--   0        0        0       41 2024-03-26 21:54:29.100650 threadmem-0.2.9/threadmem/env.py
+-rw-r--r--   0        0        0    29680 2024-04-01 15:50:55.111422 threadmem-0.2.9/threadmem/role.py
+-rw-r--r--   0        0        0     1178 2024-03-26 22:46:58.504986 threadmem-0.2.9/threadmem/server/app.py
+-rw-r--r--   0        0        0     1510 2024-04-01 01:56:13.889604 threadmem-0.2.9/threadmem/server/models.py
+-rw-r--r--   0        0        0     4391 2024-03-31 17:51:41.948190 threadmem-0.2.9/threadmem/server/routes.py
+-rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 threadmem-0.2.9/PKG-INFO
```

### Comparing `threadmem-0.2.8/LICENSE` & `threadmem-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.8/README.md` & `threadmem-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.8/pyproject.toml` & `threadmem-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "threadmem"
-version = "0.2.8"
+version = "0.2.9"
 description = "Thread memory for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "threadmem"}]
 
 [tool.poetry.dependencies]
```

### Comparing `threadmem-0.2.8/threadmem/auth/key.py` & `threadmem-0.2.9/threadmem/auth/key.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.8/threadmem/auth/provider.py` & `threadmem-0.2.9/threadmem/auth/provider.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.8/threadmem/auth/transport.py` & `threadmem-0.2.9/threadmem/auth/transport.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.8/threadmem/auth/user.py` & `threadmem-0.2.9/threadmem/auth/user.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.8/threadmem/db/conn.py` & `threadmem-0.2.9/threadmem/db/conn.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.8/threadmem/db/models.py` & `threadmem-0.2.9/threadmem/db/models.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.8/threadmem/role.py` & `threadmem-0.2.9/threadmem/role.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,15 +411,14 @@
         """
         metadata = json.dumps(self._metadata) if self._metadata else None
         role_mapping = {}
         if self._role_mapping:
             for _, role in self._role_mapping.items():
                 role_mapping[role.name] = role.model_dump()
 
-        role_mapping = json.dumps(self._role_mapping) if self._role_mapping else None
         return RoleThreadRecord(
             id=self._id,
             owner_id=self._owner_id,
             public=self._public,
             messages=[message.to_record() for message in self._messages],
             name=self._name,
             meta_data=metadata,
```

### Comparing `threadmem-0.2.8/threadmem/server/app.py` & `threadmem-0.2.9/threadmem/server/app.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.8/threadmem/server/models.py` & `threadmem-0.2.9/threadmem/server/models.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.8/threadmem/server/routes.py` & `threadmem-0.2.9/threadmem/server/routes.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.8/PKG-INFO` & `threadmem-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threadmem
-Version: 0.2.8
+Version: 0.2.9
 Summary: Thread memory for AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: threadmem Version: 0.2.8 Summary: Thread memory for
+Metadata-Version: 2.1 Name: threadmem Version: 0.2.9 Summary: Thread memory for
 AI agents License: Apache 2.0 Author: Patrick Barker Author-email:
 patrickbarkerco@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: fastapi[all] (>=0.109,<0.110)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0) Requires-Dist: requests
 (>=2.31.0,<3.0.0) Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0) Description-
```

