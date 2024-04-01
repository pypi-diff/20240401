# Comparing `tmp/strawberry_graphql_django-0.9.4.tar.gz` & `tmp/strawberry_graphql_django-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_graphql_django-0.9.4.tar", max compression
+gzip compressed data, was "strawberry_graphql_django-0.9.5.tar", max compression
```

## Comparing `strawberry_graphql_django-0.9.4.tar` & `strawberry_graphql_django-0.9.5.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1071 2022-03-07 00:11:01.609597 strawberry_graphql_django-0.9.4/LICENSE
--rw-r--r--   0        0        0     2667 2023-01-14 13:58:41.086448 strawberry_graphql_django-0.9.4/README.md
--rw-r--r--   0        0        0     2070 2023-04-03 14:59:33.775637 strawberry_graphql_django-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     1870 2023-04-03 14:46:13.467158 strawberry_graphql_django-0.9.4/strawberry_django/__init__.py
--rw-r--r--   0        0        0      147 2023-04-02 16:19:47.217399 strawberry_graphql_django-0.9.4/strawberry_django/apps.py
--rw-r--r--   0        0        0      473 2022-05-23 21:37:20.321343 strawberry_graphql_django-0.9.4/strawberry_django/arguments.py
--rw-r--r--   0        0        0      141 2023-04-03 14:46:13.467158 strawberry_graphql_django-0.9.4/strawberry_django/auth/__init__.py
--rw-r--r--   0        0        0     1387 2023-04-03 14:46:13.467158 strawberry_graphql_django-0.9.4/strawberry_django/auth/mutations.py
--rw-r--r--   0        0        0      277 2023-04-03 14:46:13.467158 strawberry_graphql_django-0.9.4/strawberry_django/auth/queries.py
--rw-r--r--   0        0        0        0 2022-05-22 20:20:34.117922 strawberry_graphql_django-0.9.4/strawberry_django/extensions/__init__.py
--rw-r--r--   0        0        0     1733 2023-04-03 14:52:32.441304 strawberry_graphql_django-0.9.4/strawberry_django/extensions/django_cache_base.py
--rw-r--r--   0        0        0      510 2022-05-22 20:20:34.121922 strawberry_graphql_django-0.9.4/strawberry_django/extensions/django_validation_cache.py
--rw-r--r--   0        0        0        0 2022-03-07 00:11:01.613597 strawberry_graphql_django-0.9.4/strawberry_django/fields/__init__.py
--rw-r--r--   0        0        0     6326 2023-04-03 14:46:13.467158 strawberry_graphql_django-0.9.4/strawberry_django/fields/field.py
--rw-r--r--   0        0        0      117 2022-03-07 00:11:01.617597 strawberry_graphql_django-0.9.4/strawberry_django/fields/resolvers.py
--rw-r--r--   0        0        0     9178 2023-04-03 14:46:13.467158 strawberry_graphql_django-0.9.4/strawberry_django/fields/types.py
--rw-r--r--   0        0        0     6613 2023-04-03 14:57:27.905779 strawberry_graphql_django-0.9.4/strawberry_django/filters.py
--rw-r--r--   0        0        0      674 2022-03-07 00:11:01.617597 strawberry_graphql_django-0.9.4/strawberry_django/hooks.py
--rw-r--r--   0        0        0     6300 2023-04-03 14:46:13.467158 strawberry_graphql_django-0.9.4/strawberry_django/middlewares/debug_toolbar.py
--rw-r--r--   0        0        0       89 2023-04-03 14:46:13.467158 strawberry_graphql_django-0.9.4/strawberry_django/mutations/__init__.py
--rw-r--r--   0        0        0     5561 2023-04-03 14:46:13.467158 strawberry_graphql_django-0.9.4/strawberry_django/mutations/fields.py
--rw-r--r--   0        0        0      752 2023-04-03 14:46:13.467158 strawberry_graphql_django-0.9.4/strawberry_django/mutations/mutations.py
--rw-r--r--   0        0        0     2609 2023-04-03 14:46:13.467158 strawberry_graphql_django-0.9.4/strawberry_django/ordering.py
--rw-r--r--   0        0        0     1724 2023-04-03 14:46:13.467158 strawberry_graphql_django-0.9.4/strawberry_django/pagination.py
--rw-r--r--   0        0        0     1275 2023-04-03 14:46:13.467158 strawberry_graphql_django-0.9.4/strawberry_django/resolvers.py
--rw-r--r--   0        0        0     1324 2023-04-03 14:46:13.467158 strawberry_graphql_django-0.9.4/strawberry_django/settings.py
--rw-r--r--   0        0        0     1445 2023-04-02 16:19:47.217399 strawberry_graphql_django-0.9.4/strawberry_django/templates/strawberry_django/debug_toolbar.html
--rw-r--r--   0        0        0     8238 2023-04-03 14:46:13.467158 strawberry_graphql_django-0.9.4/strawberry_django/type.py
--rw-r--r--   0        0        0      439 2022-03-07 00:11:01.617597 strawberry_graphql_django-0.9.4/strawberry_django/types.py
--rw-r--r--   0        0        0     2386 2023-04-03 14:46:13.467158 strawberry_graphql_django-0.9.4/strawberry_django/utils.py
--rw-r--r--   0        0        0     4227 1970-01-01 00:00:00.000000 strawberry_graphql_django-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-03-07 00:11:01.609597 strawberry_graphql_django-0.9.5/LICENSE
+-rw-r--r--   0        0        0     2667 2023-01-14 13:58:41.086448 strawberry_graphql_django-0.9.5/README.md
+-rw-r--r--   0        0        0     3045 2023-06-15 23:07:11.452111 strawberry_graphql_django-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     1833 2023-06-14 19:24:36.103341 strawberry_graphql_django-0.9.5/strawberry_django/__init__.py
+-rw-r--r--   0        0        0      147 2023-04-02 16:19:47.217399 strawberry_graphql_django-0.9.5/strawberry_django/apps.py
+-rw-r--r--   0        0        0      473 2022-05-23 21:37:20.321343 strawberry_graphql_django-0.9.5/strawberry_django/arguments.py
+-rw-r--r--   0        0        0      140 2023-06-14 19:24:36.103341 strawberry_graphql_django-0.9.5/strawberry_django/auth/__init__.py
+-rw-r--r--   0        0        0     1402 2023-06-14 19:24:36.103341 strawberry_graphql_django-0.9.5/strawberry_django/auth/mutations.py
+-rw-r--r--   0        0        0      259 2023-06-14 19:24:36.103341 strawberry_graphql_django-0.9.5/strawberry_django/auth/queries.py
+-rw-r--r--   0        0        0        0 2022-05-22 20:20:34.117922 strawberry_graphql_django-0.9.5/strawberry_django/extensions/__init__.py
+-rw-r--r--   0        0        0     1742 2023-06-14 19:24:36.103341 strawberry_graphql_django-0.9.5/strawberry_django/extensions/django_cache_base.py
+-rw-r--r--   0        0        0      510 2022-05-22 20:20:34.121922 strawberry_graphql_django-0.9.5/strawberry_django/extensions/django_validation_cache.py
+-rw-r--r--   0        0        0        0 2022-03-07 00:11:01.613597 strawberry_graphql_django-0.9.5/strawberry_django/fields/__init__.py
+-rw-r--r--   0        0        0     6488 2023-06-15 23:06:20.283148 strawberry_graphql_django-0.9.5/strawberry_django/fields/field.py
+-rw-r--r--   0        0        0      117 2022-03-07 00:11:01.617597 strawberry_graphql_django-0.9.5/strawberry_django/fields/resolvers.py
+-rw-r--r--   0        0        0     9279 2023-06-14 19:24:36.103341 strawberry_graphql_django-0.9.5/strawberry_django/fields/types.py
+-rw-r--r--   0        0        0     6818 2023-06-14 19:24:36.103341 strawberry_graphql_django-0.9.5/strawberry_django/filters.py
+-rw-r--r--   0        0        0      674 2022-03-07 00:11:01.617597 strawberry_graphql_django-0.9.5/strawberry_django/hooks.py
+-rw-r--r--   0        0        0        0 2023-06-14 19:24:36.103341 strawberry_graphql_django-0.9.5/strawberry_django/middlewares/__init__.py
+-rw-r--r--   0        0        0     6359 2023-06-14 19:24:36.103341 strawberry_graphql_django-0.9.5/strawberry_django/middlewares/debug_toolbar.py
+-rw-r--r--   0        0        0       88 2023-06-14 19:24:36.103341 strawberry_graphql_django-0.9.5/strawberry_django/mutations/__init__.py
+-rw-r--r--   0        0        0     5530 2023-06-14 19:24:36.103341 strawberry_graphql_django-0.9.5/strawberry_django/mutations/fields.py
+-rw-r--r--   0        0        0      852 2023-06-14 19:24:36.103341 strawberry_graphql_django-0.9.5/strawberry_django/mutations/mutations.py
+-rw-r--r--   0        0        0     2707 2023-06-14 19:24:36.103341 strawberry_graphql_django-0.9.5/strawberry_django/ordering.py
+-rw-r--r--   0        0        0     1814 2023-06-14 19:24:36.103341 strawberry_graphql_django-0.9.5/strawberry_django/pagination.py
+-rw-r--r--   0        0        0     1329 2023-06-14 19:24:36.103341 strawberry_graphql_django-0.9.5/strawberry_django/resolvers.py
+-rw-r--r--   0        0        0     1321 2023-06-14 19:24:36.103341 strawberry_graphql_django-0.9.5/strawberry_django/settings.py
+-rw-r--r--   0        0        0     1445 2023-04-02 16:19:47.217399 strawberry_graphql_django-0.9.5/strawberry_django/templates/strawberry_django/debug_toolbar.html
+-rw-r--r--   0        0        0     8402 2023-06-15 23:06:20.283148 strawberry_graphql_django-0.9.5/strawberry_django/type.py
+-rw-r--r--   0        0        0      439 2022-03-07 00:11:01.617597 strawberry_graphql_django-0.9.5/strawberry_django/types.py
+-rw-r--r--   0        0        0     2879 2023-06-15 23:06:20.283148 strawberry_graphql_django-0.9.5/strawberry_django/utils.py
+-rw-r--r--   0        0        0     4016 1970-01-01 00:00:00.000000 strawberry_graphql_django-0.9.5/PKG-INFO
```

### Comparing `strawberry_graphql_django-0.9.4/LICENSE` & `strawberry_graphql_django-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_graphql_django-0.9.4/README.md` & `strawberry_graphql_django-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_graphql_django-0.9.4/pyproject.toml` & `strawberry_graphql_django-0.9.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "strawberry-graphql-django"
 packages = [{ include = "strawberry_django" }]
