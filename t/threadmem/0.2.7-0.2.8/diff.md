# Comparing `tmp/threadmem-0.2.7.tar.gz` & `tmp/threadmem-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threadmem-0.2.7.tar", max compression
+gzip compressed data, was "threadmem-0.2.8.tar", max compression
```

## Comparing `threadmem-0.2.7.tar` & `threadmem-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1069 2024-03-20 16:37:21.259969 threadmem-0.2.7/LICENSE
--rw-r--r--   0        0        0     1535 2024-04-01 02:28:59.834280 threadmem-0.2.7/README.md
--rw-r--r--   0        0        0      750 2024-04-01 04:30:24.350399 threadmem-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      202 2024-04-01 02:41:59.362656 threadmem-0.2.7/threadmem/__init__.py
--rw-r--r--   0        0        0       23 2024-03-26 21:35:27.218837 threadmem-0.2.7/threadmem/auth/default.py
--rw-r--r--   0        0        0     2661 2024-03-31 17:51:41.938971 threadmem-0.2.7/threadmem/auth/key.py
--rw-r--r--   0        0        0     3930 2024-03-31 17:51:41.939305 threadmem-0.2.7/threadmem/auth/provider.py
--rw-r--r--   0        0        0      735 2024-03-26 21:36:15.906190 threadmem-0.2.7/threadmem/auth/transport.py
--rw-r--r--   0        0        0     2204 2024-03-26 21:36:24.545356 threadmem-0.2.7/threadmem/auth/user.py
--rw-r--r--   0        0        0     1862 2024-03-20 16:37:21.260985 threadmem-0.2.7/threadmem/db/conn.py
--rw-r--r--   0        0        0     1947 2024-04-01 01:50:49.121883 threadmem-0.2.7/threadmem/db/models.py
--rw-r--r--   0        0        0       41 2024-03-26 21:54:29.100650 threadmem-0.2.7/threadmem/env.py
--rw-r--r--   0        0        0    29468 2024-04-01 04:30:11.914351 threadmem-0.2.7/threadmem/role.py
--rw-r--r--   0        0        0     1178 2024-03-26 22:46:58.504986 threadmem-0.2.7/threadmem/server/app.py
--rw-r--r--   0        0        0     1510 2024-04-01 01:56:13.889604 threadmem-0.2.7/threadmem/server/models.py
--rw-r--r--   0        0        0     4391 2024-03-31 17:51:41.948190 threadmem-0.2.7/threadmem/server/routes.py
--rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 threadmem-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-20 16:37:21.259969 threadmem-0.2.8/LICENSE
+-rw-r--r--   0        0        0     1535 2024-04-01 02:28:59.834280 threadmem-0.2.8/README.md
+-rw-r--r--   0        0        0      750 2024-04-01 15:10:30.138340 threadmem-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      202 2024-04-01 02:41:59.362656 threadmem-0.2.8/threadmem/__init__.py
+-rw-r--r--   0        0        0       23 2024-03-26 21:35:27.218837 threadmem-0.2.8/threadmem/auth/default.py
+-rw-r--r--   0        0        0     2661 2024-03-31 17:51:41.938971 threadmem-0.2.8/threadmem/auth/key.py
+-rw-r--r--   0        0        0     3930 2024-03-31 17:51:41.939305 threadmem-0.2.8/threadmem/auth/provider.py
+-rw-r--r--   0        0        0      735 2024-03-26 21:36:15.906190 threadmem-0.2.8/threadmem/auth/transport.py
+-rw-r--r--   0        0        0     2204 2024-03-26 21:36:24.545356 threadmem-0.2.8/threadmem/auth/user.py
+-rw-r--r--   0        0        0     1862 2024-03-20 16:37:21.260985 threadmem-0.2.8/threadmem/db/conn.py
+-rw-r--r--   0        0        0     1947 2024-04-01 01:50:49.121883 threadmem-0.2.8/threadmem/db/models.py
+-rw-r--r--   0        0        0       41 2024-03-26 21:54:29.100650 threadmem-0.2.8/threadmem/env.py
+-rw-r--r--   0        0        0    29766 2024-04-01 15:10:03.303133 threadmem-0.2.8/threadmem/role.py
+-rw-r--r--   0        0        0     1178 2024-03-26 22:46:58.504986 threadmem-0.2.8/threadmem/server/app.py
+-rw-r--r--   0        0        0     1510 2024-04-01 01:56:13.889604 threadmem-0.2.8/threadmem/server/models.py
+-rw-r--r--   0        0        0     4391 2024-03-31 17:51:41.948190 threadmem-0.2.8/threadmem/server/routes.py
+-rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 threadmem-0.2.8/PKG-INFO
```

### Comparing `threadmem-0.2.7/LICENSE` & `threadmem-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.7/README.md` & `threadmem-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.7/pyproject.toml` & `threadmem-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "threadmem"
-version = "0.2.7"
+version = "0.2.8"
 description = "Thread memory for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "threadmem"}]
 
 [tool.poetry.dependencies]
