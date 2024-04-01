# Comparing `tmp/django_json_model_field-0.0.1rc8.tar.gz` & `tmp/django_json_model_field-0.0.1rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_json_model_field-0.0.1rc8.tar", max compression
+gzip compressed data, was "django_json_model_field-0.0.1rc9.tar", max compression
```

## Comparing `django_json_model_field-0.0.1rc8.tar` & `django_json_model_field-0.0.1rc9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0        0 2022-04-12 21:26:22.508669 django_json_model_field-0.0.1rc8/django_json_model_field/__init__.py
--rw-r--r--   0        0        0        0 2022-04-12 21:26:22.534000 django_json_model_field-0.0.1rc8/django_json_model_field/db/__init__.py
--rw-r--r--   0        0        0      201 2022-05-03 15:50:55.742337 django_json_model_field-0.0.1rc8/django_json_model_field/db/models/__init__.py
--rw-r--r--   0        0        0    11543 2022-05-03 15:50:55.743298 django_json_model_field-0.0.1rc8/django_json_model_field/db/models/base_json_model_field.py
--rw-r--r--   0        0        0     4789 2022-05-03 15:50:55.743874 django_json_model_field-0.0.1rc8/django_json_model_field/db/models/conditional_json_model_attribute.py
--rw-r--r--   0        0        0    10910 2022-05-03 15:50:55.744295 django_json_model_field-0.0.1rc8/django_json_model_field/db/models/conditional_json_model_field.py
--rw-r--r--   0        0        0    13616 2022-05-03 15:50:55.745711 django_json_model_field-0.0.1rc8/django_json_model_field/db/models/json_model.py
--rw-r--r--   0        0        0     2250 2022-05-03 15:50:55.746342 django_json_model_field-0.0.1rc8/django_json_model_field/db/models/json_model_field.py
--rw-r--r--   0        0        0     9614 2022-05-03 15:50:55.747064 django_json_model_field-0.0.1rc8/django_json_model_field/db/models/json_model_options.py
--rw-r--r--   0        0        0      222 2022-05-03 15:50:55.747678 django_json_model_field-0.0.1rc8/django_json_model_field/forms/__init__.py
--rw-r--r--   0        0        0     7724 2022-05-03 15:50:55.748434 django_json_model_field-0.0.1rc8/django_json_model_field/forms/nested_form_field.py
--rw-r--r--   0        0        0    12215 2022-05-03 15:50:55.749101 django_json_model_field-0.0.1rc8/django_json_model_field/forms/nested_model_form_field.py
--rw-r--r--   0        0        0     2859 2022-05-03 15:50:55.749434 django_json_model_field-0.0.1rc8/django_json_model_field/forms/widgets.py
--rw-r--r--   0        0        0      134 2022-05-03 15:50:55.750160 django_json_model_field-0.0.1rc8/django_json_model_field/templates/django_json_model_field/forms/widgets/nested_form_input.html
--rw-r--r--   0        0        0      188 2022-04-12 21:26:22.517626 django_json_model_field-0.0.1rc8/django_json_model_field/util.py
--rw-r--r--   0        0        0      721 2022-05-03 15:52:05.565438 django_json_model_field-0.0.1rc8/pyproject.toml
--rw-r--r--   0        0        0      919 2022-05-03 15:52:20.724551 django_json_model_field-0.0.1rc8/setup.py
--rw-r--r--   0        0        0      480 2022-05-03 15:52:20.724763 django_json_model_field-0.0.1rc8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-12 20:21:14.525602 django_json_model_field-0.0.1rc9/django_json_model_field/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-13 13:40:27.243250 django_json_model_field-0.0.1rc9/django_json_model_field/apps.py
+-rw-r--r--   0        0        0        0 2022-05-23 10:04:59.000000 django_json_model_field-0.0.1rc9/django_json_model_field/db/__init__.py
+-rw-r--r--   0        0        0      201 2023-04-12 20:20:36.134890 django_json_model_field-0.0.1rc9/django_json_model_field/db/models/__init__.py
+-rw-r--r--   0        0        0    11557 2023-04-13 14:20:30.127417 django_json_model_field-0.0.1rc9/django_json_model_field/db/models/base_json_model_field.py
+-rw-r--r--   0        0        0     4789 2023-04-12 20:20:36.135545 django_json_model_field-0.0.1rc9/django_json_model_field/db/models/conditional_json_model_attribute.py
+-rw-r--r--   0        0        0    10910 2023-04-12 20:20:36.135837 django_json_model_field-0.0.1rc9/django_json_model_field/db/models/conditional_json_model_field.py
+-rw-r--r--   0        0        0    14982 2023-04-13 15:34:27.467409 django_json_model_field-0.0.1rc9/django_json_model_field/db/models/json_model.py
+-rw-r--r--   0        0        0     2250 2023-04-12 20:20:36.136519 django_json_model_field-0.0.1rc9/django_json_model_field/db/models/json_model_field.py
+-rw-r--r--   0        0        0     9866 2023-04-13 14:29:29.094715 django_json_model_field-0.0.1rc9/django_json_model_field/db/models/json_model_options.py
+-rw-r--r--   0        0        0      222 2023-04-12 20:20:40.690115 django_json_model_field-0.0.1rc9/django_json_model_field/forms/__init__.py
+-rw-r--r--   0        0        0     7724 2023-04-12 20:20:40.690564 django_json_model_field-0.0.1rc9/django_json_model_field/forms/nested_form_field.py
+-rw-r--r--   0        0        0    12215 2023-04-12 20:20:40.690980 django_json_model_field-0.0.1rc9/django_json_model_field/forms/nested_model_form_field.py
+-rw-r--r--   0        0        0     2859 2023-04-12 20:20:40.691240 django_json_model_field-0.0.1rc9/django_json_model_field/forms/widgets.py
+-rw-r--r--   0        0        0      134 2023-04-12 20:20:45.778809 django_json_model_field-0.0.1rc9/django_json_model_field/templates/django_json_model_field/forms/widgets/nested_form_input.html
+-rw-r--r--   0        0        0      188 2022-05-23 10:04:59.000000 django_json_model_field-0.0.1rc9/django_json_model_field/util.py
+-rw-r--r--   0        0        0      405 2023-04-13 16:40:50.671476 django_json_model_field-0.0.1rc9/pyproject.toml
+-rw-r--r--   0        0        0      875 2023-04-13 16:43:39.972858 django_json_model_field-0.0.1rc9/setup.py
+-rw-r--r--   0        0        0      422 2023-04-13 16:43:39.973202 django_json_model_field-0.0.1rc9/PKG-INFO
```

### Comparing `django_json_model_field-0.0.1rc8/django_json_model_field/db/models/base_json_model_field.py` & `django_json_model_field-0.0.1rc9/django_json_model_field/db/models/base_json_model_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from abc import ABCMeta, abstractmethod
 from typing import Any, Optional, TYPE_CHECKING, Type, Union
 
 from django.core import checks
 from django.core.exceptions import ValidationError
 from django.db.backends.base.base import BaseDatabaseWrapper
