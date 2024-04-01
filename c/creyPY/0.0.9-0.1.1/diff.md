# Comparing `tmp/creyPY-0.0.9.tar.gz` & `tmp/creyPY-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creyPY-0.0.9.tar", last modified: Mon Apr  1 16:40:11 2024, max compression
+gzip compressed data, was "creyPY-0.1.1.tar", last modified: Mon Apr  1 18:48:07 2024, max compression
```

## Comparing `creyPY-0.0.9.tar` & `creyPY-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:40:11.348280 creyPY-0.0.9/
--rw-r--r--   0 conrad     (501) staff       (20)     1063 2024-04-01 15:11:19.000000 creyPY-0.0.9/LICENSE
--rw-r--r--   0 conrad     (501) staff       (20)      266 2024-04-01 16:40:11.348042 creyPY-0.0.9/PKG-INFO
--rw-r--r--   0 conrad     (501) staff       (20)      181 2024-04-01 16:11:11.000000 creyPY-0.0.9/README.md
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:40:11.344419 creyPY-0.0.9/creyPY/
--rw-r--r--   0 conrad     (501) staff       (20)        0 2024-04-01 15:50:43.000000 creyPY-0.0.9/creyPY/__init__.py
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:40:11.345605 creyPY-0.0.9/creyPY/const/
--rw-r--r--   0 conrad     (501) staff       (20)       88 2024-04-01 16:15:06.000000 creyPY-0.0.9/creyPY/const/__init__.py
--rw-r--r--   0 conrad     (501) staff       (20)      146 2024-04-01 16:01:50.000000 creyPY-0.0.9/creyPY/const/groups.py
--rw-r--r--   0 conrad     (501) staff       (20)     9324 2024-04-01 15:51:19.000000 creyPY-0.0.9/creyPY/const/i18n.py
--rw-r--r--   0 conrad     (501) staff       (20)     4373 2024-04-01 15:51:31.000000 creyPY-0.0.9/creyPY/const/stripe.py
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:40:11.346662 creyPY-0.0.9/creyPY/fastapi/
--rw-r--r--   0 conrad     (501) staff       (20)      150 2024-04-01 16:38:37.000000 creyPY-0.0.9/creyPY/fastapi/__init__.py
--rw-r--r--   0 conrad     (501) staff       (20)      848 2024-04-01 16:25:30.000000 creyPY-0.0.9/creyPY/fastapi/app.py
--rw-r--r--   0 conrad     (501) staff       (20)     1647 2024-04-01 16:29:15.000000 creyPY-0.0.9/creyPY/fastapi/crud.py
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:40:11.347029 creyPY-0.0.9/creyPY/fastapi/models/
--rw-r--r--   0 conrad     (501) staff       (20)       28 2024-04-01 16:28:08.000000 creyPY-0.0.9/creyPY/fastapi/models/__init__.py
--rw-r--r--   0 conrad     (501) staff       (20)      771 2024-04-01 16:28:31.000000 creyPY-0.0.9/creyPY/fastapi/models/base.py
--rw-r--r--   0 conrad     (501) staff       (20)     1886 2024-04-01 16:10:27.000000 creyPY-0.0.9/creyPY/fastapi/pagination.py
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:40:11.347470 creyPY-0.0.9/creyPY/fastapi/schemas/
--rw-r--r--   0 conrad     (501) staff       (20)       28 2024-04-01 16:38:22.000000 creyPY-0.0.9/creyPY/fastapi/schemas/__init__.py
--rw-r--r--   0 conrad     (501) staff       (20)      319 2024-04-01 16:38:47.000000 creyPY-0.0.9/creyPY/fastapi/schemas/base.py
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:40:11.347795 creyPY-0.0.9/creyPY.egg-info/
--rw-r--r--   0 conrad     (501) staff       (20)      266 2024-04-01 16:40:11.000000 creyPY-0.0.9/creyPY.egg-info/PKG-INFO
--rw-r--r--   0 conrad     (501) staff       (20)      488 2024-04-01 16:40:11.000000 creyPY-0.0.9/creyPY.egg-info/SOURCES.txt
--rw-r--r--   0 conrad     (501) staff       (20)        1 2024-04-01 16:40:11.000000 creyPY-0.0.9/creyPY.egg-info/dependency_links.txt
--rw-r--r--   0 conrad     (501) staff       (20)        7 2024-04-01 16:40:11.000000 creyPY-0.0.9/creyPY.egg-info/top_level.txt
--rw-r--r--   0 conrad     (501) staff       (20)       38 2024-04-01 16:40:11.348322 creyPY-0.0.9/setup.cfg
--rw-r--r--   0 conrad     (501) staff       (20)      352 2024-04-01 16:37:40.000000 creyPY-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:48:07.964023 creyPY-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-01 18:47:49.000000 creyPY-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-01 18:48:07.964023 creyPY-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-01 18:47:49.000000 creyPY-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:48:07.960023 creyPY-0.1.1/creyPY/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:47:49.000000 creyPY-0.1.1/creyPY/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:48:07.964023 creyPY-0.1.1/creyPY/const/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-01 18:47:49.000000 creyPY-0.1.1/creyPY/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-01 18:47:49.000000 creyPY-0.1.1/creyPY/const/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-01 18:47:49.000000 creyPY-0.1.1/creyPY/const/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-01 18:47:49.000000 creyPY-0.1.1/creyPY/const/stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:48:07.964023 creyPY-0.1.1/creyPY/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-01 18:47:49.000000 creyPY-0.1.1/creyPY/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-01 18:47:49.000000 creyPY-0.1.1/creyPY/fastapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-01 18:47:49.000000 creyPY-0.1.1/creyPY/fastapi/crud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:48:07.964023 creyPY-0.1.1/creyPY/fastapi/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 18:47:49.000000 creyPY-0.1.1/creyPY/fastapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-01 18:47:49.000000 creyPY-0.1.1/creyPY/fastapi/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-01 18:47:49.000000 creyPY-0.1.1/creyPY/fastapi/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:48:07.964023 creyPY-0.1.1/creyPY/fastapi/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 18:47:49.000000 creyPY-0.1.1/creyPY/fastapi/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-01 18:47:49.000000 creyPY-0.1.1/creyPY/fastapi/schemas/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:48:07.964023 creyPY-0.1.1/creyPY.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-01 18:48:07.000000 creyPY-0.1.1/creyPY.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-01 18:48:07.000000 creyPY-0.1.1/creyPY.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:48:07.000000 creyPY-0.1.1/creyPY.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-01 18:48:07.000000 creyPY-0.1.1/creyPY.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 18:48:07.000000 creyPY-0.1.1/creyPY.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 18:48:07.964023 creyPY-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-01 18:47:49.000000 creyPY-0.1.1/setup.py
```

### Comparing `creyPY-0.0.9/LICENSE` & `creyPY-0.1.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 Conrad
+Copyright (c) 2024 Conrad Großer
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `creyPY-0.0.9/creyPY/const/i18n.py` & `creyPY-0.1.1/creyPY/const/i18n.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.0.9/creyPY/const/stripe.py` & `creyPY-0.1.1/creyPY/const/stripe.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.0.9/creyPY/fastapi/app.py` & `creyPY-0.1.1/creyPY/fastapi/app.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.0.9/creyPY/fastapi/crud.py` & `creyPY-0.1.1/creyPY/fastapi/crud.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,24 +15,26 @@
     if obj is None:
         raise HTTPException(status_code=404, detail="The object does not exist.")
     if expunge:
         db.expunge(obj)
     return obj
 
 
+# TODO: Add testing
 def create_obj_from_data(
     data: BaseModel, model: Type[T], db: Session, additonal_data={}, exclude={}
 ) -> T:
     obj = model(**data.model_dump(exclude=exclude) | additonal_data)
     db.add(obj)
     db.commit()
     db.refresh(obj)
     return obj
 
 
+# TODO: Add testing
 def update_obj_from_data(
     data: BaseModel,
     model: Type[T],
     id: UUID | str,
     db: Session,
     partial: bool = False,
     ignore_fields=[],
@@ -46,13 +48,14 @@
         if field not in ignore_fields:
             setattr(obj, field, data_dict[field])
     db.commit()
     db.refresh(obj)
     return obj
 
 
+# TODO: Add testing
 def delete_object(db_class: Type[T], id: UUID | str, db: Session) -> None:
     obj = db.query(db_class).filter(db_class.id == id).one_or_none()
     if obj is None:
         raise HTTPException(status_code=404, detail="The object does not exist.")
     db.delete(obj)
     db.commit()
```

