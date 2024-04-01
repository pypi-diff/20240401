# Comparing `tmp/async_sqlmodel-0.1.2.tar.gz` & `tmp/async_sqlmodel-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_sqlmodel-0.1.2.tar", max compression
+gzip compressed data, was "async_sqlmodel-0.1.3.tar", max compression
```

## Comparing `async_sqlmodel-0.1.2.tar` & `async_sqlmodel-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2024-03-31 08:47:39.366749 async_sqlmodel-0.1.2/LICENSE
--rw-r--r--   0        0        0     3187 2024-03-31 08:47:39.366749 async_sqlmodel-0.1.2/README.md
--rw-r--r--   0        0        0      100 2024-03-31 08:47:39.366749 async_sqlmodel-0.1.2/async_sqlmodel/__init__.py
--rw-r--r--   0        0        0     2351 2024-03-31 08:47:39.366749 async_sqlmodel-0.1.2/async_sqlmodel/main.py
--rw-r--r--   0        0        0        0 2024-03-31 08:47:39.366749 async_sqlmodel-0.1.2/async_sqlmodel/py.typed
--rw-r--r--   0        0        0      433 2024-03-31 08:47:39.370749 async_sqlmodel-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3801 1970-01-01 00:00:00.000000 async_sqlmodel-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-01 19:07:01.257285 async_sqlmodel-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3160 2024-04-01 19:07:01.257285 async_sqlmodel-0.1.3/README.md
+-rw-r--r--   0        0        0      100 2024-04-01 19:07:01.257285 async_sqlmodel-0.1.3/async_sqlmodel/__init__.py
+-rw-r--r--   0        0        0     2315 2024-04-01 19:07:01.257285 async_sqlmodel-0.1.3/async_sqlmodel/main.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:07:01.257285 async_sqlmodel-0.1.3/async_sqlmodel/py.typed
+-rw-r--r--   0        0        0      431 2024-04-01 19:07:01.257285 async_sqlmodel-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3824 1970-01-01 00:00:00.000000 async_sqlmodel-0.1.3/PKG-INFO
```

### Comparing `async_sqlmodel-0.1.2/LICENSE` & `async_sqlmodel-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `async_sqlmodel-0.1.2/README.md` & `async_sqlmodel-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,15 @@
 ```
 
 ### Add an AwaitableField
 
 Adding an **AwaitableField** yields an awaitable field for the `field` specified in the argument.
 
 ```python
-from typing import Optional
-from collections.abc import Awaitable
+from typing import Optional, Awaitable
 
 from sqlmodel import Field
 from async_sqlmodel import AsyncSQLModel, AwaitableField
 
 
 class Hero(AsyncSQLModel, table=True):
     id: Optional[int] = Field(default=None, primary_key=True)
```

### Comparing `async_sqlmodel-0.1.2/async_sqlmodel/main.py` & `async_sqlmodel-0.1.3/async_sqlmodel/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Any, ClassVar, Coroutine, Dict, Tuple, Type
 
-from pydantic._internal._repr import Representation
 from sqlalchemy.util.concurrency import greenlet_spawn
 from sqlmodel import SQLModel
-from sqlmodel._compat import get_annotations
+from sqlmodel._compat import Representation, get_annotations
 from sqlmodel.main import SQLModelMetaclass
 
 
 class AwaitableFieldInfo(Representation):
     def __init__(self, *, field: str):
         self.field = field
```

### Comparing `async_sqlmodel-0.1.2/PKG-INFO` & `async_sqlmodel-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: async-sqlmodel
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: 2jun0
 Author-email: soo28819@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: greenlet (>=3.0.3,<4.0.0)
 Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
@@ -49,16 +50,15 @@
 ```
 
 ### Add an AwaitableField
 
 Adding an **AwaitableField** yields an awaitable field for the `field` specified in the argument.
 
 ```python
-from typing import Optional
-from collections.abc import Awaitable
+from typing import Optional, Awaitable
 
 from sqlmodel import Field
 from async_sqlmodel import AsyncSQLModel, AwaitableField
 
 
 class Hero(AsyncSQLModel, table=True):
     id: Optional[int] = Field(default=None, primary_key=True)
```

