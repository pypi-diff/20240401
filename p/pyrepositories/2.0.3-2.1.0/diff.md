# Comparing `tmp/pyrepositories-2.0.3.tar.gz` & `tmp/pyrepositories-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepositories-2.0.3.tar", last modified: Sat Mar 23 14:08:50 2024, max compression
+gzip compressed data, was "pyrepositories-2.1.0.tar", last modified: Mon Apr  1 18:40:53 2024, max compression
```

## Comparing `pyrepositories-2.0.3.tar` & `pyrepositories-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:08:50.004476 pyrepositories-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-23 14:08:50.004476 pyrepositories-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-23 14:08:41.000000 pyrepositories-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-23 14:08:41.000000 pyrepositories-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 14:08:50.004476 pyrepositories-2.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:08:50.004476 pyrepositories-2.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:08:50.004476 pyrepositories-2.0.3/src/pyrepositories/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-23 14:08:41.000000 pyrepositories-2.0.3/src/pyrepositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-03-23 14:08:41.000000 pyrepositories-2.0.3/src/pyrepositories/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-23 14:08:41.000000 pyrepositories-2.0.3/src/pyrepositories/datatable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-03-23 14:08:41.000000 pyrepositories-2.0.3/src/pyrepositories/json_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-03-23 14:08:41.000000 pyrepositories-2.0.3/src/pyrepositories/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-23 14:08:41.000000 pyrepositories-2.0.3/src/pyrepositories/pg_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:08:50.004476 pyrepositories-2.0.3/src/pyrepositories.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-23 14:08:49.000000 pyrepositories-2.0.3/src/pyrepositories.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-23 14:08:50.000000 pyrepositories-2.0.3/src/pyrepositories.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 14:08:49.000000 pyrepositories-2.0.3/src/pyrepositories.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-23 14:08:49.000000 pyrepositories-2.0.3/src/pyrepositories.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-23 14:08:49.000000 pyrepositories-2.0.3/src/pyrepositories.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:40:53.105064 pyrepositories-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-01 18:40:53.105064 pyrepositories-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-01 18:40:48.000000 pyrepositories-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-01 18:40:48.000000 pyrepositories-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 18:40:53.105064 pyrepositories-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:40:53.101064 pyrepositories-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:40:53.105064 pyrepositories-2.1.0/src/pyrepositories/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-01 18:40:48.000000 pyrepositories-2.1.0/src/pyrepositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-01 18:40:48.000000 pyrepositories-2.1.0/src/pyrepositories/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-01 18:40:48.000000 pyrepositories-2.1.0/src/pyrepositories/datatable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-01 18:40:48.000000 pyrepositories-2.1.0/src/pyrepositories/json_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8878 2024-04-01 18:40:48.000000 pyrepositories-2.1.0/src/pyrepositories/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-01 18:40:48.000000 pyrepositories-2.1.0/src/pyrepositories/pg_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:40:53.105064 pyrepositories-2.1.0/src/pyrepositories.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-01 18:40:53.000000 pyrepositories-2.1.0/src/pyrepositories.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-01 18:40:53.000000 pyrepositories-2.1.0/src/pyrepositories.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:40:53.000000 pyrepositories-2.1.0/src/pyrepositories.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 18:40:53.000000 pyrepositories-2.1.0/src/pyrepositories.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 18:40:53.000000 pyrepositories-2.1.0/src/pyrepositories.egg-info/top_level.txt
```

### Comparing `pyrepositories-2.0.3/PKG-INFO` & `pyrepositories-2.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepositories
-Version: 2.0.3
+Version: 2.1.0
 Summary: A simple way to interact with a database using the SOLID principles' Repository pattern.
 Author-email: kougen <info@kou-gen.net>
 Maintainer-email: Joshua Hegedus <josh.hegedus@outlook.com>
 Project-URL: Homepage, https://github.com/kougen/py-repositories
 Project-URL: Issues, https://github.com/kougen/py-repositories/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepositories-2.0.3/pyproject.toml` & `pyrepositories-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyrepositories"
-version = "2.0.3"
+version = "2.1.0"
 authors = [
   { name="kougen", email="info@kou-gen.net" },
 ]
 
 maintainers = [
   { name="Joshua Hegedus", email="josh.hegedus@outlook.com" },
 ]
```

### Comparing `pyrepositories-2.0.3/src/pyrepositories/datasource.py` & `pyrepositories-2.1.0/src/pyrepositories/datasource.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .datatable import DataTable
-from .lib import Entity, IdTypes
+from .lib import Entity, IdTypes, Filter
 import random
 import string
 from uuid import uuid4 as get_uuid
 
 
 def get_random_string_id():
     return ''.join(random.choices(string.ascii_letters + string.digits, k=16))
@@ -62,21 +62,38 @@
     def get_by_id(self, table_name: str, id: int | str):
         table = self.get_table(table_name)
         if table:
             return table.get_by_id(id)
         else:
             return None
 
-    def get_by_filter(self, table_name: str, filter: dict):
+    def get_by_filter(self, table_name: str, filter: Filter):
         table = self.get_table(table_name)
         if table:
             return table.get_by_filter(filter)
         else:
             raise ValueError("Table not found")
 
