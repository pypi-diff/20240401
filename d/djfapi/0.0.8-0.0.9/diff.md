# Comparing `tmp/djfapi-0.0.8.tar.gz` & `tmp/djfapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djfapi-0.0.8.tar", last modified: Thu Jun  9 07:42:44 2022, max compression
+gzip compressed data, was "djfapi-0.0.9.tar", last modified: Thu Jun  9 09:07:35 2022, max compression
```

## Comparing `djfapi-0.0.8.tar` & `djfapi-0.0.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2022-06-09 07:42:44.395087 djfapi-0.0.8/
--rw-rw-rw-   0        0        0    26511 2022-06-02 06:56:19.000000 djfapi-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      332 2022-06-02 06:56:19.000000 djfapi-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      825 2022-06-09 07:42:44.396086 djfapi-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      206 2022-06-02 06:56:19.000000 djfapi-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-06-09 07:42:44.255153 djfapi-0.0.8/djfapi/
--rw-rw-rw-   0        0        0       21 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-09 07:42:44.272154 djfapi-0.0.8/djfapi/enums/
--rw-rw-rw-   0        0        0       40 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/enums/__init__.py
--rw-rw-rw-   0        0        0     7709 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/enums/country_codes.py
--rw-rw-rw-   0        0        0     1525 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-06-09 07:42:44.297815 djfapi-0.0.8/djfapi/handlers/
--rw-rw-rw-   0        0        0       21 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/handlers/__init__.py
--rw-rw-rw-   0        0        0     3903 2022-06-08 06:55:30.000000 djfapi-0.0.8/djfapi/handlers/error.py
-drwxrwxrwx   0        0        0        0 2022-06-09 07:42:44.303816 djfapi-0.0.8/djfapi/middleware/
--rw-rw-rw-   0        0        0       22 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/middleware/__init__.py
--rw-rw-rw-   0        0        0      911 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/middleware/sentry.py
-drwxrwxrwx   0        0        0        0 2022-06-09 07:42:44.308817 djfapi-0.0.8/djfapi/patch/
--rw-rw-rw-   0        0        0       23 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/patch/__init__.py
--rw-rw-rw-   0        0        0      575 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/patch/fastapi.py
-drwxrwxrwx   0        0        0        0 2022-06-09 07:42:44.315814 djfapi-0.0.8/djfapi/routing/
--rw-rw-rw-   0        0        0       44 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/routing/__init__.py
--rw-rw-rw-   0        0        0     1415 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/routing/base.py
--rw-rw-rw-   0        0        0     8892 2022-06-09 07:40:35.000000 djfapi-0.0.8/djfapi/routing/django.py
-drwxrwxrwx   0        0        0        0 2022-06-09 07:42:44.331816 djfapi-0.0.8/djfapi/schemas/
--rw-rw-rw-   0        0        0      223 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/schemas/__init__.py
--rw-rw-rw-   0        0        0     2374 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/schemas/access.py
--rw-rw-rw-   0        0        0      264 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/schemas/error.py
--rw-rw-rw-   0        0        0     2109 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/schemas/event.py
--rw-rw-rw-   0        0        0      442 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/schemas/health.py
--rw-rw-rw-   0        0        0      413 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/schemas/price.py
--rw-rw-rw-   0        0        0      991 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/schemas/query.py
-drwxrwxrwx   0        0        0        0 2022-06-09 07:42:44.335818 djfapi-0.0.8/djfapi/security/
--rw-rw-rw-   0        0        0       19 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/security/__init__.py
--rw-rw-rw-   0        0        0     2767 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/security/jwt.py
-drwxrwxrwx   0        0        0        0 2022-06-09 07:42:44.363086 djfapi-0.0.8/djfapi/utils/
--rw-rw-rw-   0        0        0       95 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/utils/__init__.py
--rw-rw-rw-   0        0        0     1101 2022-06-07 09:46:23.000000 djfapi-0.0.8/djfapi/utils/asyncio.py
--rw-rw-rw-   0        0        0      346 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/utils/dict.py
--rw-rw-rw-   0        0        0      666 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/utils/fastapi.py
--rw-rw-rw-   0        0        0     1820 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/utils/fastapi_django.py
--rw-rw-rw-   0        0        0     1034 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/utils/health_check.py
--rw-rw-rw-   0        0        0     5715 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/utils/pydantic.py
-drwxrwxrwx   0        0        0        0 2022-06-09 07:42:44.389090 djfapi-0.0.8/djfapi/utils/pydantic_django/
--rw-rw-rw-   0        0        0      292 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/utils/pydantic_django/__init__.py
--rw-rw-rw-   0        0        0     2001 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/utils/pydantic_django/checks.py
--rw-rw-rw-   0        0        0    11174 2022-06-07 09:48:52.000000 djfapi-0.0.8/djfapi/utils/pydantic_django/django_to_pydantic.py
--rw-rw-rw-   0        0        0     1519 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/utils/pydantic_django/pydantic.py
--rw-rw-rw-   0        0        0    14347 2022-06-07 09:49:10.000000 djfapi-0.0.8/djfapi/utils/pydantic_django/pydantic_to_django.py
--rw-rw-rw-   0        0        0      309 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/utils/pydantic_django/utils.py
--rw-rw-rw-   0        0        0     1726 2022-06-07 14:12:34.000000 djfapi-0.0.8/djfapi/utils/sentry.py
--rw-rw-rw-   0        0        0     1366 2022-06-07 09:48:28.000000 djfapi-0.0.8/djfapi/utils/sync.py
--rw-rw-rw-   0        0        0      366 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/utils/typing.py
-drwxrwxrwx   0        0        0        0 2022-06-09 07:42:44.394087 djfapi-0.0.8/djfapi/validators/
--rw-rw-rw-   0        0        0       24 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/validators/__init__.py
--rw-rw-rw-   0        0        0      264 2022-06-02 06:56:19.000000 djfapi-0.0.8/djfapi/validators/language.py
-drwxrwxrwx   0        0        0        0 2022-06-09 07:42:44.268153 djfapi-0.0.8/djfapi.egg-info/
--rw-rw-rw-   0        0        0      825 2022-06-09 07:42:43.000000 djfapi-0.0.8/djfapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1347 2022-06-09 07:42:44.000000 djfapi-0.0.8/djfapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-09 07:42:43.000000 djfapi-0.0.8/djfapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-06-02 07:00:14.000000 djfapi-0.0.8/djfapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      117 2022-06-09 07:42:44.000000 djfapi-0.0.8/djfapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-06-09 07:42:44.000000 djfapi-0.0.8/djfapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      863 2022-06-09 07:42:44.397087 djfapi-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-06-02 06:56:19.000000 djfapi-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-09 09:07:35.555737 djfapi-0.0.9/
+-rw-rw-rw-   0        0        0    26511 2022-06-02 06:56:19.000000 djfapi-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      332 2022-06-02 06:56:19.000000 djfapi-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      825 2022-06-09 09:07:35.556735 djfapi-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2022-06-02 06:56:19.000000 djfapi-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-06-09 09:07:35.416737 djfapi-0.0.9/djfapi/
+-rw-rw-rw-   0        0        0       21 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-09 09:07:35.437736 djfapi-0.0.9/djfapi/enums/
+-rw-rw-rw-   0        0        0       40 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/enums/__init__.py
+-rw-rw-rw-   0        0        0     7709 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/enums/country_codes.py
+-rw-rw-rw-   0        0        0     1525 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/exceptions.py
+drwxrwxrwx   0        0        0        0 2022-06-09 09:07:35.442737 djfapi-0.0.9/djfapi/handlers/
+-rw-rw-rw-   0        0        0       21 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/handlers/__init__.py
+-rw-rw-rw-   0        0        0     3903 2022-06-08 06:55:30.000000 djfapi-0.0.9/djfapi/handlers/error.py
+drwxrwxrwx   0        0        0        0 2022-06-09 09:07:35.447736 djfapi-0.0.9/djfapi/middleware/
+-rw-rw-rw-   0        0        0       22 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/middleware/__init__.py
+-rw-rw-rw-   0        0        0      911 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/middleware/sentry.py
+drwxrwxrwx   0        0        0        0 2022-06-09 09:07:35.453738 djfapi-0.0.9/djfapi/patch/
+-rw-rw-rw-   0        0        0       23 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/patch/__init__.py
+-rw-rw-rw-   0        0        0      575 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/patch/fastapi.py
+drwxrwxrwx   0        0        0        0 2022-06-09 09:07:35.461736 djfapi-0.0.9/djfapi/routing/
+-rw-rw-rw-   0        0        0       44 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/routing/__init__.py
+-rw-rw-rw-   0        0        0     1416 2022-06-09 09:00:32.000000 djfapi-0.0.9/djfapi/routing/base.py
+-rw-rw-rw-   0        0        0     9063 2022-06-09 09:06:08.000000 djfapi-0.0.9/djfapi/routing/django.py
+drwxrwxrwx   0        0        0        0 2022-06-09 09:07:35.478737 djfapi-0.0.9/djfapi/schemas/
+-rw-rw-rw-   0        0        0      223 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/schemas/__init__.py
+-rw-rw-rw-   0        0        0     2374 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/schemas/access.py
+-rw-rw-rw-   0        0        0      264 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/schemas/error.py
+-rw-rw-rw-   0        0        0     2109 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/schemas/event.py
+-rw-rw-rw-   0        0        0      442 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/schemas/health.py
+-rw-rw-rw-   0        0        0      413 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/schemas/price.py
+-rw-rw-rw-   0        0        0      991 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/schemas/query.py
+drwxrwxrwx   0        0        0        0 2022-06-09 09:07:35.484736 djfapi-0.0.9/djfapi/security/
+-rw-rw-rw-   0        0        0       19 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/security/__init__.py
+-rw-rw-rw-   0        0        0     2767 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/security/jwt.py
+drwxrwxrwx   0        0        0        0 2022-06-09 09:07:35.527737 djfapi-0.0.9/djfapi/utils/
+-rw-rw-rw-   0        0        0       95 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/utils/__init__.py
+-rw-rw-rw-   0        0        0     1101 2022-06-07 09:46:23.000000 djfapi-0.0.9/djfapi/utils/asyncio.py
+-rw-rw-rw-   0        0        0      346 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/utils/dict.py
+-rw-rw-rw-   0        0        0      666 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/utils/fastapi.py
+-rw-rw-rw-   0        0        0     1820 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/utils/fastapi_django.py
+-rw-rw-rw-   0        0        0     1034 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/utils/health_check.py
+-rw-rw-rw-   0        0        0     5715 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/utils/pydantic.py
+drwxrwxrwx   0        0        0        0 2022-06-09 09:07:35.546737 djfapi-0.0.9/djfapi/utils/pydantic_django/
+-rw-rw-rw-   0        0        0      292 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/utils/pydantic_django/__init__.py
+-rw-rw-rw-   0        0        0     2001 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/utils/pydantic_django/checks.py
+-rw-rw-rw-   0        0        0    11174 2022-06-09 09:03:51.000000 djfapi-0.0.9/djfapi/utils/pydantic_django/django_to_pydantic.py
+-rw-rw-rw-   0        0        0     1519 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/utils/pydantic_django/pydantic.py
+-rw-rw-rw-   0        0        0    14347 2022-06-07 09:49:10.000000 djfapi-0.0.9/djfapi/utils/pydantic_django/pydantic_to_django.py
+-rw-rw-rw-   0        0        0      309 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/utils/pydantic_django/utils.py
+-rw-rw-rw-   0        0        0     1726 2022-06-07 14:12:34.000000 djfapi-0.0.9/djfapi/utils/sentry.py
+-rw-rw-rw-   0        0        0     1366 2022-06-07 09:48:28.000000 djfapi-0.0.9/djfapi/utils/sync.py
+-rw-rw-rw-   0        0        0      366 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/utils/typing.py
+drwxrwxrwx   0        0        0        0 2022-06-09 09:07:35.553738 djfapi-0.0.9/djfapi/validators/
+-rw-rw-rw-   0        0        0       24 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/validators/__init__.py
+-rw-rw-rw-   0        0        0      264 2022-06-02 06:56:19.000000 djfapi-0.0.9/djfapi/validators/language.py
+drwxrwxrwx   0        0        0        0 2022-06-09 09:07:35.433740 djfapi-0.0.9/djfapi.egg-info/
+-rw-rw-rw-   0        0        0      825 2022-06-09 09:07:34.000000 djfapi-0.0.9/djfapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1347 2022-06-09 09:07:35.000000 djfapi-0.0.9/djfapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-09 09:07:34.000000 djfapi-0.0.9/djfapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-06-02 07:00:14.000000 djfapi-0.0.9/djfapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      117 2022-06-09 09:07:35.000000 djfapi-0.0.9/djfapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2022-06-09 09:07:35.000000 djfapi-0.0.9/djfapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      863 2022-06-09 09:07:35.557740 djfapi-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       41 2022-06-02 06:56:19.000000 djfapi-0.0.9/setup.py
```

### Comparing `djfapi-0.0.8/LICENSE` & `djfapi-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/PKG-INFO` & `djfapi-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djfapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities for use with FastAPI and django
 Home-page: https://github.com/Voltane-EU/djfapi
 Author: Manuel Stingl
 Author-email: opensource@voltane.eu
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `djfapi-0.0.8/djfapi/enums/country_codes.py` & `djfapi-0.0.9/djfapi/enums/country_codes.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/exceptions.py` & `djfapi-0.0.9/djfapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/handlers/error.py` & `djfapi-0.0.9/djfapi/handlers/error.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/middleware/sentry.py` & `djfapi-0.0.9/djfapi/middleware/sentry.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/patch/fastapi.py` & `djfapi-0.0.9/djfapi/patch/fastapi.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/routing/base.py` & `djfapi-0.0.9/djfapi/routing/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class RouterSchema(BaseModel, arbitrary_types_allowed=True, extra=Extra.allow):
     name: str
     list: Type[BaseModel]
     get: Type[TBaseModel]
     create: Optional[Type[TCreateModel]] = None
-    create_multi: bool = True
+    create_multi: bool = False
     update: Optional[Type[TUpdateModel]] = None
     delete: bool = True
     children: List[RouterSchema] = []
     parent: Optional[RouterSchema] = None
     security: Optional[SecurityBase] = None
     security_scopes: Optional[Sequence[str]] = None
```