-from django.db.models import Field, Model
-from django_jsonfield_backport.models import JSONField
+from django.db.models import Field, JSONField, Model
 
 if TYPE_CHECKING:
     from .json_model import JSONModel
 
 
 class BaseJSONModelField(JSONField, metaclass=ABCMeta):
     """
@@ -93,15 +92,16 @@
             # nested validation errors from attempting to validate the JSONModel instance, and allows form fields
             # derived from this field to hide the messaging from this validation error in favor of showing the
             # validation errors on the individual fields for the JSONModel.
             raise ValidationError("The model contains validation errors", code="model_validation")
         self.run_validators(value)
         return value
 
-    def to_python(self, value: Optional[Union[dict, "JSONModel"]], model_instance: Model = None) -> Optional["JSONModel"]:
+    def to_python(self, value: Optional[Union[dict, "JSONModel"]], model_instance: Model = None) -> Optional[
+        "JSONModel"]:
         from django_json_model_field.db.models import JSONModel
 
         # note: signature is overridden from the base Field signature to include the model instance. This is possible
         #       since the `clean` method is also overridden to pass its model_instance argument along.
 
         # the value must either already be a JSONModel instance, or a dict that can then be converted to JSONModel
         # instance so that the field validation for that model can be checked before saving
@@ -203,14 +203,15 @@
         django/core/checks/model_checks.py). If a use case for using JSONModel classes outside a BaseJSONModelField emerges,
         this approach will need to be reconsidered.
         """
 
         errors = super().check(**kwargs)
         errors.extend(self._check_null())
         errors.extend(self._check_json_model_arguments())