```

### Comparing `threadmem-0.2.7/threadmem/auth/key.py` & `threadmem-0.2.8/threadmem/auth/key.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.7/threadmem/auth/provider.py` & `threadmem-0.2.8/threadmem/auth/provider.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.7/threadmem/auth/transport.py` & `threadmem-0.2.8/threadmem/auth/transport.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.7/threadmem/auth/user.py` & `threadmem-0.2.8/threadmem/auth/user.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.7/threadmem/db/conn.py` & `threadmem-0.2.8/threadmem/db/conn.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.7/threadmem/db/models.py` & `threadmem-0.2.8/threadmem/db/models.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.7/threadmem/role.py` & `threadmem-0.2.8/threadmem/role.py`

 * *Files 2% similar despite different names*

```diff
@@ -406,14 +406,19 @@
         """
         Converts the RoleThread instance into a RoleThreadRecord for database storage.
 
         Returns:
             RoleThreadRecord: An instance of RoleThreadRecord with fields populated from the RoleThread instance.
         """
         metadata = json.dumps(self._metadata) if self._metadata else None
+        role_mapping = {}
+        if self._role_mapping:
+            for _, role in self._role_mapping.items():
+                role_mapping[role.name] = role.model_dump()
+
         role_mapping = json.dumps(self._role_mapping) if self._role_mapping else None
         return RoleThreadRecord(
             id=self._id,
             owner_id=self._owner_id,
             public=self._public,
             messages=[message.to_record() for message in self._messages],
             name=self._name,
@@ -433,17 +438,21 @@
         Args:
             record (RoleThreadRecord): The database record to convert into a RoleThread instance.
 
         Returns:
             RoleThread: An instance of RoleThread with properties populated from the database record.
         """
         metadata_dict = json.loads(record.meta_data) if record.meta_data else None
-        role_mapping_dict = (
-            json.loads(record.role_mapping) if record.role_mapping else None
-        )
+
+        role_mapping_dict = {}
+        if record.role_mapping:
+            jdict = json.loads(record.role_mapping)
+            for role_name, role_dict in jdict.items():
+                role_mapping_dict[role_name] = RoleModel(**role_dict)
+
         obj = cls.__new__(cls)
         obj._id = record.id
         obj._owner_id = record.owner_id
         obj._public = record.public
         obj._name = record.name
         obj._metadata = metadata_dict
         obj._created = record.created
```

### Comparing `threadmem-0.2.7/threadmem/server/app.py` & `threadmem-0.2.8/threadmem/server/app.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.7/threadmem/server/models.py` & `threadmem-0.2.8/threadmem/server/models.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.7/threadmem/server/routes.py` & `threadmem-0.2.8/threadmem/server/routes.py`

 * *Files identical despite different names*

### Comparing `threadmem-0.2.7/PKG-INFO` & `threadmem-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threadmem
-Version: 0.2.7
+Version: 0.2.8
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
-Metadata-Version: 2.1 Name: threadmem Version: 0.2.7 Summary: Thread memory for
+Metadata-Version: 2.1 Name: threadmem Version: 0.2.8 Summary: Thread memory for
 AI agents License: Apache 2.0 Author: Patrick Barker Author-email:
 patrickbarkerco@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: fastapi[all] (>=0.109,<0.110)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0) Requires-Dist: requests
 (>=2.31.0,<3.0.0) Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0) Description-
```