### Comparing `djfapi-0.0.8/djfapi/routing/django.py` & `djfapi-0.0.9/djfapi/routing/django.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from functools import partial
 from typing import Any, List, Optional, Type, TypeVar, Union
 import forge
 from django.db import models
-from pydantic import BaseModel
 from fastapi import APIRouter, Security, Path, Body, Depends
 from fastapi.security.base import SecurityBase
 from ..schemas import Access, Error
 from ..utils.fastapi import Pagination, depends_pagination
 from ..utils.pydantic_django import transfer_to_orm, TransferAction
 from ..exceptions import ValidationError
 from .base import TBaseModel, TCreateModel, TUpdateModel
@@ -28,28 +27,35 @@
     model: Type[TDjangoModel]
     get: Type[TBaseModel]
     create: Type[TCreateModel] = None
     update: Type[TUpdateModel] = None
     delete_status: Optional[Any] = None
     pagination_options: dict = {}
 
+    def __init__(self, **data: Any) -> None:
+        if self.create_multi:
+            # create_multi is WIP
+            raise NotImplementedError("create_multi is not supported for DjangoRouterSchema")
+
+        super().__init__(**data)
+
     def objects_filter(self, access: Optional[Access] = None) -> models.Q:
         return models.Q()
 
     def objects_get_filtered(self, *, access: Optional[Access] = None, pagination: Pagination) -> List[TDjangoModel]:
         return list(pagination.query(self.model.objects, self.objects_filter(access)))
 
     def object_get_by_id(self, id: str, access: Optional[Access] = None) -> TDjangoModel:
         return self.model.objects.filter(self.objects_filter(access)).get(id=id)
 
     def object_create(self, *, access: Optional[Access] = None, data: Union[TCreateModel, List[TCreateModel]]) -> List[TDjangoModel]:
         if not isinstance(data, list):
             data = [data]
 