-version = "0.9.4"
+version = "0.9.5"
 description = "Strawberry GraphQL Django extension"
 authors = ["Lauri Hintsala <lauri.hintsala@verkkopaja.fi>"]
 repository = "https://github.com/strawberry-graphql/strawberry-graphql-django"
 license = "MIT"
 readme = "README.md"
 keywords = ["graphql", "api", "django"]
 classifiers = [
@@ -19,56 +19,135 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
+  "Framework :: Django :: 4.2",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 Django = ">=3.2"
-strawberry-graphql = ">=0.160.0"
+strawberry-graphql = ">=0.184.0"
 django-debug-toolbar = { version = ">=3.4", optional = true }
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.21.0"
 pytest = "^7.1.2"
-pytest-asyncio = "^0.20.3"
+pytest-asyncio = "^0.21.0"
 pytest-django = "^4.1.0"
 pytest-pythonpath = "^0.7.3"
 pytest-watch = "^4.2.0"
 pytest-mock = "^3.5.1"
 django-debug-toolbar = "^3.2.4"
 #docs requires
 mkdocs = "^1.4.2"
 mkdocs-markdownextradata-plugin = "^0.2.5"
 mkdocs-material = "^9.0.4"
 mkdocs-minify-plugin = "^0.6.2"
 pymdown-extensions = "^9.5"
+ruff = "^0.0.272"
+django-types = "^0.17.0"
 Markdown = "^3.3.7"
 
 [tool.poetry.extras]
 debug-toolbar = ["django-debug-toolbar"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.isort]
-profile = "black"
-indent = 4
-combine_star = true
-combine_as_imports = true
-lines_after_imports = 2
+[tool.ruff]
+select = [
+  "E",
+  "F",
+  "W",
+  "I",
+  "N",
+  "D",
+  "UP",
+  "YTT",
+  "D2",
+  "D3",
+  "D4",
+  "BLE",
+  "B",
+  "A",
+  "COM",
+  "C4",
+  "DTZ",
+  "T10",
+  "EXE",
+  "ISC",
+  "ICN001",
+  "G",
+  "INP",
+  "PIE",
+  "T20",
+  "PYI",
+  "PT",
+  "Q",
+  "RET",
+  "SIM",
+  "TID",
+  "TCH",
+  "PTH",
+  "ERA",
+  "PGH",
+  "PL",
+  "RSE",
+  "RUF",
+  "TRY",
+  "SLF",
+]
+ignore = ["D1", "D203", "D213", "PLR09", "SLF001", "TRY003", "PGH003"]
+# FIXME: Enable autofix for UP006 when we don't need to support django 3.8 anymore
+unfixable = ["UP006"]
+target-version = "py38"
+exclude = [
+  ".eggs",
+  ".git",
+  ".hg",
+  ".mypy_cache",
+  ".tox",
+  ".venv",
+  "__pycached__",
+  "_build",
+  "buck-out",
+  "build",
+  "dist",
+]
+
+[tool.ruff.per-file-ignores]
+"tests/*" = ["A003", "PLW0603"]
+"examples/*" = ["A003"]
+
+[tool.ruff.isort]
+known-first-party = ["strawberry-django-plus"]
 
 [tool.black]
 target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 preview = true
+exclude = '''
+/(
+    \.eggs
+  | \.git
+  | \.hg
+  | \.mypy_cache
+  | \.tox
+  | \.venv
+  | __pycached__
+  | _build
+  | buck-out
+  | build
+  | dist
+)/
+'''
 
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "tests.django_settings"
 testpaths = ["tests"]
 filterwarnings = "ignore:.*is deprecated.*:DeprecationWarning"
 asyncio_mode = "strict"
```

### Comparing `strawberry_graphql_django-0.9.4/strawberry_django/__init__.py` & `strawberry_graphql_django-0.9.5/strawberry_django/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,28 @@
 from typing import Any, Dict
 
 from django.core.exceptions import ImproperlyConfigured
 from strawberry import auto as _deprecated_auto  # noqa: F401
 
 from . import auth, filters, mutations, ordering, types
 from .fields.field import field
-from .fields.types import (  # noqa: F401
+from .fields.types import (
     DjangoFileType,
     DjangoImageType,
     DjangoModelType,
     ManyToManyInput,
     ManyToOneInput,
     OneToManyInput,
     OneToOneInput,
-    is_auto as _deprecated_is_auto,
 )
-from .filters import filter_deprecated as filter
+from .filters import filter_deprecated as filter  # noqa: A001
 from .resolvers import django_resolver
 from .type import input, mutation, type
 from .utils import fields
 
-
 try:
     from django.contrib.gis import geos  # noqa: F401
 
     from .fields.types import (  # noqa: F401
         LinearRing,
         LineString,
         MultiLineString,
```

### Comparing `strawberry_graphql_django-0.9.4/strawberry_django/auth/mutations.py` & `strawberry_graphql_django-0.9.5/strawberry_django/auth/mutations.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from django.contrib.auth.password_validation import validate_password
 
 from strawberry_django.mutations.fields import (
     DjangoCreateMutation,
     get_input_data,
     update_m2m,
 )
-
-from ..resolvers import django_resolver
+from strawberry_django.resolvers import django_resolver
 
 
 @django_resolver
 def resolve_login(info, username: str, password: str):
     request = info.context.request
     user = auth.authenticate(request, username=username, password=password)
     if user is not None:
```

### Comparing `strawberry_graphql_django-0.9.4/strawberry_django/extensions/django_cache_base.py` & `strawberry_graphql_django-0.9.5/strawberry_django/extensions/django_cache_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 
 from django.core.cache import caches
 from django.core.cache.backends.base import DEFAULT_TIMEOUT
 from strawberry.extensions import SchemaExtension
 
 
 class DjangoCacheBase(SchemaExtension):
-    """
-    Base for a Cache that uses Django built in cache instead of an in memory cache
+    """Base for a Cache that uses Django built in cache instead of an in memory cache.
 
     Arguments:
-
+    ---------
     `cache_name: str`
         Name of the Django Cache to use, defaults to 'default'
 
     `timeout: Optional[float]`
         How long to hold items in the cache. See the Django Cache docs for details
         https://docs.djangoproject.com/en/4.0/topics/cache/
```

### Comparing `strawberry_graphql_django-0.9.4/strawberry_django/fields/field.py` & `strawberry_graphql_django-0.9.5/strawberry_django/fields/field.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,51 @@
-from typing import Any, Optional, Type, TypeVar
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any, TypeVar
 
 from django.db import models
 from strawberry import UNSET
 from strawberry.annotation import StrawberryAnnotation
 from strawberry.field import StrawberryField
 from strawberry.type import StrawberryList, StrawberryOptional
-from strawberry.types import Info
 
-from .. import utils
-from ..filters import StrawberryDjangoFieldFilters
-from ..ordering import StrawberryDjangoFieldOrdering
-from ..pagination import StrawberryDjangoPagination
-from ..resolvers import django_resolver
+from strawberry_django import utils
+from strawberry_django.filters import StrawberryDjangoFieldFilters
+from strawberry_django.ordering import StrawberryDjangoFieldOrdering
+from strawberry_django.pagination import StrawberryDjangoPagination
+from strawberry_django.resolvers import django_resolver
 
+if TYPE_CHECKING:
+    from strawberry.types import Info
 
 T = TypeVar("T", bound="StrawberryDjangoFieldBase")
 
 
 class StrawberryDjangoFieldBase:
     def get_queryset(self, queryset: models.QuerySet, info: Info, **kwargs):
         return queryset
 
     @property
     def django_model(self):
         type_ = utils.unwrap_type(self.type)
         return utils.get_django_model(type_)
 
     @classmethod
-    def from_field(cls: Type[T], field, django_type) -> T:
+    def from_field(cls: type[T], field, django_type) -> T:
         raise NotImplementedError
 
 
 class StrawberryDjangoField(
     StrawberryDjangoPagination,
     StrawberryDjangoFieldOrdering,
     StrawberryDjangoFieldFilters,
     StrawberryDjangoFieldBase,
     StrawberryField,
 ):
-    """Basic field
+    """Basic field.
 
     StrawberryDjangoField inherits all features from StrawberryField and
     implements Django specific functionalities like ordering, filtering and
     pagination.
 
     This field takes care of that Django ORM is always accessed from sync
     context. Resolver function is wrapped in sync_to_async decorator in async
@@ -58,17 +61,17 @@
 
     kwargs argument is passed to ordering, filtering, pagination and
     StrawberryField super classes.
     """
 
     def __init__(
         self,
-        django_name: Optional[str] = None,
-        graphql_name: Optional[str] = None,
-        python_name: Optional[str] = None,
+        django_name: str | None = None,
+        graphql_name: str | None = None,
+        python_name: str | None = None,
         **kwargs,
     ):
         self.django_name = django_name
         self.is_auto = utils.is_auto(kwargs.get("type_annotation", None))
         self.is_relation = False
         self.origin_django_type = None
         self.input_type = None  # used by mutations
@@ -81,15 +84,15 @@
     @property
     def is_list(self):
         return isinstance(self.type, StrawberryList) or (
             self.is_optional and isinstance(self.type.of_type, StrawberryList)
         )
 
     @classmethod
-    def from_field(cls, field: "StrawberryDjangoField", django_type):
+    def from_field(cls, field: StrawberryDjangoField, django_type):
         if utils.is_strawberry_django_field(field) and not field.origin_django_type:
             return field
 
         new_field = StrawberryDjangoField(
             python_name=field.name,
             graphql_name=getattr(field, "graphql_name", None),
             type_annotation=(
@@ -100,15 +103,15 @@
             description=getattr(field, "description", None),
             base_resolver=getattr(field, "base_resolver", None),
             permission_classes=getattr(field, "permission_classes", []),
             default=getattr(field, "default", UNSET),
             default_factory=field.default_factory,
             deprecation_reason=getattr(field, "deprecation_reason", None),
             directives=getattr(field, "directives", []),
-            django_name=getattr(field, "django_name", field.name),
+            django_name=getattr(field, "django_name", None),
         )
         new_field.is_auto = getattr(field, "is_auto", False)
         new_field.origin_django_type = getattr(field, "origin_django_type", None)
         return new_field
 
     def get_result(self, source, info, args, kwargs):
         if self.base_resolver:
@@ -119,22 +122,21 @@
     def get_django_result(
         self,
         source,
         info,
         args,
         kwargs,
     ):
-        return self.resolver(info=info, source=source, *args, **kwargs)
+        return self.resolver(info, source, *args, **kwargs)
 
     def resolver(self, info, source, **kwargs):
         if source is None:
             # TODO: would there be better and safer way to detect root?
             # root query object
             result = self.django_model.objects.all()
-
         else:
             # relation model field
             result = getattr(source, self.django_name or self.python_name)
 
             if isinstance(result, models.manager.Manager):
                 result = result.all()
             elif callable(result):
@@ -154,23 +156,30 @@
         get_queryset = getattr(type_, "get_queryset", None)
         if get_queryset:
             queryset = get_queryset(queryset, info, **kwargs)
         return super().get_queryset(queryset, info, order=order, **kwargs)
 
     @property
     def is_basic_field(self) -> bool:
-        """
+        """Mark this field as not basic.
+
         All StrawberryDjango fields define a custom resolver that needs to be
         run, so always return False here.
         """
         return False
 
 
 def field(
-    resolver=None, *, name=None, field_name=None, filters=UNSET, default=UNSET, **kwargs
+    resolver=None,
+    *,
+    name=None,
+    field_name=None,
+    filters=UNSET,
+    default=UNSET,
+    **kwargs,
 ) -> Any:
     field_ = StrawberryDjangoField(
         python_name=None,
         graphql_name=name,
         type_annotation=None,
         filters=filters,
         django_name=field_name,
```

### Comparing `strawberry_graphql_django-0.9.4/strawberry_django/fields/types.py` & `strawberry_graphql_django-0.9.5/strawberry_django/fields/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 import strawberry
 from django.db.models import Field, Model, fields
 from django.db.models.fields.reverse_related import ForeignObjectRel
 from strawberry import UNSET
 from strawberry.auto import StrawberryAuto
 from strawberry.scalars import JSON
 
-from .. import filters
-
+from strawberry_django import filters
 
 if TYPE_CHECKING:
     from strawberry_django.type import StrawberryDjangoType
 
 
 @strawberry.type
 class DjangoFileType:
@@ -35,34 +34,34 @@
 @strawberry.type
 class DjangoModelType:
     pk: strawberry.ID
 
 
 @strawberry.input
 class OneToOneInput:
-    set: Optional[strawberry.ID]
+    set: Optional[strawberry.ID]  # noqa: A003
 
 
 @strawberry.input
 class OneToManyInput:
-    set: Optional[strawberry.ID]
+    set: Optional[strawberry.ID]  # noqa: A003
 
 
 @strawberry.input
 class ManyToOneInput:
     add: Optional[List[strawberry.ID]] = UNSET
     remove: Optional[List[strawberry.ID]] = UNSET
-    set: Optional[List[strawberry.ID]] = UNSET
+    set: Optional[List[strawberry.ID]] = UNSET  # noqa: A003
 
 
 @strawberry.input
 class ManyToManyInput:
     add: Optional[List[strawberry.ID]] = UNSET
     remove: Optional[List[strawberry.ID]] = UNSET
-    set: Optional[List[strawberry.ID]] = UNSET
+    set: Optional[List[strawberry.ID]] = UNSET  # noqa: A003
 
 
 field_type_map = {
     fields.AutoField: strawberry.ID,
     fields.BigAutoField: strawberry.ID,
     fields.BigIntegerField: int,
     fields.BooleanField: bool,
@@ -96,15 +95,15 @@
 }
 
 if django.VERSION >= (3, 1):
     field_type_map.update(
         {
             fields.json.JSONField: JSON,
             fields.PositiveBigIntegerField: int,
-        }
+        },
     )
 
 try:
     from django.contrib.gis import geos
     from django.contrib.gis.db import models as geos_fields
 
 except django.core.exceptions.ImproperlyConfigured:
@@ -164,28 +163,28 @@
         description="A geographical object that contains multiple line strings.",
     )
 
     MultiPolygon = strawberry.scalar(
         NewType("MultiPolygon", Tuple[Polygon]),
         serialize=lambda v: v.tuple if isinstance(v, geos.MultiPolygon) else v,
         parse_value=lambda v: geos.MultiPolygon(
-            *[geos.Polygon(*[y for y in x]) for x in v]
+            *[geos.Polygon(*list(x)) for x in v],
         ),
         description="A geographical object that contains multiple polygons.",
     )
 
     field_type_map.update(
         {
             geos_fields.PointField: Point,
             geos_fields.LineStringField: LineString,
             geos_fields.PolygonField: Polygon,
             geos_fields.MultiPointField: MultiPoint,
             geos_fields.MultiLineStringField: MultiLineString,
             geos_fields.MultiPolygonField: MultiPolygon,
-        }
+        },
     )
 
 
 input_field_type_map = {
     fields.files.FileField: NotImplemented,
     fields.files.ImageField: NotImplemented,
     fields.related.ForeignKey: OneToManyInput,
@@ -194,44 +193,52 @@
     fields.reverse_related.OneToOneRel: OneToOneInput,
     fields.related.ManyToManyField: ManyToManyInput,
     fields.reverse_related.ManyToManyRel: ManyToManyInput,
 }
 
 
 def resolve_model_field_type(
-    model_field: Union[Field, ForeignObjectRel], django_type: "StrawberryDjangoType"
+    model_field: Union[Field, ForeignObjectRel],
+    django_type: "StrawberryDjangoType",
 ):
     model_field_type = type(model_field)
     field_type: Any = None
     if django_type.is_filter and model_field.is_relation:
         field_type = filters.DjangoModelFilterInput
     elif django_type.is_input:
         field_type = input_field_type_map.get(model_field_type, None)
     if field_type is None:
         field_type = field_type_map.get(model_field_type, NotImplemented)
     if field_type is NotImplemented:
         raise NotImplementedError(
-            f"GraphQL type for model field '{model_field}' has not been implemented"
+            f"GraphQL type for model field '{model_field}' has not been implemented",
         )
-    if django_type.is_filter == "lookups":
-        # TODO: could this be moved into filters.py
-        if not model_field.is_relation and field_type is not bool:
-            field_type = filters.FilterLookup[field_type]
+    # TODO: could this be moved into filters.py
+    if (
+        django_type.is_filter == "lookups"
+        and not model_field.is_relation
+        and field_type is not bool
+    ):
+        field_type = filters.FilterLookup[field_type]
+
     return field_type
 
 
 def resolve_model_field_name(
-    model_field: Union[Field, ForeignObjectRel], is_input=False, is_filter=False
+    model_field: Union[Field, ForeignObjectRel],
+    is_input=False,
+    is_filter=False,
 ):
     if isinstance(model_field, ForeignObjectRel):
         return model_field.get_accessor_name()
+
     if is_input and not is_filter:
         return model_field.attname
-    else:
-        return model_field.name
+
+    return model_field.name
 
 
 def get_model_field(model: Type[Model], field_name: str):
     try:
         return model._meta.get_field(field_name)
     except django.core.exceptions.FieldDoesNotExist as e:
         model_field_names = []
@@ -242,18 +249,19 @@
             model_field_name = resolve_model_field_name(field)
             if field_name == model_field_name:
                 return field
             model_field_names.append(model_field_name)
 
         e.args = (
             "{}, did you mean {}?".format(
-                e.args[0], ", ".join([f"'{n}'" for n in model_field_names])
+                e.args[0],
+                ", ".join([f"'{n}'" for n in model_field_names]),
             ),
         )
-        raise e
+        raise
 
 
 def is_auto(type_):
     return isinstance(type_, StrawberryAuto)
 
 
 def is_optional(model_field, is_input, partial):
```

### Comparing `strawberry_graphql_django-0.9.4/strawberry_django/filters.py` & `strawberry_graphql_django-0.9.5/strawberry_django/filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,55 @@
+from __future__ import annotations
+
 import functools
 import inspect
 from enum import Enum
-from types import FunctionType
-from typing import Generic, List, Optional, Type, TypeVar
+from typing import TYPE_CHECKING, Generic, List, TypeVar
 
 import strawberry
-from django.db.models import QuerySet
 from django.db.models.sql.query import get_field_names_from_opts
 from strawberry import UNSET
-from strawberry.arguments import StrawberryArgument
-from strawberry.types import Info
 
 from . import utils
 from .arguments import argument
 
+if TYPE_CHECKING:
+    from types import FunctionType
+
+    from django.db.models import QuerySet
+    from strawberry.arguments import StrawberryArgument
+    from strawberry.types import Info
 
 T = TypeVar("T")
 
 
 @strawberry.input
 class DjangoModelFilterInput:
     pk: strawberry.ID
 
 
 @strawberry.input
 class FilterLookup(Generic[T]):
-    exact: Optional[T] = UNSET
-    i_exact: Optional[T] = UNSET
-    contains: Optional[T] = UNSET
-    i_contains: Optional[T] = UNSET
-    in_list: Optional[List[T]] = UNSET
-    gt: Optional[T] = UNSET
-    gte: Optional[T] = UNSET
-    lt: Optional[T] = UNSET
-    lte: Optional[T] = UNSET
-    starts_with: Optional[T] = UNSET
-    i_starts_with: Optional[T] = UNSET
-    ends_with: Optional[T] = UNSET
-    i_ends_with: Optional[T] = UNSET
-    range: Optional[List[T]] = UNSET
-    is_null: Optional[bool] = UNSET
-    regex: Optional[str] = UNSET
-    i_regex: Optional[str] = UNSET
+    exact: T | None = UNSET
+    i_exact: T | None = UNSET
+    contains: T | None = UNSET
+    i_contains: T | None = UNSET
+    in_list: List[T] | None = UNSET  # noqa: UP006
+    gt: T | None = UNSET
+    gte: T | None = UNSET
+    lt: T | None = UNSET
+    lte: T | None = UNSET
+    starts_with: T | None = UNSET
+    i_starts_with: T | None = UNSET
+    ends_with: T | None = UNSET
+    i_ends_with: T | None = UNSET
+    range: List[T] | None = UNSET  # noqa: A003,UP006
+    is_null: bool | None = UNSET
+    regex: str | None = UNSET
+    i_regex: str | None = UNSET
 
 
 lookup_name_conversion_map = {
     "i_exact": "iexact",
     "i_contains": "icontains",
     "in_list": "in",
     "starts_with": "startswith",
@@ -53,23 +57,26 @@
     "ends_with": "endswith",
     "i_ends_with": "iendswith",
     "is_null": "isnull",
     "i_regex": "iregex",
 }
 
 
-def filter(model, *, name=None, lookups=False):
+def filter(model, *, name=None, lookups=False):  # noqa: A001
     def wrapper(cls):
-        is_filter = lookups and "lookups" or True
         from .type import process_type
 
-        type_ = process_type(
-            cls, model, is_input=True, partial=True, is_filter=is_filter
+        is_filter = "lookups" if lookups else True
+        return process_type(
+            cls,
+            model,
+            is_input=True,
+            partial=True,
+            is_filter=is_filter,
         )
-        return type_
 
     return wrapper
 
 
 def filter_deprecated(model, *, name=None, lookups=False):
     utils.deprecated(
         (
@@ -96,45 +103,50 @@
             field_value = field_value.value
 
         filter_method = getattr(filters, f"filter_{field_name}", None)
         if filter_method:
             filter_methods.append(filter_method)
             continue
 
-        if django_model:
-            if field_name not in get_field_names_from_opts(django_model._meta):
-                continue
+        if django_model and field_name not in get_field_names_from_opts(
+            django_model._meta,
+        ):
+            continue
 
         if field_name in lookup_name_conversion_map:
             field_name = lookup_name_conversion_map[field_name]
         if utils.is_strawberry_type(field_value):
             (
                 subfield_filter_kwargs,
                 subfield_filter_methods,
             ) = build_filter_kwargs(field_value)
             for (
                 subfield_name,
                 subfield_value,
             ) in subfield_filter_kwargs.items():
-                if isinstance(subfield_value, Enum):
-                    subfield_value = subfield_value.value
-                filter_kwargs[f"{field_name}__{subfield_name}"] = subfield_value
+                filter_kwargs[f"{field_name}__{subfield_name}"] = (
+                    subfield_value.value
+                    if isinstance(subfield_value, Enum)
+                    else subfield_value
+                )
             filter_methods.extend(subfield_filter_methods)
         else:
             filter_kwargs[field_name] = field_value
 
     return filter_kwargs, filter_methods
 
 
 @functools.lru_cache(maxsize=256)
 def function_allow_passing_info(filter_method: FunctionType) -> bool:
     argspec = inspect.getfullargspec(filter_method)
 
     return "info" in getattr(argspec, "args", []) or "info" in getattr(
-        argspec, "kwargs", []
+        argspec,
+        "kwargs",
+        [],
     )
 
 
 def apply(filters, queryset: QuerySet, info=UNSET, pk=UNSET) -> QuerySet:
     if pk is not UNSET:
         queryset = queryset.filter(pk=pk)
 
@@ -146,43 +158,41 @@
     ):
         return queryset
 
     filter_method = getattr(filters, "filter", None)
     if filter_method:
         if function_allow_passing_info(
             # Pass the original __func__ which is always the same
-            getattr(filter_method, "__func__", filter_method)
+            getattr(filter_method, "__func__", filter_method),
         ):
             return filter_method(queryset=queryset, info=info)
 
-        else:
-            return filter_method(queryset=queryset)
+        return filter_method(queryset=queryset)
 
     filter_kwargs, filter_methods = build_filter_kwargs(filters)
     queryset = queryset.filter(**filter_kwargs)
     for filter_method in filter_methods:
         if function_allow_passing_info(
             # Pass the original __func__ which is always the same
-            getattr(filter_method, "__func__", filter_method)
+            getattr(filter_method, "__func__", filter_method),
         ):
             queryset = filter_method(queryset=queryset, info=info)
-
         else:
             queryset = filter_method(queryset=queryset)
 
     return queryset
 
 
 class StrawberryDjangoFieldFilters:
     def __init__(self, filters=UNSET, **kwargs):
         self.filters = filters
         super().__init__(**kwargs)
 
     @property
-    def arguments(self) -> List[StrawberryArgument]:
+    def arguments(self) -> list[StrawberryArgument]:
         arguments = []
         if not self.base_resolver:
             filters = self.get_filters()
             if (
                 self.django_model
                 and not self.is_list
                 and self.origin._type_definition.name == "Query"
@@ -191,26 +201,35 @@
             elif self.django_model and not self.is_list:
                 # Do not add filters to non list fields
                 pass
             elif filters and filters is not UNSET:
                 arguments.append(argument("filters", filters))
         return super().arguments + arguments
 
-    def get_filters(self) -> Optional[Type]:
+    def get_filters(self) -> type | None:
         if self.filters is not UNSET:
             return self.filters
         type_ = utils.unwrap_type(self.type or self.child.type)
 
         if utils.is_django_type(type_):
             return type_._django_type.filters
         return None
 
     def apply_filters(
-        self, queryset: QuerySet, filters: Type = UNSET, pk=UNSET, info: Info = UNSET
+        self,
+        queryset: QuerySet,
+        filters: type = UNSET,
+        pk=UNSET,
+        info: Info = UNSET,
     ) -> QuerySet:
         return apply(filters, queryset, info, pk)
 
     def get_queryset(
-        self, queryset: QuerySet, info: Info, pk=UNSET, filters: Type = UNSET, **kwargs
+        self,
+        queryset: QuerySet,
+        info: Info,
+        pk=UNSET,
+        filters: type = UNSET,
+        **kwargs,
     ):
         queryset = super().get_queryset(queryset, info, **kwargs)
         return self.apply_filters(queryset, filters, pk, info)
```

### Comparing `strawberry_graphql_django-0.9.4/strawberry_django/hooks.py` & `strawberry_graphql_django-0.9.5/strawberry_django/hooks.py`

 * *Files identical despite different names*

### Comparing `strawberry_graphql_django-0.9.4/strawberry_django/middlewares/debug_toolbar.py` & `strawberry_graphql_django-0.9.5/strawberry_django/middlewares/debug_toolbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 import json
 import weakref
 from typing import Optional
 
 from asgiref.sync import sync_to_async
 from debug_toolbar.middleware import (
     _HTML_TYPES,
-    DebugToolbarMiddleware as _DebugToolbarMiddleware,
     show_toolbar,
 )
+from debug_toolbar.middleware import (
+    DebugToolbarMiddleware as _DebugToolbarMiddleware,
+)
 from debug_toolbar.panels.sql.panel import SQLPanel
 from debug_toolbar.panels.templates import TemplatesPanel
 from debug_toolbar.toolbar import DebugToolbar
 from django.core.exceptions import SynchronousOnlyOperation
 from django.core.serializers.json import DjangoJSONEncoder
 from django.http.request import HttpRequest
 from django.http.response import HttpResponse
 from django.template.loader import render_to_string
 from django.utils.encoding import force_str
 from strawberry.django.views import BaseView
 
-
 _store_cache = weakref.WeakKeyDictionary()
 _debug_toolbar_map: "weakref.WeakKeyDictionary[HttpRequest, DebugToolbar]" = (
     weakref.WeakKeyDictionary()
 )
 
 _original_store = DebugToolbar.store
 _original_debug_toolbar_init = DebugToolbar.__init__
@@ -72,15 +73,15 @@
     toolbar: Optional[DebugToolbar] = DebugToolbar.fetch(store_id)
     if not toolbar:
         return None
 
     content = force_str(response.content, encoding=response.charset)
     payload = json.loads(content, object_pairs_hook=collections.OrderedDict)
     payload["debugToolbar"] = collections.OrderedDict(
-        [("panels", collections.OrderedDict())]
+        [("panels", collections.OrderedDict())],
     )
     payload["debugToolbar"]["storeId"] = toolbar.store_id
 
     for p in reversed(toolbar.enabled_panels):
         if p.panel_id == "TemplatesPanel":
             continue
 
@@ -146,28 +147,28 @@
         return self.process_request(request)
 
     async def __acall__(self, request: HttpRequest):
         if _is_websocket(request):
             return await self._original_get_response(request)
 
         return await sync_to_async(self.process_request, thread_sensitive=False)(
-            request
+            request,
         )
 
     def process_request(self, request: HttpRequest):
         response = super().__call__(request)
 
         if not show_toolbar(request) or DebugToolbar.is_toolbar_request(request):
             return response
 
         content_type = response.get("Content-Type", "").split(";")[0]
         is_html = content_type in _HTML_TYPES
         is_graphiql = getattr(request, "_is_graphiql", False)
 
-        if is_html and is_graphiql and response.status_code == 200:
+        if is_html and is_graphiql and response.status_code == 200:  # noqa: PLR2004
             template = render_to_string("strawberry_django/debug_toolbar.html")
             response.write(template)
             if "Content-Length" in response:
                 response["Content-Length"] = len(response.content)
 
         if is_html or not is_graphiql or content_type != "application/json":
             return response
```

### Comparing `strawberry_graphql_django-0.9.4/strawberry_django/mutations/fields.py` & `strawberry_graphql_django-0.9.5/strawberry_django/mutations/fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,29 +2,36 @@
 
 from django.db import transaction
 from strawberry import UNSET
 from strawberry.annotation import StrawberryAnnotation
 from strawberry.arguments import StrawberryArgument
 from strawberry.type import StrawberryList, StrawberryOptional
 
-from .. import utils
-from ..fields.field import (
+from strawberry_django import utils
+from strawberry_django.fields.field import (
     StrawberryDjangoFieldBase,
     StrawberryDjangoFieldFilters,
     StrawberryField,
 )
-from ..fields.types import ManyToManyInput, ManyToOneInput, OneToManyInput
-from ..resolvers import django_resolver
+from strawberry_django.fields.types import (
+    ManyToManyInput,
+    ManyToOneInput,
+    OneToManyInput,
+)
+from strawberry_django.resolvers import django_resolver
 
 
 class DjangoMutationBase:
     def __init__(self, input_type, **kwargs):
         self.input_type = input_type
         super().__init__(
-            graphql_name=None, python_name=None, type_annotation=None, **kwargs
+            graphql_name=None,
+            python_name=None,
+            type_annotation=None,
+            **kwargs,
         )
 
     @property
     def is_optional(self):
         return isinstance(self.type, StrawberryOptional)
 
     @property
@@ -33,51 +40,54 @@
             self.is_optional and isinstance(self.type.of_type, StrawberryList)
         )
 
     @property
     def arguments(self):
         if self.input_type:
             assert self.django_model == utils.get_django_model(
-                self.input_type
+                self.input_type,
             ), "Input and output types should be from the same Django model"
 
         arguments = []
         if self.input_type:
             is_list = self.is_list and isinstance(self, DjangoCreateMutation)
             arguments.append(get_argument("data", self.input_type, is_list))
         return arguments + super().arguments
 
     @django_resolver
     def get_result(self, source, info, args, kwargs):
-        return self.resolver(info=info, source=source, *args, **kwargs)
+        return self.resolver(info, source, *args, **kwargs)
 
     @property
     def is_basic_field(self) -> bool:
-        """
-        Since all mutations define a resolver function they are never basic
-        fields so always return False here.
+        """Mark this field as not basic.
+
+        All StrawberryDjango fields define a custom resolver that needs to be
+        run, so always return False here.
         """
         return False
 
 
 class DjangoCreateMutation(
-    DjangoMutationBase, StrawberryDjangoFieldBase, StrawberryField
+    DjangoMutationBase,
+    StrawberryDjangoFieldBase,
+    StrawberryField,
 ):
     def create(self, data):
         input_data = get_input_data(self.input_type, data)
         instance = self.django_model.objects.create(**input_data)
         update_m2m([instance], data)
         return instance
 
     @transaction.atomic
     def resolver(self, info, source, data):
         if self.is_list:
             return [self.create(d) for d in data]
-        else:
-            return self.create(data)
+
+        return self.create(data)
 
 
 class DjangoUpdateMutation(
     DjangoMutationBase,
     StrawberryDjangoFieldFilters,
     StrawberryDjangoFieldBase,
     StrawberryField,
@@ -104,26 +114,20 @@
         queryset = self.get_queryset(queryset=queryset, info=info, **kwargs)
         instances = list(queryset)
         queryset.delete()
         return instances
 
 
 def get_argument(name, type_, is_list=False):
-    if is_list:
-        return StrawberryArgument(
-            python_name=name,
-            graphql_name=name,
-            type_annotation=StrawberryAnnotation(List[type_]),
-        )
-    else:
-        return StrawberryArgument(
-            python_name=name,
-            graphql_name=name,
-            type_annotation=StrawberryAnnotation(type_),
-        )
+    annotation = StrawberryAnnotation(List[type_] if is_list else type_)
+    return StrawberryArgument(
+        python_name=name,
+        graphql_name=name,
+        type_annotation=annotation,
+    )
 
 
 def get_input_data(input_type, data):
     input_data = {}
     for field in input_type._type_definition.fields:
         value = getattr(data, field.name)
         if isinstance(value, (ManyToOneInput, ManyToManyInput)):
```

### Comparing `strawberry_graphql_django-0.9.4/strawberry_django/mutations/mutations.py` & `strawberry_graphql_django-0.9.5/strawberry_django/mutations/mutations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from typing import Any
 
 from strawberry import UNSET
 
 from .fields import DjangoCreateMutation, DjangoDeleteMutation, DjangoUpdateMutation
 
 
-def create(input_type=UNSET, permission_classes=[], **kwargs) -> Any:
+# FIXME: This needs proper typing
+def create(input_type=UNSET, permission_classes=None, **kwargs) -> Any:
     return DjangoCreateMutation(
-        input_type, permission_classes=permission_classes, **kwargs
+        input_type,
+        permission_classes=permission_classes or [],
+        **kwargs,
     )
 
 
-def update(input_type=UNSET, filters=UNSET, permission_classes=[], **kwargs) -> Any:
+def update(input_type=UNSET, filters=UNSET, permission_classes=None, **kwargs) -> Any:
     return DjangoUpdateMutation(
-        input_type, filters=filters, permission_classes=permission_classes, **kwargs
+        input_type,
+        filters=filters,
+        permission_classes=permission_classes or [],
+        **kwargs,
     )
 
 
-def delete(filters=UNSET, permission_classes=[], **kwargs) -> Any:
+def delete(filters=UNSET, permission_classes=None, **kwargs) -> Any:
     return DjangoDeleteMutation(
         input_type=None,
         filters=filters,
-        permission_classes=permission_classes,
+        permission_classes=permission_classes or [],
         **kwargs,
     )
```

### Comparing `strawberry_graphql_django-0.9.4/strawberry_django/ordering.py` & `strawberry_graphql_django-0.9.5/strawberry_django/ordering.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+from __future__ import annotations
+
 import enum
-from typing import List, Optional, Type
+from typing import TYPE_CHECKING, Optional
 
 import strawberry
-from django.db.models import QuerySet
 from strawberry import UNSET
-from strawberry.arguments import StrawberryArgument
 from strawberry.auto import StrawberryAuto
-from strawberry.types import Info
 
 from strawberry_django.utils import fields
 
 from . import utils
 from .arguments import argument
 
+if TYPE_CHECKING:
+    from django.db.models import QuerySet
+    from strawberry.arguments import StrawberryArgument
+    from strawberry.types import Info
+
 
 @strawberry.enum
 class Ordering(enum.Enum):
     ASC = "ASC"
     DESC = "DESC"
 
 
@@ -35,17 +39,17 @@
             args.extend(subargs)
     return args
 
 
 def order(model):
     def wrapper(cls):
         for name, type_ in cls.__annotations__.items():
-            if isinstance(type_, StrawberryAuto):
-                type_ = Ordering
-            cls.__annotations__[name] = Optional[type_]
+            cls.__annotations__[name] = Optional[
+                Ordering if isinstance(type_, StrawberryAuto) else type_
+            ]
             setattr(cls, name, UNSET)
         return strawberry.input(cls)
 
     return wrapper
 
 
 def apply(order, queryset: QuerySet) -> QuerySet:
@@ -59,32 +63,36 @@
 
 class StrawberryDjangoFieldOrdering:
     def __init__(self, order=UNSET, **kwargs):
         self.order = order
         super().__init__(**kwargs)
 
     @property
-    def arguments(self) -> List[StrawberryArgument]:
+    def arguments(self) -> list[StrawberryArgument]:
         arguments = []
         if not self.base_resolver:
             order = self.get_order()
             if order and order is not UNSET and self.is_list:
                 arguments.append(argument("order", order))
         return super().arguments + arguments
 
-    def get_order(self) -> Optional[Type]:
+    def get_order(self) -> type | None:
         if self.order is not UNSET:
             return self.order
         type_ = utils.unwrap_type(self.type or self.child.type)
 
         if utils.is_django_type(type_):
             return type_._django_type.order
         return None
 
     def apply_order(self, queryset: QuerySet, order) -> QuerySet:
         return apply(order, queryset)
 
     def get_queryset(
-        self, queryset: QuerySet, info: Info, order: Type = UNSET, **kwargs
+        self,
+        queryset: QuerySet,
+        info: Info,
+        order: type = UNSET,
+        **kwargs,
     ):
         queryset = super().get_queryset(queryset, info, **kwargs)
         return self.apply_order(queryset, order)
```

### Comparing `strawberry_graphql_django-0.9.4/strawberry_django/pagination.py` & `strawberry_graphql_django-0.9.5/strawberry_django/pagination.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-from typing import List, Optional, Type
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
 import strawberry
-from django.db.models import QuerySet
 from strawberry import UNSET
-from strawberry.arguments import StrawberryArgument
-from strawberry.types import Info
 
 from . import utils
 from .arguments import argument
 
+if TYPE_CHECKING:
+    from django.db.models import QuerySet
+    from strawberry.arguments import StrawberryArgument
+    from strawberry.types import Info
+
 
 @strawberry.input
 class OffsetPaginationInput:
     offset: int = 0
     limit: int = -1
 
 
@@ -27,32 +31,36 @@
 
 class StrawberryDjangoPagination:
     def __init__(self, pagination=UNSET, **kwargs):
         self.pagination = pagination
         super().__init__(**kwargs)
 
     @property
-    def arguments(self) -> List[StrawberryArgument]:
+    def arguments(self) -> list[StrawberryArgument]:
         arguments = []
         if not self.base_resolver:
             pagination = self.get_pagination()
             if pagination and pagination is not UNSET:
                 arguments.append(argument("pagination", OffsetPaginationInput))
         return super().arguments + arguments
 
-    def get_pagination(self) -> Optional[Type]:
+    def get_pagination(self) -> type | None:
         if self.pagination is not UNSET:
             return self.pagination
 
         type_ = utils.unwrap_type(self.type or self.child.type)
         if utils.is_django_type(type_):
             return type_._django_type.pagination
         return None
 
     def apply_pagination(self, queryset: QuerySet, pagination=UNSET):
         return apply(pagination, queryset)
 
     def get_queryset(
-        self, queryset: QuerySet, info: Info, pagination: Type = UNSET, **kwargs
+        self,
+        queryset: QuerySet,
+        info: Info,
+        pagination: type = UNSET,
+        **kwargs,
     ):
         queryset = super().get_queryset(queryset, info, **kwargs)
         return self.apply_pagination(queryset, pagination)
```

### Comparing `strawberry_graphql_django-0.9.4/strawberry_django/resolvers.py` & `strawberry_graphql_django-0.9.5/strawberry_django/resolvers.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,41 +4,41 @@
 from asgiref.sync import sync_to_async
 from django.db import models
 
 from . import utils
 
 
 def django_resolver(resolver):
-    """This decorator is used to make sure that resolver is always called from
+    """Django resolver for handling both sync and async.
+
+    This decorator is used to make sure that resolver is always called from
     sync context.  sync_to_async helper in used if function is called from
     async context. This is useful especially with Django ORM, which does not
     support async. Coroutines are not wrapped.
     """
-
     if inspect.iscoroutinefunction(resolver) or inspect.isasyncgenfunction(resolver):
         return resolver
 
     @functools.wraps(resolver)
     def wrapper(*args, **kwargs):
         if utils.is_async():
             return call_sync_resolver(resolver, *args, **kwargs)
-        else:
-            return resolver(*args, **kwargs)
+
+        return resolver(*args, **kwargs)
 
     return wrapper
 
 
 def sync_to_async_thread_sensitive(func):
     # django 3.0 defaults to thread_sensitive=False
     return sync_to_async(func, thread_sensitive=True)
 
 
 @sync_to_async_thread_sensitive
 def call_sync_resolver(resolver, *args, **kwargs):
-    """This function executes resolver function in sync context and ensures
+    """Safe resolve a sync resolver.
+
+    This function executes resolver function in sync context and ensures
     that querysets are executed.
     """
-
     result = resolver(*args, **kwargs)
-    if isinstance(result, models.QuerySet):
-        result = list(result)
-    return result
+    return list(result) if isinstance(result, models.QuerySet) else result
```

### Comparing `strawberry_graphql_django-0.9.4/strawberry_django/settings.py` & `strawberry_graphql_django-0.9.5/strawberry_django/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-"""
-Code for interacting with Django settings.
-"""
+"""Code for interacting with Django settings."""
 try:
     from typing import TypedDict
 except ImportError:
     from typing_extensions import TypedDict
 
 from django.conf import settings
 
 
 class StrawberryDjangoSettings(TypedDict):
-    """
-    Dictionary defining the shape `settings.STRAWBERRY_DJANGO` should have.
+    """Dictionary defining the shape `settings.STRAWBERRY_DJANGO` should have.
 
     All settings are optional and have defaults as described in their docstrings and
     defined in `DEFAULT_DJANGO_SETTINGS`.
     """
 
     FIELD_DESCRIPTION_FROM_HELP_TEXT: bool
     """(Default: False) If True, field descriptions will be fetched from the
@@ -29,16 +26,16 @@
 DEFAULT_DJANGO_SETTINGS = StrawberryDjangoSettings(
     FIELD_DESCRIPTION_FROM_HELP_TEXT=False,
     TYPE_DESCRIPTION_FROM_MODEL_DOCSTRING=False,
 )
 
 
 def strawberry_django_settings() -> StrawberryDjangoSettings:
-    """
-    Return the dictionary from `settings.STRAWBERRY_DJANGO`, with defaults for missing
-    keys.
+    """Get strawberry django settings.
+
+    Return the dictionary from `settings.STRAWBERRY_DJANGO`, with defaults
+    for missing keys.
 
     Preferred to direct access for the type hints and defaults.
     """
     defaults = DEFAULT_DJANGO_SETTINGS
-    customized = {**defaults, **getattr(settings, "STRAWBERRY_DJANGO", {})}
-    return customized
+    return {**defaults, **getattr(settings, "STRAWBERRY_DJANGO", {})}
```

### Comparing `strawberry_graphql_django-0.9.4/strawberry_django/templates/strawberry_django/debug_toolbar.html` & `strawberry_graphql_django-0.9.5/strawberry_django/templates/strawberry_django/debug_toolbar.html`

 * *Files identical despite different names*

### Comparing `strawberry_graphql_django-0.9.4/strawberry_django/type.py` & `strawberry_graphql_django-0.9.5/strawberry_django/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dataclasses
 from contextlib import suppress
-from inspect import cleandoc
+from inspect import cleandoc, ismethod
 from typing import Any, Dict, Generic, Optional, Type, TypeVar
 
 import django
 import django.db.models
 import strawberry
 from strawberry import UNSET
 from strawberry.annotation import StrawberryAnnotation
@@ -18,22 +18,21 @@
     get_model_field,
     is_optional,
     resolve_model_field_name,
     resolve_model_field_type,
 )
 from .settings import strawberry_django_settings as django_settings
 
-
 _type = type
 
 
 def get_type_attr(type_, field_name: str):
     attr = getattr(type_, field_name, UNSET)
-    if attr is UNSET:
-        attr = getattr(type_, "__dataclass_fields__", {}).get(field_name, UNSET)
+    if attr is UNSET or ismethod(attr):
+        return getattr(type_, "__dataclass_fields__", {}).get(field_name, attr)
     return attr
 
 
 def get_field(
     django_type: "StrawberryDjangoType",
     field_name: str,
     field_annotation: Optional[StrawberryAnnotation] = None,
@@ -62,58 +61,62 @@
 
     try:
         # resolve the django_name and check if it is relation field. django_name
         # is used to access the field data in resolvers
         django_name = field.django_name or field_name
         model_field = get_model_field(django_type.model, django_name)
         field.django_name = resolve_model_field_name(
-            model_field, django_type.is_input, django_type.is_filter
+            model_field,
+            django_type.is_input,
+            django_type.is_filter,
         )
         field.is_relation = model_field.is_relation
 
         # Use the Django field help_text if no other description is available.
         settings = django_settings()
         if not field.description and settings["FIELD_DESCRIPTION_FROM_HELP_TEXT"]:
             model_field_help_text = getattr(model_field, "help_text", "")
             field.description = str(model_field_help_text) or None
     except django.core.exceptions.FieldDoesNotExist:
         if field.django_name or field.is_auto:
             raise  # field should exist, reraise caught exception
         model_field = None
 
-    if field.is_relation:
-        # change relation field type to auto if field is inherited from another
-        # type. for example if field is inherited from output type but we are
-        # configuring field for input type
-        if not utils.is_similar_django_type(django_type, field.origin_django_type):
-            field.is_auto = True
+    # change relation field type to auto if field is inherited from another
+    # type. for example if field is inherited from output type but we are
+    # configuring field for input type
+    if field.is_relation and not utils.is_similar_django_type(
+        django_type,
+        field.origin_django_type,
+    ):
+        field.is_auto = True
 
     # Only set the type_annotation for auto fields if they don't have a base_resolver.
     # Since strawberry 0.139 the type_annotation has a higher priority than the
     # resolver's annotation, and that would force our automatic model resolution to be
     # used instead of the resolver's type annotation.
     if field.is_auto and not field.base_resolver:
         # resolve type of auto field
         field_type = resolve_model_field_type(model_field, django_type)
         field.type_annotation = StrawberryAnnotation(field_type)
 
     if field.type_annotation and is_optional(
-        model_field, django_type.is_input, django_type.is_partial
+        model_field,
+        django_type.is_input,
+        django_type.is_partial,
     ):
         field.type_annotation.annotation = Optional[field.type_annotation.annotation]
 
-    if django_type.is_input:
-        if field.default is dataclasses.MISSING:
-            # strawberry converts UNSET value to MISSING, let's set
-            # it back to UNSET. this is important especially for partial
-            # input types
-            # TODO: could strawberry support UNSET default value?
-            field.default_value = UNSET
-            field.default = UNSET
-
+    if django_type.is_input and field.default is dataclasses.MISSING:
+        # strawberry converts UNSET value to MISSING, let's set
+        # it back to UNSET. this is important especially for partial
+        # input types
+        # TODO: could strawberry support UNSET default value?
+        field.default_value = UNSET
+        field.default = UNSET
     return field
 
 
 def get_fields(django_type: "StrawberryDjangoType"):
     annotations = utils.get_annotations(django_type.origin)
     fields: Dict[str, StrawberryDjangoField] = {}
     seen_fields = set()
@@ -221,20 +224,23 @@
     # restore original annotations for further use
     cls.__annotations__ = original_annotations
     cls._django_type = django_type
 
     return cls
 
 
-def type(model, *, filters=UNSET, **kwargs):
+# FIXME: This needs proper typing
+def type(model, *, filters=UNSET, **kwargs):  # noqa: A001
     def wrapper(cls):
         return process_type(cls, model, filters=filters, **kwargs)
 
     return wrapper
 
 
-def input(model, *, partial=False, **kwargs):
+# FIXME: This needs proper typing
+def input(model, *, partial=False, **kwargs):  # noqa: A001
     return type(model, partial=partial, is_input=True, **kwargs)
 
 
+# FIXME: This needs proper typing
 def mutation(model, **kwargs):
     return type(model, **kwargs)
```

### Comparing `strawberry_graphql_django-0.9.4/strawberry_django/utils.py` & `strawberry_graphql_django-0.9.5/strawberry_django/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import asyncio
 import dataclasses
 import sys
 import warnings
-from typing import Dict
+from typing import ClassVar, Dict
 
 from django.db import models
 from strawberry.annotation import StrawberryAnnotation
 from strawberry.field import StrawberryField
 from strawberry.type import StrawberryContainer
 
-
 __all__ = ["deprecated"]
 
 
 def is_async() -> bool:
     # django uses the same method to detect async operation
     # https://github.com/django/django/blob/bb076476cf560b988f8d80dbbc4a3c85df54b1b9/django/utils/asyncio.py
     try:
@@ -68,38 +67,50 @@
     from .fields.types import is_auto
 
     return is_auto(obj)
 
 
 def get_django_model(type_):
     if not is_django_type(type_):
-        return
+        return None
     return type_._django_type.model
 
 
 def is_similar_django_type(a, b):
     if not a or not b:
         return False
     if a.is_input != b.is_input:
         return False
     if a.is_filter != b.is_filter:
         return False
     return True
 
 
+# dirty workaround, but similar to the one of dataclasses
+# it would be better to use dataclasses.fields
+def _is_classvar(annotation, namespace):
+    if isinstance(annotation, str):
+        if annotation.startswith("ClassVar["):
+            annotation = namespace["ClassVar"]
+        elif annotation.startswith("typing.ClassVar["):
+            annotation = namespace["typing"].ClassVar
+    return annotation is ClassVar
+
+
 def get_annotations(cls):
     annotations: Dict[str, StrawberryAnnotation] = {}
-    namespace = sys.modules[cls.__module__].__dict__
     for c in reversed(cls.__mro__):
+        namespace = sys.modules[c.__module__].__dict__
         if "__annotations__" in c.__dict__:
             annotations.update(
                 {
                     k: StrawberryAnnotation(v, namespace=namespace)
                     for k, v in c.__annotations__.items()
-                }
+                    if not _is_classvar(v, namespace)
+                },
             )
     return annotations
 
 
 def unwrap_type(type_):
     while isinstance(type_, StrawberryContainer):
         type_ = type_.of_type
```

### Comparing `strawberry_graphql_django-0.9.4/PKG-INFO` & `strawberry_graphql_django-0.9.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 Metadata-Version: 2.1
 Name: strawberry-graphql-django
-Version: 0.9.4
+Version: 0.9.5
 Summary: Strawberry GraphQL Django extension
 Home-page: https://github.com/strawberry-graphql/strawberry-graphql-django
 License: MIT
 Keywords: graphql,api,django
 Author: Lauri Hintsala
 Author-email: lauri.hintsala@verkkopaja.fi
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: debug-toolbar
 Requires-Dist: Django (>=3.2)
 Requires-Dist: django-debug-toolbar (>=3.4) ; extra == "debug-toolbar"
-Requires-Dist: strawberry-graphql (>=0.160.0)
+Requires-Dist: strawberry-graphql (>=0.184.0)
 Project-URL: Repository, https://github.com/strawberry-graphql/strawberry-graphql-django
 Description-Content-Type: text/markdown
 
 # Strawberry GraphQL Django integration
 
 [![CI](https://github.com/la4de/strawberry-graphql-django/actions/workflows/main.yml/badge.svg)](https://github.com/la4de/strawberry-graphql-django/actions/workflows/main.yml)
 [![PyPI](https://img.shields.io/pypi/v/strawberry-graphql-django)](https://pypi.org/project/strawberry-graphql-django/)
```

