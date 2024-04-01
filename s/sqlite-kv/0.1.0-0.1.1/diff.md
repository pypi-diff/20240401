# Comparing `tmp/sqlite-kv-0.1.0.tar.gz` & `tmp/sqlite-kv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite-kv-0.1.0.tar", last modified: Mon Apr  1 16:38:02 2024, max compression
+gzip compressed data, was "sqlite-kv-0.1.1.tar", last modified: Mon Apr  1 16:46:22 2024, max compression
```

## Comparing `sqlite-kv-0.1.0.tar` & `sqlite-kv-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-01 16:38:02.734712 sqlite-kv-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      367 2024-04-01 16:38:02.734712 sqlite-kv-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      100 2024-04-01 16:25:38.000000 sqlite-kv-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      555 2024-04-01 16:25:38.000000 sqlite-kv-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-01 16:38:02.734712 sqlite-kv-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-01 16:38:02.724712 sqlite-kv-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-01 16:38:02.724712 sqlite-kv-0.1.0/src/sqlite_kv/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      146 2024-04-01 16:34:06.000000 sqlite-kv-0.1.0/src/sqlite_kv/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-01 16:38:02.734712 sqlite-kv-0.1.0/src/sqlite_kv/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-04-01 16:33:56.000000 sqlite-kv-0.1.0/src/sqlite_kv/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1935 2024-04-01 16:33:29.000000 sqlite-kv-0.1.0/src/sqlite_kv/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-01 16:38:02.734712 sqlite-kv-0.1.0/src/sqlite_kv/decorators/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       82 2024-04-01 16:28:31.000000 sqlite-kv-0.1.0/src/sqlite_kv/decorators/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1659 2024-04-01 16:27:58.000000 sqlite-kv-0.1.0/src/sqlite_kv/decorators/decorators.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-01 16:38:02.734712 sqlite-kv-0.1.0/src/sqlite_kv/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-04-01 15:29:18.000000 sqlite-kv-0.1.0/src/sqlite_kv/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1829 2024-04-01 15:29:12.000000 sqlite-kv-0.1.0/src/sqlite_kv/ops/ops.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-01 16:38:02.734712 sqlite-kv-0.1.0/src/sqlite_kv.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      367 2024-04-01 16:38:02.000000 sqlite-kv-0.1.0/src/sqlite_kv.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      384 2024-04-01 16:38:02.000000 sqlite-kv-0.1.0/src/sqlite_kv.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-01 16:38:02.000000 sqlite-kv-0.1.0/src/sqlite_kv.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       10 2024-04-01 16:38:02.000000 sqlite-kv-0.1.0/src/sqlite_kv.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-01 16:46:22.194710 sqlite-kv-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1234 2024-04-01 16:46:22.194710 sqlite-kv-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      967 2024-04-01 16:45:33.000000 sqlite-kv-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      555 2024-04-01 16:39:08.000000 sqlite-kv-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-01 16:46:22.194710 sqlite-kv-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-01 16:46:22.184710 sqlite-kv-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-01 16:46:22.184710 sqlite-kv-0.1.1/src/sqlite_kv/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      146 2024-04-01 16:34:06.000000 sqlite-kv-0.1.1/src/sqlite_kv/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-01 16:46:22.194710 sqlite-kv-0.1.1/src/sqlite_kv/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-04-01 16:33:56.000000 sqlite-kv-0.1.1/src/sqlite_kv/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1920 2024-04-01 16:45:47.000000 sqlite-kv-0.1.1/src/sqlite_kv/api/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-01 16:46:22.194710 sqlite-kv-0.1.1/src/sqlite_kv/decorators/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       82 2024-04-01 16:28:31.000000 sqlite-kv-0.1.1/src/sqlite_kv/decorators/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1659 2024-04-01 16:27:58.000000 sqlite-kv-0.1.1/src/sqlite_kv/decorators/decorators.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-01 16:46:22.194710 sqlite-kv-0.1.1/src/sqlite_kv/ops/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-04-01 15:29:18.000000 sqlite-kv-0.1.1/src/sqlite_kv/ops/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1829 2024-04-01 15:29:12.000000 sqlite-kv-0.1.1/src/sqlite_kv/ops/ops.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-01 16:46:22.194710 sqlite-kv-0.1.1/src/sqlite_kv.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1234 2024-04-01 16:46:22.000000 sqlite-kv-0.1.1/src/sqlite_kv.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      384 2024-04-01 16:46:22.000000 sqlite-kv-0.1.1/src/sqlite_kv.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-01 16:46:22.000000 sqlite-kv-0.1.1/src/sqlite_kv.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       10 2024-04-01 16:46:22.000000 sqlite-kv-0.1.1/src/sqlite_kv.egg-info/top_level.txt
```

### Comparing `sqlite-kv-0.1.0/pyproject.toml` & `sqlite-kv-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqlite-kv"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Async Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB"
 dependencies = [
   
 ]
```

### Comparing `sqlite-kv-0.1.0/src/sqlite_kv/api/api.py` & `sqlite-kv-0.1.1/src/sqlite_kv/api/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 @dataclass
 class SQLiteKV(Generic[T]):
 
   db_path: str = 'db.sqlite'
   table: str = 'kv'
   parse: Callable[[str], T] = lambda x: x
-  stringify: Callable[[T], str] = lambda x: x
+  dump: Callable[[T], str] = lambda x: x
   dtype: str = 'TEXT'
 
   @classmethod
   async def new(cls, *args, **kw) -> 'SQLiteKV':
     obj = cls(*args, **kw)
     await obj.create()
     return obj
   
   @classmethod
   async def documents(cls, db_path: str = 'db.sqlite', table: str = 'documents') -> 'SQLiteKV[dict]':
     """Create a JSON documents key-value DB"""
-    return await SQLiteKV.new(db_path=db_path, table=table, parse=json.loads, stringify=json.dumps, dtype='JSON')
+    return await SQLiteKV.new(db_path=db_path, table=table, parse=json.loads, dump=json.dumps, dtype='JSON')
   
   @classmethod
   async def blobs(cls, db_path: str = 'db.sqlite', table: str = 'blobs') -> 'SQLiteKV[dict]':
     """Create a BLOB key-value DB"""
     return await SQLiteKV.new(db_path=db_path, table=table, dtype='BLOB')
 
 
@@ -39,15 +39,15 @@
     return with_args_gen(self.db_path, self.table)(f)
 
   async def create(self, **kw):
     """Create the DB (if it didn't exist). Automatically called by factory static methods"""
     return await self._wrap(create)(dtype=self.dtype, **kw)
 
   async def upsert(self, key: str, value: T, **kw):
-    return await self._wrap(upsert)(key, self.stringify(value), **kw)
+    return await self._wrap(upsert)(key, self.dump(value), **kw)
 
   async def read(self, key: str, **kw) -> T | None:
     r = await self._wrap(read)(key, **kw)
     return r and self.parse(r)
 
   async def readall(self, batch_size: int = 256, **kw) -> AsyncIterable[tuple[str, T]]:
     async for k, v in self._wrap_gen(readall)(batch_size=batch_size, **kw):
```

### Comparing `sqlite-kv-0.1.0/src/sqlite_kv/decorators/decorators.py` & `sqlite-kv-0.1.1/src/sqlite_kv/decorators/decorators.py`

 * *Files identical despite different names*

### Comparing `sqlite-kv-0.1.0/src/sqlite_kv/ops/ops.py` & `sqlite-kv-0.1.1/src/sqlite_kv/ops/ops.py`

 * *Files identical despite different names*

