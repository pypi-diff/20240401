# Comparing `tmp/djdantic-0.0.8.tar.gz` & `tmp/djdantic-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djdantic-0.0.8.tar", last modified: Wed Apr 19 12:21:16 2023, max compression
+gzip compressed data, was "djdantic-0.0.9.tar", last modified: Wed Apr 19 14:02:25 2023, max compression
```

## Comparing `djdantic-0.0.8.tar` & `djdantic-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:21:16.812976 djdantic-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    26022 2023-04-19 12:21:11.000000 djdantic-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-19 12:21:11.000000 djdantic-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-19 12:21:16.812976 djdantic-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-19 12:21:11.000000 djdantic-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:21:16.808976 djdantic-0.0.8/djdantic/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:21:16.812976 djdantic-0.0.8/djdantic/context/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/context/access.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:21:16.812976 djdantic-0.0.8/djdantic/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/schemas/access.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/schemas/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/schemas/price.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:21:16.812976 djdantic-0.0.8/djdantic/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:21:16.812976 djdantic-0.0.8/djdantic/utils/pydantic_django/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/pydantic_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/pydantic_django/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/pydantic_django/django_to_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/pydantic_django/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/pydantic_django/pydantic_to_django.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/pydantic_django/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:21:16.812976 djdantic-0.0.8/djdantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-19 12:21:16.000000 djdantic-0.0.8/djdantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-19 12:21:16.000000 djdantic-0.0.8/djdantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:21:16.000000 djdantic-0.0.8/djdantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:21:16.000000 djdantic-0.0.8/djdantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-19 12:21:16.000000 djdantic-0.0.8/djdantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 12:21:16.000000 djdantic-0.0.8/djdantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-19 12:21:16.812976 djdantic-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 12:21:11.000000 djdantic-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:02:25.188737 djdantic-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    26022 2023-04-19 14:02:20.000000 djdantic-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-19 14:02:20.000000 djdantic-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-19 14:02:25.188737 djdantic-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-19 14:02:20.000000 djdantic-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:02:25.184737 djdantic-0.0.9/djdantic/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:02:25.184737 djdantic-0.0.9/djdantic/context/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/context/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:02:25.184737 djdantic-0.0.9/djdantic/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/schemas/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/schemas/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/schemas/price.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:02:25.184737 djdantic-0.0.9/djdantic/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/utils/pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:02:25.188737 djdantic-0.0.9/djdantic/utils/pydantic_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/utils/pydantic_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/utils/pydantic_django/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/utils/pydantic_django/django_to_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/utils/pydantic_django/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/utils/pydantic_django/pydantic_to_django.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/utils/pydantic_django/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-19 14:02:20.000000 djdantic-0.0.9/djdantic/utils/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:02:25.184737 djdantic-0.0.9/djdantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-19 14:02:25.000000 djdantic-0.0.9/djdantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-19 14:02:25.000000 djdantic-0.0.9/djdantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 14:02:25.000000 djdantic-0.0.9/djdantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 14:02:25.000000 djdantic-0.0.9/djdantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-19 14:02:25.000000 djdantic-0.0.9/djdantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 14:02:25.000000 djdantic-0.0.9/djdantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-19 14:02:25.188737 djdantic-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 14:02:20.000000 djdantic-0.0.9/setup.py
```

### Comparing `djdantic-0.0.8/LICENSE` & `djdantic-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.8/PKG-INFO` & `djdantic-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djdantic
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities to use pydantic with the django orm
 Home-page: https://github.com/Voltane-EU/djdantic
 Author: Manuel Stingl
 Author-email: opensource@voltane.eu
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `djdantic-0.0.8/README.md` & `djdantic-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.8/djdantic/fields.py` & `djdantic-0.0.9/djdantic/fields.py`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.8/djdantic/models.py` & `djdantic-0.0.9/djdantic/models.py`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.8/djdantic/schemas/access.py` & `djdantic-0.0.9/djdantic/schemas/access.py`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.8/djdantic/utils/pydantic.py` & `djdantic-0.0.9/djdantic/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.8/djdantic/utils/pydantic_django/checks.py` & `djdantic-0.0.9/djdantic/utils/pydantic_django/checks.py`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.8/djdantic/utils/pydantic_django/django_to_pydantic.py` & `djdantic-0.0.9/djdantic/utils/pydantic_django/django_to_pydantic.py`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.8/djdantic/utils/pydantic_django/pydantic.py` & `djdantic-0.0.9/djdantic/utils/pydantic_django/pydantic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from typing import Any, Generator, Mapping, Optional, Tuple, Type, TypeVar, Union
-from fastapi.exceptions import RequestValidationError
 from pydantic import BaseModel, validate_model
 from django.db import models
 from django.db.models.manager import Manager
 from djutils.asyncio import AllowAsyncUnsafe
 from ... import context
 from ..pydantic import get_orm_field_attr
 from .django_to_pydantic import transfer_from_orm
 
+try:
+    from fastapi.exceptions import RequestValidationError
+
+except ImportError:
+    from pydantic import ValidationError as RequestValidationError
+
 
 class DjangoORMBaseModel(BaseModel):
     @classmethod
     def from_orm(cls, obj: models.Model, filter_submodel: Optional[Mapping[Manager, models.Q]] = None):
         return transfer_from_orm(cls, obj, filter_submodel=filter_submodel)
 
     class Config:
```

### Comparing `djdantic-0.0.8/djdantic/utils/pydantic_django/pydantic_to_django.py` & `djdantic-0.0.9/djdantic/utils/pydantic_django/pydantic_to_django.py`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.8/djdantic.egg-info/PKG-INFO` & `djdantic-0.0.9/djdantic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djdantic
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities to use pydantic with the django orm
 Home-page: https://github.com/Voltane-EU/djdantic
 Author: Manuel Stingl
 Author-email: opensource@voltane.eu
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `djdantic-0.0.8/djdantic.egg-info/SOURCES.txt` & `djdantic-0.0.9/djdantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.8/setup.cfg` & `djdantic-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djdantic
-version = 0.0.8
+version = 0.0.9
 author = Manuel Stingl
 author_email = opensource@voltane.eu
 description = Utilities to use pydantic with the django orm
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GNU LGPLv2.1
 classifiers =
```