+        errors.extend(self._check_json_models())
 
         return errors
 
     def _check_null(self):
         """
         Checks the `null` and `blank` arguments to make sure they are both True. To prevent duplicate errors from being
         surfaced to the end user, JSONModelFields are always nullable. Since the actual JSONModel class used to store
```

### Comparing `django_json_model_field-0.0.1rc8/django_json_model_field/db/models/conditional_json_model_attribute.py` & `django_json_model_field-0.0.1rc9/django_json_model_field/db/models/conditional_json_model_attribute.py`

 * *Files identical despite different names*

### Comparing `django_json_model_field-0.0.1rc8/django_json_model_field/db/models/conditional_json_model_field.py` & `django_json_model_field-0.0.1rc9/django_json_model_field/db/models/conditional_json_model_field.py`

 * *Files identical despite different names*

### Comparing `django_json_model_field-0.0.1rc8/django_json_model_field/db/models/json_model.py` & `django_json_model_field-0.0.1rc9/django_json_model_field/db/models/json_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from __future__ import annotations
+
 import copy
 import inspect
 from itertools import chain
 from typing import Any
 
+from django.apps import apps
+from django.core import checks
 from django.core.exceptions import FieldDoesNotExist, FieldError
-from django.db.models import Model
+from django.db.models import DateField, Field, Model
 from django.db.models.base import ModelBase
 
 from .json_model_options import JSONModelOptions
 
 
 def _has_contribute_to_class(value):
     # Only call contribute_to_class() if it's bound.
@@ -63,17 +67,32 @@
                 new_attrs[obj_name] = obj
         new_class = super_new(mcs, name, bases, new_attrs, **kwargs)
 
         abstract = getattr(attr_meta, "abstract", False)
         meta = attr_meta or getattr(new_class, "Meta", None)
         base_meta = getattr(new_class, "_meta", None)
 
-        # skipping ModelBase logic related to app_label since it's not used (Django uses it for its model registry)
+        app_label = None
+
+        # Look for an application configuration to attach the model to.
+        app_config = apps.get_containing_app_config(module)
 
-        new_class.add_to_class("_meta", JSONModelOptions(meta))
+        if getattr(meta, 'app_label', None) is None:
+            if app_config is None:
+                if not abstract:
+                    raise RuntimeError(
+                        "Model class %s.%s doesn't declare an explicit "
+                        "app_label and isn't in an application in "
+                        "INSTALLED_APPS." % (module, name)
+                    )
+
+            else:
+                app_label = app_config.label
+
+        new_class.add_to_class("_meta", JSONModelOptions(meta, app_label))
         if not abstract and base_meta and not base_meta.abstract:
             # Non-abstract child classes inherit some attributes from their
             # non-abstract parent (unless an ABC comes before it in the
             # method resolution order).
             if not hasattr(meta, "ordering"):
                 new_class._meta.ordering = base_meta.ordering
 
@@ -226,19 +245,31 @@
         replaced; if it is not replaced, it will raise an error if anything attempts to access the field's value.
 
         Parameters
         ----------
         initial
         """
 
-        # Iterate through the list of fields rather than data keys so that a None value is set for any missing fields
+        # Iterate through the list of fields rather than data keys so that the field's default value is set if there is
+        # no initial value
         for field in self._meta.fields:
-            value = field.to_python(str(initial[field.name])) if field.name in initial else field.get_default()
+            value = self._get_initial_value(field=field, initial=initial)
             setattr(self, field.name, value)
 
+    @classmethod
+    def _get_initial_value(cls, field: Field, initial: dict[str, Any]) -> Any:
+        if field.name not in initial:
+            return field.get_default()
+
+        initial_value = initial[field.name]
+        if initial_value is None or initial_value in field.empty_values:
+            return None
+
+        return field.to_python(initial_value)
+
     def _init_field_defaults(self) -> None:
         for field in self._meta.fields:
             if field.has_default():
                 setattr(self, field.name, field.get_default())
 
     def _ensure_fields_initialized(self, data: dict = None) -> None:
         """
@@ -273,14 +304,26 @@
 
         # adapted from Model._check_fields - only local fields need to be checked, no other types of fields are
         # supported
 
         errors = []
         for field in cls._meta.local_fields:
             errors.extend(field.check(**kwargs))
+            if isinstance(field, DateField):
+                errors.extend(cls._check_date_field(field))
+        return errors
+
+    @classmethod
+    def _check_date_field(cls, field: DateField):
+        errors = []
+        if field.auto_now_add:
+            errors.append(
+                checks.Critical("DateFields defined on a JSONModel cannot use auto_now_add=True", obj=field)
+            )
+
         return errors
 
     ###############################################################################################################
     # passthrough methods - these can be used as-is from Django's Model class directly rather than copy/pasting the
     # code
     ###############################################################################################################
```

### Comparing `django_json_model_field-0.0.1rc8/django_json_model_field/db/models/json_model_field.py` & `django_json_model_field-0.0.1rc9/django_json_model_field/db/models/json_model_field.py`

 * *Files identical despite different names*

### Comparing `django_json_model_field-0.0.1rc8/django_json_model_field/db/models/json_model_options.py` & `django_json_model_field-0.0.1rc9/django_json_model_field/db/models/json_model_options.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from __future__ import annotations
+
 import inspect
 from collections import OrderedDict
 from typing import TYPE_CHECKING, Type
 
 from django.core.exceptions import FieldDoesNotExist
 from django.db.models.options import Options as ModelOptions
-
 from django.utils.datastructures import ImmutableList
 from django.utils.functional import cached_property
 from django.utils.translation import override
 
 if TYPE_CHECKING:
     from .json_model import JSONModel
 
@@ -37,47 +38,55 @@
 
     Adapted from Django's Options class (imported in this module as ModelOptions for easier disambiguation)
     """
 
     FORWARD_PROPERTIES = {"fields", "concrete_fields", "local_concrete_fields", "_forward_fields_map"}
     REVERSE_PROPERTIES = {"related_objects", "fields_map", "_relation_tree"}
 