-        if not self.create_multi and len(data) > 1:
+        elif not self.create_multi:
             raise ValidationError(detail=Error(code='create_multi_disabled'))
 
         instances = []
         for el in data:
             instance: TDjangoModel = self.model()
             transfer_to_orm(el, instance, action=TransferAction.CREATE, access=access)
             instances.append(instance)
@@ -91,23 +97,23 @@
         return forge.sign(*[
             *self._security_signature('list'),
             forge.kwarg('pagination', type=Pagination, default=Depends(depends_pagination(**self.pagination_options))),
         ])(self.endpoint_list)
 
     def endpoint_post(self, *, data: TCreateModel, access: Optional[Access] = None, **kwargs):
         obj = self.object_create(access=access, data=data)
-        if isinstance(obj, list):
+        if len(obj) > 1:
             return [self.get.from_orm(o) for o in obj]
 
-        return self.get.from_orm(obj)
+        return self.get.from_orm(obj[0])
 
     def _create_endpoint_post(self):
         create_type = self.create
         if self.create_multi:
-            create_type = Union[self.create, List[self.create]]
+            create_type = List[self.create]
 
         return forge.sign(*[
             forge.kwarg('data', type=create_type, default=Body(...)),
             *self._security_signature('post'),
         ])(self.endpoint_post)
 
     def endpoint_get(self, *, id: str = Path(...), access: Optional[Access] = None, **kwargs):
