# Comparing `tmp/creyPY-0.0.7.tar.gz` & `tmp/creyPY-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creyPY-0.0.7.tar", last modified: Mon Apr  1 16:21:05 2024, max compression
+gzip compressed data, was "creyPY-0.0.8.tar", last modified: Mon Apr  1 16:29:34 2024, max compression
```

## Comparing `creyPY-0.0.7.tar` & `creyPY-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:21:05.435537 creyPY-0.0.7/
--rw-r--r--   0 conrad     (501) staff       (20)     1063 2024-04-01 15:11:19.000000 creyPY-0.0.7/LICENSE
--rw-r--r--   0 conrad     (501) staff       (20)      266 2024-04-01 16:21:05.435327 creyPY-0.0.7/PKG-INFO
--rw-r--r--   0 conrad     (501) staff       (20)      181 2024-04-01 16:11:11.000000 creyPY-0.0.7/README.md
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:21:05.432447 creyPY-0.0.7/creyPY/
--rw-r--r--   0 conrad     (501) staff       (20)        0 2024-04-01 15:50:43.000000 creyPY-0.0.7/creyPY/__init__.py
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:21:05.433928 creyPY-0.0.7/creyPY/const/
--rw-r--r--   0 conrad     (501) staff       (20)       88 2024-04-01 16:15:06.000000 creyPY-0.0.7/creyPY/const/__init__.py
--rw-r--r--   0 conrad     (501) staff       (20)      146 2024-04-01 16:01:50.000000 creyPY-0.0.7/creyPY/const/groups.py
--rw-r--r--   0 conrad     (501) staff       (20)     9324 2024-04-01 15:51:19.000000 creyPY-0.0.7/creyPY/const/i18n.py
--rw-r--r--   0 conrad     (501) staff       (20)     4373 2024-04-01 15:51:31.000000 creyPY-0.0.7/creyPY/const/stripe.py
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:21:05.434845 creyPY-0.0.7/creyPY/fastapi/
--rw-r--r--   0 conrad     (501) staff       (20)       62 2024-04-01 16:15:53.000000 creyPY-0.0.7/creyPY/fastapi/__init__.py
--rw-r--r--   0 conrad     (501) staff       (20)     1624 2024-04-01 16:20:46.000000 creyPY-0.0.7/creyPY/fastapi/crud.py
--rw-r--r--   0 conrad     (501) staff       (20)     1886 2024-04-01 16:10:27.000000 creyPY-0.0.7/creyPY/fastapi/pagination.py
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:21:05.435110 creyPY-0.0.7/creyPY.egg-info/
--rw-r--r--   0 conrad     (501) staff       (20)      266 2024-04-01 16:21:05.000000 creyPY-0.0.7/creyPY.egg-info/PKG-INFO
--rw-r--r--   0 conrad     (501) staff       (20)      336 2024-04-01 16:21:05.000000 creyPY-0.0.7/creyPY.egg-info/SOURCES.txt
--rw-r--r--   0 conrad     (501) staff       (20)        1 2024-04-01 16:21:05.000000 creyPY-0.0.7/creyPY.egg-info/dependency_links.txt
--rw-r--r--   0 conrad     (501) staff       (20)        7 2024-04-01 16:21:05.000000 creyPY-0.0.7/creyPY.egg-info/top_level.txt
--rw-r--r--   0 conrad     (501) staff       (20)       38 2024-04-01 16:21:05.435578 creyPY-0.0.7/setup.cfg
--rw-r--r--   0 conrad     (501) staff       (20)      352 2024-04-01 16:15:57.000000 creyPY-0.0.7/setup.py
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:29:34.474346 creyPY-0.0.8/
+-rw-r--r--   0 conrad     (501) staff       (20)     1063 2024-04-01 15:11:19.000000 creyPY-0.0.8/LICENSE
+-rw-r--r--   0 conrad     (501) staff       (20)      266 2024-04-01 16:29:34.474124 creyPY-0.0.8/PKG-INFO
+-rw-r--r--   0 conrad     (501) staff       (20)      181 2024-04-01 16:11:11.000000 creyPY-0.0.8/README.md
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:29:34.471325 creyPY-0.0.8/creyPY/
+-rw-r--r--   0 conrad     (501) staff       (20)        0 2024-04-01 15:50:43.000000 creyPY-0.0.8/creyPY/__init__.py
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:29:34.472529 creyPY-0.0.8/creyPY/const/
+-rw-r--r--   0 conrad     (501) staff       (20)       88 2024-04-01 16:15:06.000000 creyPY-0.0.8/creyPY/const/__init__.py
+-rw-r--r--   0 conrad     (501) staff       (20)      146 2024-04-01 16:01:50.000000 creyPY-0.0.8/creyPY/const/groups.py
+-rw-r--r--   0 conrad     (501) staff       (20)     9324 2024-04-01 15:51:19.000000 creyPY-0.0.8/creyPY/const/i18n.py
+-rw-r--r--   0 conrad     (501) staff       (20)     4373 2024-04-01 15:51:31.000000 creyPY-0.0.8/creyPY/const/stripe.py
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:29:34.473313 creyPY-0.0.8/creyPY/fastapi/
+-rw-r--r--   0 conrad     (501) staff       (20)      119 2024-04-01 16:28:00.000000 creyPY-0.0.8/creyPY/fastapi/__init__.py
+-rw-r--r--   0 conrad     (501) staff       (20)      848 2024-04-01 16:25:30.000000 creyPY-0.0.8/creyPY/fastapi/app.py
+-rw-r--r--   0 conrad     (501) staff       (20)     1647 2024-04-01 16:29:15.000000 creyPY-0.0.8/creyPY/fastapi/crud.py
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:29:34.473700 creyPY-0.0.8/creyPY/fastapi/models/
+-rw-r--r--   0 conrad     (501) staff       (20)       28 2024-04-01 16:28:08.000000 creyPY-0.0.8/creyPY/fastapi/models/__init__.py
+-rw-r--r--   0 conrad     (501) staff       (20)      771 2024-04-01 16:28:31.000000 creyPY-0.0.8/creyPY/fastapi/models/base.py
+-rw-r--r--   0 conrad     (501) staff       (20)     1886 2024-04-01 16:10:27.000000 creyPY-0.0.8/creyPY/fastapi/pagination.py
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:29:34.473884 creyPY-0.0.8/creyPY.egg-info/
+-rw-r--r--   0 conrad     (501) staff       (20)      266 2024-04-01 16:29:34.000000 creyPY-0.0.8/creyPY.egg-info/PKG-INFO
+-rw-r--r--   0 conrad     (501) staff       (20)      422 2024-04-01 16:29:34.000000 creyPY-0.0.8/creyPY.egg-info/SOURCES.txt
+-rw-r--r--   0 conrad     (501) staff       (20)        1 2024-04-01 16:29:34.000000 creyPY-0.0.8/creyPY.egg-info/dependency_links.txt
+-rw-r--r--   0 conrad     (501) staff       (20)        7 2024-04-01 16:29:34.000000 creyPY-0.0.8/creyPY.egg-info/top_level.txt
+-rw-r--r--   0 conrad     (501) staff       (20)       38 2024-04-01 16:29:34.474385 creyPY-0.0.8/setup.cfg
+-rw-r--r--   0 conrad     (501) staff       (20)      352 2024-04-01 16:28:22.000000 creyPY-0.0.8/setup.py
```

### Comparing `creyPY-0.0.7/LICENSE` & `creyPY-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `creyPY-0.0.7/creyPY/const/i18n.py` & `creyPY-0.0.8/creyPY/const/i18n.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.0.7/creyPY/const/stripe.py` & `creyPY-0.0.8/creyPY/const/stripe.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.0.7/creyPY/fastapi/crud.py` & `creyPY-0.0.8/creyPY/fastapi/crud.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import Type, TypeVar
 from uuid import UUID
 
 from fastapi import HTTPException
 from pydantic import BaseModel
 from sqlalchemy.orm import Session
 
-T = TypeVar("T")  # TODO: bound=Base
+from .models.base import Base
+
+T = TypeVar("T", bound=Base)
 
 
 def get_object_or_404(db_class: Type[T], id: UUID | str, db: Session, expunge: bool = False) -> T:
     obj = db.query(db_class).filter(db_class.id == id).one_or_none()
     if obj is None:
         raise HTTPException(status_code=404, detail="The object does not exist.")
     if expunge:
```

### Comparing `creyPY-0.0.7/creyPY/fastapi/pagination.py` & `creyPY-0.0.8/creyPY/fastapi/pagination.py`

 * *Files identical despite different names*