-    model: Type["JSONModel"]
+    model: Type[JSONModel]
 
     # not supported
     proxy = False
     proxy_for_model = None
 
-    def __init__(self, meta):
+    def __init__(self, meta, app_label: str):
         self._get_fields_cache = {}
         self.local_fields = []
         self.private_fields = []
         self.model_name = None
         self.verbose_name = None
         self.verbose_name_plural = None
         self.object_name = None
         self.meta = meta
         self.parents = OrderedDict()
         self.concrete_model = None
         self.ordering = []
         self._ordering_clash = False
         self.abstract = False
+        self.app_label = app_label
 
         ##########################################################################################################
         # attributes used for compatibility with Model; values are only used for conditional checks an enumeration
         ##########################################################################################################
 
-        self.app_label = None
         self.db_table = "n/a"
         self.required_db_features: tuple = ()
         self.local_many_to_many: list = []
         self.many_to_many: list = []
         self.proxy = None
         self._relation_tree = ()
 
+    @property
+    def label(self):
+        return '%s.%s' % (self.app_label, self.object_name)
+
+    @property
+    def label_lower(self):
+        return '%s.%s' % (self.app_label, self.model_name)
+
     def get_field(self, field_name):
         """
         Return a field instance given the name of a forward or reverse field.
         """
 
         # Adapted from Options.get_field to omit checks for related fields, which are not supported
 
@@ -153,14 +162,15 @@
         Return a list of all forward fields on the model and its parents,
         excluding ManyToManyFields.
 
         Private API intended only to be used by Django itself; get_fields()
         combined with filtering of field properties is the public API for
         obtaining this field list.
         """
+
         # For legacy reasons, the fields property should only contain forward
         # fields that are not private or with a m2m cardinality. Therefore we
         # pass these three filters as filters to the generator.
         # The third lambda is a longwinded way of checking f.related_model - we don't
         # use that property directly because related_model is a cached property,
         # and all the models may not have been loaded yet; we don't want to cache
         # the string reference to the related_model.
```

### Comparing `django_json_model_field-0.0.1rc8/django_json_model_field/forms/nested_form_field.py` & `django_json_model_field-0.0.1rc9/django_json_model_field/forms/nested_form_field.py`

 * *Files identical despite different names*

### Comparing `django_json_model_field-0.0.1rc8/django_json_model_field/forms/nested_model_form_field.py` & `django_json_model_field-0.0.1rc9/django_json_model_field/forms/nested_model_form_field.py`

 * *Files identical despite different names*

### Comparing `django_json_model_field-0.0.1rc8/django_json_model_field/forms/widgets.py` & `django_json_model_field-0.0.1rc9/django_json_model_field/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `django_json_model_field-0.0.1rc8/setup.py` & `django_json_model_field-0.0.1rc9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,27 +8,27 @@
  'django_json_model_field.forms']
 
 package_data = \
 {'': ['*'],
  'django_json_model_field': ['templates/django_json_model_field/forms/widgets/*']}
 
 install_requires = \
-['Django>=2.2,<3.0', 'django-jsonfield-backport>=1.0.4,<1.1.0']
+['Django>=3.2,<4.0']
 
 setup_kwargs = {
     'name': 'django-json-model-field',
-    'version': '0.0.1rc8',
+    'version': '0.0.1rc9',
     'description': 'Use a model class to provide a strict data structure for JSON fields',
     'long_description': None,
     'author': 'Daniel Schaffer',
     'author_email': 'dschaffer@instawork.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.10',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