+    def get_by_filters(self, table_name: str, filters: list[Filter]):
+        table = self.get_table(table_name)
+        if table:
+            entities = []
+            for filter in filters:
+                entities.extend(table.get_by_filter(filter))
+            return entities
+        else:
+            raise ValueError("Table not found")
+
+    def get_unique(self, table_name: str, field_name: str, value: any):
+        table = self.get_table(table_name)
+        if table:
+            return table.get_unique(field_name, value)
+        else:
+            return None
+
     def insert(self, table_name: str, data: Entity):
         table = self.get_table(table_name)
         if not table:
             raise ValueError("Table not found")
 
         if self.auto_increment:
             data.id = get_id(self.id_type, table.get_all())
```

### Comparing `pyrepositories-2.0.3/src/pyrepositories/json_repository.py` & `pyrepositories-2.1.0/src/pyrepositories/json_repository.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,102 @@
+from typing import Any
 from .datatable import DataTable
 from jsonservice import JsonService
-from .datasource import DataSource
-from .lib import Entity, filter_by_fields
+from .lib import Entity, IdTypes, EntityField, FieldBase, Filter
 import os
 
-def convert_to_entity(data: dict) -> Entity:
+
+def convert_to_entity(data: dict, fields: list[FieldBase]) -> Entity | None:
     if 'id' not in data:
         raise ValueError("Entity must have an id")
 
-    entity = Entity(data['id'])
-    for key, value in data.items():
-        if key != 'id':
-            entity.add_field(key, value)
-    return entity
+    fields_dict = {field.name: field for field in fields}
+    entity_fields = []
+    for key, field in fields_dict.items():
+        entity_fields.append(EntityField(field, data.get(key)))
+    entity = Entity(entity_fields, data['id'])
+    if entity.validate():
+        return entity
+
+    entity.print_errors()
+    return None
+
 
 class JsonTable(DataTable):
-    def __init__(self, name: str, store_path: str):
-        super().__init__(name)
+    def __init__(self, name: str, store_path: str, fields: list[FieldBase], create_if_not_exists: bool = True):
+        super().__init__(name, fields)
         file_path = os.path.join(store_path, f'{name}.json')
-        self.json_service = JsonService(file_path)
+        self.json_service = JsonService(file_path, create_if_not_exists=create_if_not_exists)
         current_content = self.json_service.read('content')
 
         if not current_content:
             self.json_service.write('content', [])
+            current_content = []
+
+        self._refresh_fields()
 
     def get_all(self):
         content = self.json_service.read('content') or []
         entities = []
         for item in content:
-            entities.append(convert_to_entity(item))
+            entities.append(convert_to_entity(item, self.field_structure))
+
         return entities
 
-    def get_by_id(self, id):
+    def get_by_id(self, entity_id: int | str) -> Entity | None:
         content = self.json_service.read('content') or []
         for item in content:
-            if item['id'] == id:
-                return item
+            if item['id'] == entity_id:
+                return convert_to_entity(item, self.field_structure)
         return None
 
-    def insert(self, data: Entity):
+    def get_unique(self, key: str, value: Any) -> Entity | None:
+        field_value = self._get_unique(key, value)
+        if not field_value:
+            return None
+
+        entity = self.get_by_id(field_value.entity_id)
+        if not entity:
+            return None
+        return entity
+
+    def insert(self, data: Entity) -> Entity | None:
+        result = super().insert(data)
+        if not result:
+            return None
         content = self.json_service.read('content') or []
-        content.append(data.serialize())
+        content.append(result.serialize())
         self.json_service.write('content', content)
-        return True
+        return result
 
-    def update(self, id, data: Entity):
+    def insert_many(self, data: list[Entity]) -> list[Entity] | None:
+        results = []
+        for entity in data:
+            result = self.insert(entity)
+            if not result:
+                return None
+            results.append(result)
+        return results
+
+    def update(self, entity_id, data: Entity) -> Entity | None:
+        result = super().update(entity_id, data)
+        if not result:
+            return None
         content = self.json_service.read('content') or []  # type: list[dict]
         for index, item in enumerate(content):
-            if item['id'] == id:
-                content[index] = data.serialize()
+            if item['id'] == entity_id:
+                content[index] = result.serialize()
                 self.json_service.write('content', content)
-                return True
-        return False
+                return result
+        return None
 
-    def delete(self, id):
+    def delete(self, entity_id: IdTypes) -> bool:
         content = self.json_service.read('content') or []
         for index, item in enumerate(content):
-            if item['id'] == id:
+            if item['id'] == entity_id:
                 del content[index]
                 self.json_service.write('content', content)
                 return True
         return False
 
     def clear(self):
         self.json_service.write('content', [])
```

### Comparing `pyrepositories-2.0.3/src/pyrepositories.egg-info/PKG-INFO` & `pyrepositories-2.1.0/src/pyrepositories.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepositories
-Version: 2.0.3
+Version: 2.1.0
 Summary: A simple way to interact with a database using the SOLID principles' Repository pattern.
 Author-email: kougen <info@kou-gen.net>
 Maintainer-email: Joshua Hegedus <josh.hegedus@outlook.com>
 Project-URL: Homepage, https://github.com/kougen/py-repositories
 Project-URL: Issues, https://github.com/kougen/py-repositories/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