```

### Comparing `djfapi-0.0.8/djfapi/schemas/access.py` & `djfapi-0.0.9/djfapi/schemas/access.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/schemas/event.py` & `djfapi-0.0.9/djfapi/schemas/event.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/schemas/query.py` & `djfapi-0.0.9/djfapi/schemas/query.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/security/jwt.py` & `djfapi-0.0.9/djfapi/security/jwt.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/utils/asyncio.py` & `djfapi-0.0.9/djfapi/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/utils/fastapi.py` & `djfapi-0.0.9/djfapi/utils/fastapi.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/utils/fastapi_django.py` & `djfapi-0.0.9/djfapi/utils/fastapi_django.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/utils/health_check.py` & `djfapi-0.0.9/djfapi/utils/health_check.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/utils/pydantic.py` & `djfapi-0.0.9/djfapi/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/utils/pydantic_django/checks.py` & `djfapi-0.0.9/djfapi/utils/pydantic_django/checks.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/utils/pydantic_django/django_to_pydantic.py` & `djfapi-0.0.9/djfapi/utils/pydantic_django/django_to_pydantic.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/utils/pydantic_django/pydantic.py` & `djfapi-0.0.9/djfapi/utils/pydantic_django/pydantic.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/utils/pydantic_django/pydantic_to_django.py` & `djfapi-0.0.9/djfapi/utils/pydantic_django/pydantic_to_django.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/utils/sentry.py` & `djfapi-0.0.9/djfapi/utils/sentry.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi/utils/sync.py` & `djfapi-0.0.9/djfapi/utils/sync.py`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/djfapi.egg-info/PKG-INFO` & `djfapi-0.0.9/djfapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djfapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities for use with FastAPI and django
 Home-page: https://github.com/Voltane-EU/djfapi
 Author: Manuel Stingl
 Author-email: opensource@voltane.eu
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `djfapi-0.0.8/djfapi.egg-info/SOURCES.txt` & `djfapi-0.0.9/djfapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djfapi-0.0.8/setup.cfg` & `djfapi-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a66 6170 690d 0a76 6572 7369   = djfapi..versi
-00000020: 6f6e 203d 2030 2e30 2e38 0d0a 6175 7468  on = 0.0.8..auth
+00000020: 6f6e 203d 2030 2e30 2e39 0d0a 6175 7468  on = 0.0.9..auth
 00000030: 6f72 203d 204d 616e 7565 6c20 5374 696e  or = Manuel Stin
 00000040: 676c 0d0a 6175 7468 6f72 5f65 6d61 696c  gl..author_email
 00000050: 203d 206f 7065 6e73 6f75 7263 6540 766f   = opensource@vo
 00000060: 6c74 616e 652e 6575 0d0a 6465 7363 7269  ltane.eu..descri
 00000070: 7074 696f 6e20 3d20 5574 696c 6974 6965  ption = Utilitie
 00000080: 7320 666f 7220 7573 6520 7769 7468 2046  s for use with F
 00000090: 6173 7441 5049 2061 6e64 2064 6a61 6e67  astAPI and djang
```