### Comparing `creyPY-0.0.9/creyPY/fastapi/models/base.py` & `creyPY-0.1.1/creyPY/fastapi/models/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,11 +15,14 @@
     id = Column(UUID(as_uuid=True), primary_key=True, default=uuid.uuid4)
     created_at = Column(DateTime(timezone=True), server_default=func.now())
     updated_at = Column(DateTime, default=datetime.utcnow, onupdate=datetime.utcnow)
     created_by_id = Column(String)
 
     __name__: str
 
+    # TODO: Add default representation string
+    # TODO: Add automated foreign key resolution
+
     # Generate __tablename__ automatically
     @declared_attr
     def __tablename__(cls) -> str:
         return cls.__name__.lower()
```

### Comparing `creyPY-0.0.9/creyPY/fastapi/pagination.py` & `creyPY-0.1.1/creyPY/fastapi/pagination.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from fastapi_pagination.bases import AbstractPage, AbstractParams
 from fastapi_pagination.types import GreaterEqualOne, GreaterEqualZero
 from pydantic.json_schema import SkipJsonSchema
 
 T = TypeVar("T")
 
 
+# TODO: Add complete fastapi-pagination proxy here
+# TODO: Add pagination off functionality
+# SkipJsonSchema is used to avoid generating invalid JSON schema in FastAPI
 class Page(AbstractPage[T], Generic[T]):
     results: Sequence[T]
     page: GreaterEqualOne | SkipJsonSchema[None] = None
     size: GreaterEqualOne | SkipJsonSchema[None] = None
     pages: GreaterEqualZero | SkipJsonSchema[None] = None
     total: GreaterEqualZero
     has_next: bool | SkipJsonSchema[None] = None
```

