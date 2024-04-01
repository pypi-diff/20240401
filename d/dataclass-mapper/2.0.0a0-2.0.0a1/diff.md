# Comparing `tmp/dataclass_mapper-2.0.0a0.tar.gz` & `tmp/dataclass_mapper-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_mapper-2.0.0a0.tar", max compression
+gzip compressed data, was "dataclass_mapper-2.0.0a1.tar", max compression
```

## Comparing `dataclass_mapper-2.0.0a0.tar` & `dataclass_mapper-2.0.0a1.tar`

### file list

```diff
@@ -1,54 +1,56 @@
--rw-r--r--   0        0        0     1057 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/LICENSE.md
--rw-r--r--   0        0        0     6107 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/README.rst
--rw-r--r--   0        0        0      686 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/__init__.py
--rw-r--r--   0        0        0      849 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/classmeta.py
--rw-r--r--   0        0        0     9691 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/code_generator.py
--rw-r--r--   0        0        0     2285 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/enum.py
--rw-r--r--   0        0        0      337 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/exceptions.py
--rw-r--r--   0        0        0     1139 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/__init__.py
--rw-r--r--   0        0        0      581 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/anything_to_any.py
--rw-r--r--   0        0        0      753 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/class_to_union.py
--rw-r--r--   0        0        0     1185 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/dict.py
--rw-r--r--   0        0        0     1049 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/different_class.py
--rw-r--r--   0        0        0     1504 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/expression_converter.py
--rw-r--r--   0        0        0      958 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/list.py
--rw-r--r--   0        0        0      763 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/non_optional_to_optional.py
--rw-r--r--   0        0        0      877 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/optional_to_optional.py
--rw-r--r--   0        0        0      719 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/same_class.py
--rw-r--r--   0        0        0      906 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/set.py
--rw-r--r--   0        0        0     1072 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/tuple.py
--rw-r--r--   0        0        0      760 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/union_to_union.py
--rw-r--r--   0        0        0      555 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/__init__.py
--rw-r--r--   0        0        0      401 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/any.py
--rw-r--r--   0        0        0      817 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/base.py
--rw-r--r--   0        0        0      778 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/class_fieldtype.py
--rw-r--r--   0        0        0      895 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/dict.py
--rw-r--r--   0        0        0      758 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/list.py
--rw-r--r--   0        0        0     1169 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/optional.py
--rw-r--r--   0        0        0      754 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/set.py
--rw-r--r--   0        0        0      891 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/tuple.py
--rw-r--r--   0        0        0      878 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/union.py
--rw-r--r--   0        0        0      719 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/utils.py
--rw-r--r--   0        0        0      484 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/implementations/__init__.py
--rw-r--r--   0        0        0     2343 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/implementations/base.py
--rw-r--r--   0        0        0       77 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/implementations/class_type.py
--rw-r--r--   0        0        0     2190 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/implementations/dataclasses.py
--rw-r--r--   0        0        0     4090 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/implementations/pydantic_v1.py
--rw-r--r--   0        0        0     4085 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/implementations/pydantic_v2.py
--rw-r--r--   0        0        0     6179 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/implementations/sqlalchemy.py
--rw-r--r--   0        0        0      238 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/implementations/utils.py
--rw-r--r--   0        0        0    19408 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/mapper.py
--rw-r--r--   0        0        0      859 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/mapper_mode.py
--rw-r--r--   0        0        0    11776 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/mapping_method.py
--rw-r--r--   0        0        0     4126 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/mapping_preparation.py
--rw-r--r--   0        0        0      404 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/namespace.py
--rw-r--r--   0        0        0        0 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/py.typed
--rw-r--r--   0        0        0     2979 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/special_field_mappings.py
--rw-r--r--   0        0        0      280 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/update_expressions/__init__.py
--rw-r--r--   0        0        0     1102 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/update_expressions/classes.py
--rw-r--r--   0        0        0     1072 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/update_expressions/unsupported_dataclasses.py
--rw-r--r--   0        0        0     1442 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/update_expressions/update_expression.py
--rw-r--r--   0        0        0     1306 2024-02-11 13:56:04.952648 dataclass_mapper-2.0.0a0/dataclass_mapper/utils.py
--rw-r--r--   0        0        0     2406 2024-02-11 13:57:15.588335 dataclass_mapper-2.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     7140 1970-01-01 00:00:00.000000 dataclass_mapper-2.0.0a0/setup.py
--rw-r--r--   0        0        0     7495 1970-01-01 00:00:00.000000 dataclass_mapper-2.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/LICENSE.md
+-rw-r--r--   0        0        0     6336 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/README.rst
+-rw-r--r--   0        0        0      686 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/__init__.py
+-rw-r--r--   0        0        0      951 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/classmeta.py
+-rw-r--r--   0        0        0    10106 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/code_generator.py
+-rw-r--r--   0        0        0     3720 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/collection.py
+-rw-r--r--   0        0        0     2285 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/enum.py
+-rw-r--r--   0        0        0      337 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/exceptions.py
+-rw-r--r--   0        0        0     1139 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/__init__.py
+-rw-r--r--   0        0        0      581 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/anything_to_any.py
+-rw-r--r--   0        0        0      753 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/class_to_union.py
+-rw-r--r--   0        0        0     1185 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/dict.py
+-rw-r--r--   0        0        0     1244 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/different_class.py
+-rw-r--r--   0        0        0     1504 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/expression_converter.py
+-rw-r--r--   0        0        0      958 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/list.py
+-rw-r--r--   0        0        0      763 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/non_optional_to_optional.py
+-rw-r--r--   0        0        0      877 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/optional_to_optional.py
+-rw-r--r--   0        0        0      719 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/same_class.py
+-rw-r--r--   0        0        0      906 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/set.py
+-rw-r--r--   0        0        0     1072 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/tuple.py
+-rw-r--r--   0        0        0      760 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/union_to_union.py
+-rw-r--r--   0        0        0      555 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/__init__.py
+-rw-r--r--   0        0        0      401 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/any.py
+-rw-r--r--   0        0        0      817 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/base.py
+-rw-r--r--   0        0        0      778 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/class_fieldtype.py
+-rw-r--r--   0        0        0      895 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/dict.py
+-rw-r--r--   0        0        0      758 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/list.py
+-rw-r--r--   0        0        0     1169 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/optional.py
+-rw-r--r--   0        0        0      754 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/set.py
+-rw-r--r--   0        0        0      891 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/tuple.py
+-rw-r--r--   0        0        0      878 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/union.py
+-rw-r--r--   0        0        0      719 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/utils.py
+-rw-r--r--   0        0        0      536 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/implementations/__init__.py
+-rw-r--r--   0        0        0     2367 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/implementations/base.py
+-rw-r--r--   0        0        0       77 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/implementations/class_type.py
+-rw-r--r--   0        0        0     2190 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/implementations/dataclasses.py
+-rw-r--r--   0        0        0     4090 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/implementations/pydantic_v1.py
+-rw-r--r--   0        0        0     4085 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/implementations/pydantic_v2.py
+-rw-r--r--   0        0        0     1243 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/implementations/simple_type.py
+-rw-r--r--   0        0        0     6171 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/implementations/sqlalchemy.py
+-rw-r--r--   0        0        0      238 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/implementations/utils.py
+-rw-r--r--   0        0        0    19109 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/mapper.py
+-rw-r--r--   0        0        0      859 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/mapper_mode.py
+-rw-r--r--   0        0        0    11752 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/mapping_method.py
+-rw-r--r--   0        0        0     4126 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/mapping_preparation.py
+-rw-r--r--   0        0        0      404 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/namespace.py
+-rw-r--r--   0        0        0        0 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/py.typed
+-rw-r--r--   0        0        0     2979 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/special_field_mappings.py
+-rw-r--r--   0        0        0      280 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/update_expressions/__init__.py
+-rw-r--r--   0        0        0     1294 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/update_expressions/classes.py
+-rw-r--r--   0        0        0     1083 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/update_expressions/unsupported_dataclasses.py
+-rw-r--r--   0        0        0     1442 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/update_expressions/update_expression.py
+-rw-r--r--   0        0        0      423 2024-04-01 18:43:17.759646 dataclass_mapper-2.0.0a1/dataclass_mapper/utils.py
+-rw-r--r--   0        0        0     2406 2024-04-01 18:44:21.516139 dataclass_mapper-2.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     7374 1970-01-01 00:00:00.000000 dataclass_mapper-2.0.0a1/setup.py
+-rw-r--r--   0        0        0     7724 1970-01-01 00:00:00.000000 dataclass_mapper-2.0.0a1/PKG-INFO
```

### Comparing `dataclass_mapper-2.0.0a0/LICENSE.md` & `dataclass_mapper-2.0.0a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/README.rst` & `dataclass_mapper-2.0.0a1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -129,14 +129,19 @@
 
 * Python's ``dataclass`` (with recursive models, update existing models, custom initializers, optional types, extra-context, ...): see `Supported features <https://dataclass-mapper.readthedocs.io/en/latest/features.html>`_ for the full list and examples
 * Mappings between Enum classes:  see `Enum mappings <https://dataclass-mapper.readthedocs.io/en/latest/enums.html>`_
 * Pydantic models:  see `Pydantic models <https://dataclass-mapper.readthedocs.io/en/latest/pydantic.html>`_
 * SQLAlchemy ORM models:  see `SQLAlchemy ORM models <https://dataclass-mapper.readthedocs.io/en/latest/sqlalchemy.html>`_
 * Type/Value checks:  see `Type safety <https://dataclass-mapper.readthedocs.io/en/latest/type_safety.html>`_
 
+Demo project
+------------
+
+We maintain a small demo project, whichs shows some of the interworkings of the library together with a FastAPI API and SQLAlchemy ORM: `todo-app <https://github.com/dataclass-mapper/todo-app-demo>`_.
+
 Contributing
 ------------
 
 See `CONTRIBUTING.rst <https://github.com/dataclass-mapper/dataclass-mapper/blob/develop/CONTRIBUTING.rst>`_.
 
 License
 -------
```

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/__init__.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/classmeta.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/classmeta.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from enum import Enum
 from typing import Any
 
+from dataclass_mapper.implementations.simple_type import SimpleType
+
 from .implementations import class_meta_types
 from .implementations.base import ClassMeta
 from .implementations.class_type import ClassType
 from .namespace import Namespace
 
 
 def get_class_meta(cls: Any, namespace: Namespace, type_: ClassType = ClassType.TARGET) -> ClassMeta:
@@ -14,8 +16,8 @@
 
     if issubclass(cls, Enum):
         raise ValueError("`mapper` does not support enum classes, use `enum_mapper` instead")
     raise NotImplementedError("only dataclasses, pydantic and sqlalchemy classes are supported")
 
 
 def is_dataclass_supported(cls: Any) -> bool:
-    return any(class_meta_type.applies(cls) for class_meta_type in class_meta_types)
+    return any(class_meta_type.applies(cls) for class_meta_type in class_meta_types if class_meta_type != SimpleType)
```

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/code_generator.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/code_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,15 @@
     def get_ctx(self):
         if self.store:
             return ast.Store()
         else:
             return ast.Load()
 
     @abstractmethod
-    def generate_ast(self) -> ast.expr:
-        ...
+    def generate_ast(self) -> ast.expr: ...
 
     def is_(self, other: "Expression") -> "Expression":
         return Compare(self, other, ast.Is())
 
     def is_not(self, other: "Expression") -> "Expression":
         return Compare(self, other, ast.IsNot())
 
@@ -95,15 +94,27 @@
 
 
 @dataclass
 class AttributeLookup(Expression):
     obj: Expression
     attribute: str
 
+    def as_store(self) -> "Expression":
+        """Empty attribute means, that there is no attribute lookup at all.
+        So the as_store() hint needs to be handed over to the nested obj.
+        """
+        if self.attribute:
+            return super().as_store()
+        else:
+            self.obj = self.obj.as_store()
+            return self
+
     def generate_ast(self) -> ast.expr:
+        if not self.attribute:
+            return self.obj.generate_ast()
         return ast.Attribute(value=self.obj.generate_ast(), attr=self.attribute, ctx=self.get_ctx())
 
 
 @dataclass
 class TernaryOperator(Expression):
     condition: Expression
     true_case: Expression
```

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/enum.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/enum.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/__init__.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/anything_to_any.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/anything_to_any.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/class_to_union.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/class_to_union.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/dict.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/dict.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/different_class.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/different_class.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-from dataclass_mapper.code_generator import Expression, MethodCall, Variable
+from dataclass_mapper.code_generator import Constant, DictLookup, Expression, FunctionCall, Variable
+from dataclass_mapper.collection import COLLECTION
 from dataclass_mapper.fieldtypes import FieldType
 from dataclass_mapper.fieldtypes.class_fieldtype import ClassFieldType
-from dataclass_mapper.utils import get_map_to_func_name, is_mappable_to
 
 from .expression_converter import ExpressionConverter
 
 
 class DifferentClassExpressionConverter(ExpressionConverter):
     def is_applicable_to_outer(self, source: FieldType, target: FieldType) -> bool:
         return (
             isinstance(source, ClassFieldType)
             and isinstance(target, ClassFieldType)
             and source.cls_type is not target.cls_type
-            and is_mappable_to(source.cls_type, target.cls_type)
+            and COLLECTION.contains_create(source.cls_type, target.cls_type)
         )
 
     def map_expression(
         self, source: FieldType, target: FieldType, source_exp: Expression, recursion_depth: int
     ) -> Expression:
+        assert isinstance(source, ClassFieldType)
         assert isinstance(target, ClassFieldType)
         extra_variable = Variable("extra")
-        return MethodCall(source_exp, get_map_to_func_name(target.cls_type), [extra_variable])
+        func_name = COLLECTION.create_func_name(source.cls_type, target.cls_type)
+        function = DictLookup(Variable("COLLECTION"), Constant(func_name))
+        return FunctionCall(function, [source_exp, extra_variable])
```

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/expression_converter.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/expression_converter.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/list.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/list.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/non_optional_to_optional.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/non_optional_to_optional.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/optional_to_optional.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/optional_to_optional.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/same_class.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/same_class.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/set.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/set.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/tuple.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/tuple.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/expression_converters/union_to_union.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/expression_converters/union_to_union.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/__init__.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/base.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/base.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/class_fieldtype.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/class_fieldtype.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/dict.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/dict.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/list.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/list.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/optional.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/optional.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/set.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/set.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/tuple.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/tuple.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/union.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/union.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/fieldtypes/utils.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/fieldtypes/utils.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/implementations/base.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/implementations/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 from .class_type import ClassType
 
 
 class DataclassType(Enum):
     DATACLASSES = auto()
     PYDANTIC = auto()
-    SQLAlchemy = auto()
+    SQLALCHEMY = auto()
+    SIMPLETYPE = auto()
 
 
 @dataclass(frozen=True)
 class FieldMeta:
     """Dataclass containing meta information about fields in dataclasses or pydantic classes.
     Information like the name and type of the field, and if it is required to set it.
     """
```

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/implementations/dataclasses.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/implementations/dataclasses.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/implementations/pydantic_v1.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/implementations/pydantic_v1.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/implementations/pydantic_v2.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/implementations/pydantic_v2.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/implementations/sqlalchemy.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/implementations/sqlalchemy.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,16 +153,15 @@
 
 
 @runtime_checkable
 class InstrumentedAttribute(Protocol):
     class_: Any
 
     @property
-    def property(self) -> Any:
-        ...
+    def property(self) -> Any: ...
 
 
 def extract_instrumented_attribute_name_and_class(attribute: InstrumentedAttribute) -> Tuple[str, Any]:
     try:
         sqlalchemy = __import__("sqlalchemy")
     except ModuleNotFoundError:
         raise ValueError("Unknown field") from None
```

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/mapper.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/mapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import ast
 import sys
 from dataclasses import replace
+from enum import Enum
 from importlib import import_module
 from typing import Any, Callable, Dict, Optional, Tuple, Type, TypeVar, Union, cast, overload
 
+from dataclass_mapper.implementations.simple_type import SimpleType
+
 from .classmeta import get_class_meta
+from .collection import COLLECTION
 from .enum import EnumMapping, make_enum_mapper
 from .fieldtypes.optional import OptionalFieldType
 from .implementations.class_type import ClassType
 from .mapper_mode import MapperMode
 from .mapping_method import CreateMappingMethodSourceCode, MappingMethodSourceCode, UpdateMappingMethodSourceCode
 from .mapping_preparation import (
     convert_sqlalchemy_fields,
@@ -20,15 +24,14 @@
 from .special_field_mappings import (
     AssumeNotNone,
     FromExtra,
     Ignore,
     StringSqlAlchemyFieldMapping,
     UpdateOnlyIfSet,
 )
-from .utils import get_map_to_func_name, get_mapupdate_to_func_name
 
 
 def _make_mapper(
     mapping: StringSqlAlchemyFieldMapping,
     source_cls: Any,
     target_cls: Any,
     namespace: Namespace,
@@ -36,14 +39,21 @@
     mapper_mode: MapperMode,
 ) -> Tuple[ast.Module, Dict[str, Callable], Dict[str, Any]]:
     source_cls_meta = get_class_meta(source_cls, namespace=namespace, type_=ClassType.SOURCE)
     target_cls_meta = get_class_meta(target_cls, namespace=namespace, type_=ClassType.TARGET)
     actual_source_fields = source_cls_meta.fields
     actual_target_fields = target_cls_meta.fields
 
+    if (isinstance(source_cls_meta, SimpleType) and "" not in mapping.values()) or (
+        isinstance(target_cls_meta, SimpleType) and "" not in mapping
+    ):
+        if issubclass(source_cls, Enum) and issubclass(target_cls, Enum):
+            raise ValueError("`mapper` does not support enum classes, use `enum_mapper` instead")
+        raise NotImplementedError("only dataclasses, pydantic and sqlalchemy classes are supported")
+
     string_field_mapping = convert_sqlalchemy_fields(
         mapping, source_cls_meta=source_cls_meta, target_cls_meta=target_cls_meta
     )
     string_field_mapping = generate_missing_mappings(
         string_field_mapping, actual_source_fields=actual_source_fields, actual_target_fields=actual_target_fields
     )
     raise_if_mapping_doesnt_match_target(
@@ -102,15 +112,19 @@
                     "as it has no default"
                 )
         elif callable(raw_source):
             source_code.add_factory(target=target_field, source=raw_source)
         else:
             raise AssertionError("impossible to reach")
 
-    return source_code.get_ast(), source_code.factories, {target_cls_meta.internal_name: target_cls}
+    return (
+        source_code.get_ast(),
+        source_code.factories,
+        {target_cls_meta.internal_name: target_cls, "COLLECTION": COLLECTION},
+    )
 
 
 def create_mapper(
     SourceCls: Any,
     TargetCls: Any,
     mapping: Optional[StringSqlAlchemyFieldMapping] = None,
     mapper_mode: MapperMode = MapperMode.CREATE_AND_UPDATE,
@@ -219,46 +233,41 @@
     mapping: Optional[StringSqlAlchemyFieldMapping],
     namespace: Namespace,
     mapper_mode: MapperMode,
 ) -> None:
     field_mapping = mapping or cast(StringSqlAlchemyFieldMapping, {})
 
     if mapper_mode in (MapperMode.CREATE, MapperMode.CREATE_AND_UPDATE):
-        create_map_func_name = get_map_to_func_name(TargetCls)
         add_specific_mapper_function(
             SourceCls=SourceCls,
             TargetCls=TargetCls,
             field_mapping=field_mapping,
             source_code_type=CreateMappingMethodSourceCode,
             mapper_mode=mapper_mode,
             namespace=namespace,
-            map_func_name=create_map_func_name,
         )
 
     if mapper_mode in (MapperMode.UPDATE, MapperMode.CREATE_AND_UPDATE):
-        update_map_func_name = get_mapupdate_to_func_name(TargetCls)
         add_specific_mapper_function(
             SourceCls=SourceCls,
             TargetCls=TargetCls,
             field_mapping=field_mapping,
             source_code_type=UpdateMappingMethodSourceCode,
             mapper_mode=mapper_mode,
             namespace=namespace,
-            map_func_name=update_map_func_name,
         )
 
 
 def add_specific_mapper_function(
     SourceCls: Any,
     TargetCls: Any,
     field_mapping: StringSqlAlchemyFieldMapping,
     namespace: Namespace,
     source_code_type: Type[MappingMethodSourceCode],
     mapper_mode: MapperMode,
-    map_func_name: str,
 ) -> None:
     map_code_ast, factories, context = _make_mapper(
         field_mapping,
         source_cls=SourceCls,
         target_cls=TargetCls,
         namespace=namespace,
         source_code_type=source_code_type,
@@ -269,26 +278,25 @@
 
     d: Dict = {}
     filename = f"<{source_code_type.func_name}_{SourceCls.__name__}_{TargetCls.__name__}>"
     map_code = compile(map_code_ast, filename=filename, mode="exec")
     # Support older versions of python by calling {**a, **b} rather than a|b
     exec(map_code, {**module.__dict__, **context}, d)  # noqa: S102
 
-    if hasattr(SourceCls, map_func_name):
-        raise AttributeError(
-            f"There already exists a mapping between '{SourceCls.__name__}' and '{TargetCls.__name__}'"
-        )
     map_func = d[source_code_type.func_name]
+
     if sys.version_info < (3, 9):
-        map_func.__doc__ = ast.dump(map_code_ast)
+        map_code_str = ast.dump(map_code_ast)
     else:
-        map_func.__doc__ = ast.unparse(map_code_ast)
-    setattr(SourceCls, map_func_name, map_func)
-    for name, factory in factories.items():
-        setattr(SourceCls, name, factory)
+        map_code_str = ast.unparse(map_code_ast)
+
+    if source_code_type is CreateMappingMethodSourceCode:
+        COLLECTION.store_create_func(SourceCls, TargetCls, map_func, map_code_str, factories)
+    else:
+        COLLECTION.store_update_func(SourceCls, TargetCls, map_func, map_code_str, factories)
 
 
 def create_enum_mapper(SourceCls: Any, TargetCls: Any, mapping: Optional[EnumMapping] = None) -> None:
     """Creates a private mapper method, that maps the enum class ``SourceCls`` to the
     enum class ``TargetCls``. The mapper method can be called using the :func:`map_to` function.
 
     :param SourceCls: The enum class (source class) that you want to map an object of the current
@@ -355,20 +363,15 @@
 
 def add_enum_mapper_function(SourceCls: Any, TargetCls: Any, mapping: Optional[EnumMapping]) -> None:
     convert_function = make_enum_mapper(
         source_cls=SourceCls,
         target_cls=TargetCls,
         mapping=mapping or cast(EnumMapping, {}),
     )
-    map_func_name = get_map_to_func_name(TargetCls)
-    if hasattr(SourceCls, map_func_name):
-        raise AttributeError(
-            f"There already exists a mapping between '{SourceCls.__name__}' and '{TargetCls.__name__}'"
-        )
-    setattr(SourceCls, map_func_name, convert_function)
+    COLLECTION.store_create_func(SourceCls, TargetCls, convert_function, "", {})
 
 
 @overload
 def map_to(obj, target: Type[T], extra: Optional[Dict[str, Any]] = None) -> T:
     pass
 
 
@@ -388,34 +391,24 @@
     :param extra: dictionary with the values for the `provide_with_extra()` fields
     :return: the mapped object
     """
     if extra is None:
         extra = {}
 
     if isinstance(target, type):
-        TargetCls = target
-        func_name = get_map_to_func_name(target)
-
-        if hasattr(obj, func_name):
-            return cast(T, getattr(obj, func_name)(extra))
+        func = COLLECTION.get_create_func(obj.__class__, target)
+        return cast(T, func(obj, extra))
     else:
-        TargetCls = target.__class__
-        func_name = get_mapupdate_to_func_name(TargetCls)
-
-        if hasattr(obj, func_name):
-            return cast(T, getattr(obj, func_name)(target, extra))
-
-    raise NotImplementedError(f"Object of type '{type(obj).__name__}' cannot be mapped to '{TargetCls.__name__}'")
+        func = COLLECTION.get_update_func(obj.__class__, target.__class__)
+        return cast(T, func(obj, target, extra))
 
 
-def debug_map_codes(source: Type, target: Type) -> Tuple[Optional[str], Optional[str]]:
-    create_func_name = get_map_to_func_name(target)
+def debug_map_codes(SourceCls: Type, TargetCls: Type) -> Tuple[Optional[str], Optional[str]]:
     map_create_code: Optional[str] = None
-    if hasattr(source, create_func_name):
-        map_create_code = getattr(source, create_func_name).__doc__
+    if COLLECTION.contains_create(SourceCls, TargetCls):
+        map_create_code = COLLECTION.get_create_code(SourceCls, TargetCls)
 
-    update_func_name = get_mapupdate_to_func_name(target)
     map_update_code: Optional[str] = None
-    if hasattr(source, update_func_name):
-        map_update_code = getattr(source, update_func_name).__doc__
+    if COLLECTION.contains_update(SourceCls, TargetCls):
+        map_update_code = COLLECTION.get_update_code(SourceCls, TargetCls)
 
     return (map_create_code, map_update_code)
```

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/mapper_mode.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/mapper_mode.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/mapping_method.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/mapping_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ast
 from abc import ABC, abstractmethod
 from dataclasses import replace
 from inspect import signature
-from typing import Callable, Dict, List, Optional, cast
+from typing import Callable, Dict, List, Optional
 from uuid import uuid4
 
 from dataclass_mapper.exceptions import ConvertingNotPossibleError, UpdatingNotPossibleError
 from dataclass_mapper.expression_converters import map_expression
 from dataclass_mapper.mapper_mode import MapperMode
 from dataclass_mapper.update_expressions import map_update_expression
 
@@ -83,20 +83,18 @@
             # can only happen, if the typing annotation fails (e.g. because mypy is not installed)
             raise ValueError(
                 f"'{target.attribute_name}' of '{self.target_cls.name}' cannot be mapped "
                 "using a factory with more than one parameter"
             )
 
         factory_name = f"_{uuid4().hex}"
-        if parameter_cnt == 0:
-            self.factories[factory_name] = cast(Callable, staticmethod(source))
-        else:
-            self.factories[factory_name] = source
+        self.factories[factory_name] = source
 
-        factory_call = cg.MethodCall(SELF_VAR, factory_name, [])
+        factory = cg.DictLookup(cg.Variable("COLLECTION"), cg.Constant(factory_name))
+        factory_call = cg.FunctionCall(factory, [] if parameter_cnt == 0 else [SELF_VAR])
         assignment = self._get_assignment(None, target, factory_call, only_if_source_is_set=False)
         self._add(target.init_with_ctor, assignment)
 
     def add_from_extra(self, target: FieldMeta, source: FromExtra) -> None:
         """Generate code for assign the result of a lookup in the extra dictionary to the field, if it exists.
         Raise an exception if it doesn't exist.
         """
```

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/mapping_preparation.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/mapping_preparation.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/special_field_mappings.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/special_field_mappings.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/update_expressions/classes.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/update_expressions/classes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,33 @@
-from dataclass_mapper.code_generator import Expression, ExpressionStatement, MethodCall, Statement, Variable
+from dataclass_mapper.code_generator import (
+    Constant,
+    DictLookup,
+    Expression,
+    ExpressionStatement,
+    FunctionCall,
+    Statement,
+    Variable,
+)
+from dataclass_mapper.collection import COLLECTION
 from dataclass_mapper.fieldtypes import FieldType
 from dataclass_mapper.fieldtypes.class_fieldtype import ClassFieldType
-from dataclass_mapper.utils import get_mapupdate_to_func_name, is_updatable_to
 
 from .update_expression import UpdateExpression
 
 
 class ClassesUpdateExpression(UpdateExpression):
     def is_applicable_to_outer(self, source: FieldType, target: FieldType) -> bool:
         return (
             isinstance(source, ClassFieldType)
             and isinstance(target, ClassFieldType)
-            and is_updatable_to(source.cls_type, target.cls_type)
+            and COLLECTION.contains_update(source.cls_type, target.cls_type)
         )
 
     def update_expression(
         self, source: FieldType, target: FieldType, source_exp: Expression, target_exp: Expression, recursion_depth: int
     ) -> Statement:
+        assert isinstance(source, ClassFieldType)
         assert isinstance(target, ClassFieldType)
         extra_variable = Variable("extra")
-        return ExpressionStatement(
-            MethodCall(source_exp, get_mapupdate_to_func_name(target.cls_type), [target_exp, extra_variable])
-        )
+        func_name = COLLECTION.update_func_name(source.cls_type, target.cls_type)
+        function = DictLookup(Variable("COLLECTION"), Constant(func_name))
+        return ExpressionStatement(FunctionCall(function, [source_exp, target_exp, extra_variable]))
```

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/update_expressions/unsupported_dataclasses.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/update_expressions/unsupported_dataclasses.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from dataclass_mapper.classmeta import is_dataclass_supported
 from dataclass_mapper.code_generator import Expression, Statement
+from dataclass_mapper.collection import COLLECTION
 from dataclass_mapper.fieldtypes import FieldType
 from dataclass_mapper.fieldtypes.class_fieldtype import ClassFieldType
-from dataclass_mapper.utils import is_updatable_to
 
 from .update_expression import UpdateExpression
 
 
 class UnsupportedDataclassesUpdateExpression(UpdateExpression):
     def is_applicable_to_outer(self, source: FieldType, target: FieldType) -> bool:
         return (
             isinstance(source, ClassFieldType)
             and isinstance(target, ClassFieldType)
             and is_dataclass_supported(source.cls_type)
             and is_dataclass_supported(target.cls_type)
-            and not is_updatable_to(source.cls_type, target.cls_type)
+            and not COLLECTION.contains_update(source.cls_type, target.cls_type)
         )
 
     def update_expression(
         self, source: FieldType, target: FieldType, source_exp: Expression, target_exp: Expression, recursion_depth: int
     ) -> Statement:
         raise TypeError(f"There is no update mapper defined between '{source}' and '{target}'.")
```

### Comparing `dataclass_mapper-2.0.0a0/dataclass_mapper/update_expressions/update_expression.py` & `dataclass_mapper-2.0.0a1/dataclass_mapper/update_expressions/update_expression.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-2.0.0a0/pyproject.toml` & `dataclass_mapper-2.0.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-mapper"
-version = "2.0.0-a.0"
+version = "2.0.0-a.1"
 description = "Autogenerate mappings between dataclasses"
 authors = ["Jakob Kogler <jakob.kogler@gmail.com>"]
 
 readme = "README.rst"
 license = "MIT"
 
 repository = "https://github.com/dataclass-mapper/dataclass-mapper"
@@ -47,15 +47,15 @@
 Sphinx = "^5.0.2"
 sphinx-rtd-theme = "^1.3.0"
 sphinxcontrib-plantuml = "^0.25"
 sphinx-autobuild = "^2021.3.14"
 enum-tools = {extras = ["sphinx"], version = "^0.11.0"}
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.2.1"
+ruff = "^0.3.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 120
```

### Comparing `dataclass_mapper-2.0.0a0/setup.py` & `dataclass_mapper-2.0.0a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 {'': ['*']}
 
 extras_require = \
 {'pydantic': ['pydantic>=1.9.0'], 'sqlalchemy': ['SQLAlchemy>=2.0.0']}
 
 setup_kwargs = {
     'name': 'dataclass-mapper',
-    'version': '2.0.0a0',
+    'version': '2.0.0a1',
     'description': 'Autogenerate mappings between dataclasses',
-    'long_description': 'dataclass-mapper\n================\n\n|pypi| |support| |licence| |readthedocs| |build| |coverage|\n\n.. |pypi| image:: https://img.shields.io/pypi/v/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: pypi version\n\n.. |support| image:: https://img.shields.io/pypi/pyversions/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: supported Python version\n\n.. |build| image:: https://github.com/dataclass-mapper/dataclass-mapper/actions/workflows/test.yml/badge.svg\n    :target: https://github.com/dataclass-mapper/dataclass-mapper/actions\n    :alt: build status\n\n.. |coverage| image:: https://codecov.io/gh/dataclass-mapper/dataclass-mapper/branch/develop/graphs/badge.svg?branch=develop\n    :target: https://codecov.io/gh/dataclass-mapper/dataclass-mapper?branch=develop\n    :alt: Code coverage\n\n.. |licence| image:: https://img.shields.io/pypi/l/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: licence\n\n.. |readthedocs| image:: https://img.shields.io/readthedocs/dataclass-mapper/latest.svg?style=flat-square&label=Read%20the%20Docs\n   :alt: Read the documentation at https://dataclass-mapper.readthedocs.io/en/latest/\n   :target: https://dataclass-mapper.readthedocs.io/en/latest/\n\nWriting mapper methods between two similar dataclasses is boring, need to be actively maintained and are error-prone.\nMuch better to let this library auto-generate them for you.\n\nThe focus of this library is:\n\n- **Concise and easy syntax:**\n  \n  - using it has to be a lot less overhead than writing the mappers by hand\n  - trivial mappings should not require code\n  - identical syntax for mapping between dataclasses, Pydantic and SQLAlchemy models\n\n- **Safety:**\n\n  - using this library must give equal or more type safety than writing the mappers by hand\n  - the types between source and target classes must matches (including optional checks)\n  - all target fields must be actually initialized\n  - mappings cannot reference non-existing fields\n  - in case of an error a clean exception must be raised\n\n- **Performance:**\n\n  - mapping an object using this library must be the same speed than mapping using a custom mapper function\n  - the type checks shouldn\'t slow down the program\n  - because of the first two points, all type checks and the generation of the mapper functions happen during the definition of the classes\n\nMotivation\n----------\n\nA couple of example usecases, that show why this library might be useful.\n\n* Given an API with multiple, different interfaces (e.g. different API versions), that are all connected to a common algorithm with some common datamodel.\n  All the different API models needs to be mapped to the common datamodel, and afterwards mapped back to the API model.\n* Given an API that has a ``POST`` and a ``GET`` endpoint.\n  Both models (``POST`` request body model and ``GET`` response body model) are almost the same, but there are some minor differences.\n  E.g. response model has an additional ``id`` parameter.\n  You need a way of mapping the request model to a response model.\n\nInstallation\n------------\n\n``dataclass-mapper`` can be installed using:\n\n.. code-block:: bash\n\n   pip install dataclass-mapper\n   # or for Pydantic support\n   pip install \'dataclass-mapper[pydantic]\'\n   # or for SQLAlchemy support\n   pip install \'dataclass-mapper[sqlalchemy]\'\n\nExample\n-------\n\nWe have the following target data structure, a class called ``Person``.\n\n.. code-block:: python\n\n   >>> from dataclasses import dataclass\n\n   >>> @dataclass\n   ... class Person:\n   ...     first_name: str\n   ...     second_name: str\n   ...     age: int\n\n\nWe want to have a mapper from the source data structure, a class called ``ContactInfo``.\nNotice that the attribute ``second_name`` of ``Person`` is called ``surname`` in ``ContactInfo``.\nOther than that, all the attribute names are the same.\n\nInstead of writing a mapper function by hand, you can let it autogenerate one using this library:\n\n.. code-block:: python\n\n   >>> from dataclass_mapper import map_to, mapper\n   >>>\n   >>> @mapper(Person, {"second_name": "surname"})\n   ... @dataclass\n   ... class ContactInfo:\n   ...     first_name: str\n   ...     surname: str\n   ...     age: int\n   >>>\n   >>> contact = ContactInfo(first_name="Henry", surname="Kaye", age=42)\n   >>> map_to(contact, Person)\n   Person(first_name=\'Henry\', second_name=\'Kaye\', age=42)\n\nThe ``dataclass-mapper`` library autogenerated a mapper, that can be used with the ``map_to`` function.\nAll we had to specify was the name of the target class, and optionally specify which fields map to which other fields.\nNotice that we only had to specify that the ``second_name`` field has to be mapped to ``surname``,\nall other fields were mapped automatically because the field names didn\'t change.\n\nAnd the ``dataclass-mapper`` library will perform a lot of checks around this mapping.\nIt will check if the data types match, if some fields would be left uninitialized, etc.\n\nFeatures\n--------\n\nThe current version has support for:\n\n* Python\'s ``dataclass`` (with recursive models, update existing models, custom initializers, optional types, extra-context, ...): see `Supported features <https://dataclass-mapper.readthedocs.io/en/latest/features.html>`_ for the full list and examples\n* Mappings between Enum classes:  see `Enum mappings <https://dataclass-mapper.readthedocs.io/en/latest/enums.html>`_\n* Pydantic models:  see `Pydantic models <https://dataclass-mapper.readthedocs.io/en/latest/pydantic.html>`_\n* SQLAlchemy ORM models:  see `SQLAlchemy ORM models <https://dataclass-mapper.readthedocs.io/en/latest/sqlalchemy.html>`_\n* Type/Value checks:  see `Type safety <https://dataclass-mapper.readthedocs.io/en/latest/type_safety.html>`_\n\nContributing\n------------\n\nSee `CONTRIBUTING.rst <https://github.com/dataclass-mapper/dataclass-mapper/blob/develop/CONTRIBUTING.rst>`_.\n\nLicense\n-------\n\nThe project is released under the `MIT license <https://github.com/dataclass-mapper/dataclass-mapper/blob/develop/LICENSE.md>`_.\n',
+    'long_description': 'dataclass-mapper\n================\n\n|pypi| |support| |licence| |readthedocs| |build| |coverage|\n\n.. |pypi| image:: https://img.shields.io/pypi/v/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: pypi version\n\n.. |support| image:: https://img.shields.io/pypi/pyversions/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: supported Python version\n\n.. |build| image:: https://github.com/dataclass-mapper/dataclass-mapper/actions/workflows/test.yml/badge.svg\n    :target: https://github.com/dataclass-mapper/dataclass-mapper/actions\n    :alt: build status\n\n.. |coverage| image:: https://codecov.io/gh/dataclass-mapper/dataclass-mapper/branch/develop/graphs/badge.svg?branch=develop\n    :target: https://codecov.io/gh/dataclass-mapper/dataclass-mapper?branch=develop\n    :alt: Code coverage\n\n.. |licence| image:: https://img.shields.io/pypi/l/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: licence\n\n.. |readthedocs| image:: https://img.shields.io/readthedocs/dataclass-mapper/latest.svg?style=flat-square&label=Read%20the%20Docs\n   :alt: Read the documentation at https://dataclass-mapper.readthedocs.io/en/latest/\n   :target: https://dataclass-mapper.readthedocs.io/en/latest/\n\nWriting mapper methods between two similar dataclasses is boring, need to be actively maintained and are error-prone.\nMuch better to let this library auto-generate them for you.\n\nThe focus of this library is:\n\n- **Concise and easy syntax:**\n  \n  - using it has to be a lot less overhead than writing the mappers by hand\n  - trivial mappings should not require code\n  - identical syntax for mapping between dataclasses, Pydantic and SQLAlchemy models\n\n- **Safety:**\n\n  - using this library must give equal or more type safety than writing the mappers by hand\n  - the types between source and target classes must matches (including optional checks)\n  - all target fields must be actually initialized\n  - mappings cannot reference non-existing fields\n  - in case of an error a clean exception must be raised\n\n- **Performance:**\n\n  - mapping an object using this library must be the same speed than mapping using a custom mapper function\n  - the type checks shouldn\'t slow down the program\n  - because of the first two points, all type checks and the generation of the mapper functions happen during the definition of the classes\n\nMotivation\n----------\n\nA couple of example usecases, that show why this library might be useful.\n\n* Given an API with multiple, different interfaces (e.g. different API versions), that are all connected to a common algorithm with some common datamodel.\n  All the different API models needs to be mapped to the common datamodel, and afterwards mapped back to the API model.\n* Given an API that has a ``POST`` and a ``GET`` endpoint.\n  Both models (``POST`` request body model and ``GET`` response body model) are almost the same, but there are some minor differences.\n  E.g. response model has an additional ``id`` parameter.\n  You need a way of mapping the request model to a response model.\n\nInstallation\n------------\n\n``dataclass-mapper`` can be installed using:\n\n.. code-block:: bash\n\n   pip install dataclass-mapper\n   # or for Pydantic support\n   pip install \'dataclass-mapper[pydantic]\'\n   # or for SQLAlchemy support\n   pip install \'dataclass-mapper[sqlalchemy]\'\n\nExample\n-------\n\nWe have the following target data structure, a class called ``Person``.\n\n.. code-block:: python\n\n   >>> from dataclasses import dataclass\n\n   >>> @dataclass\n   ... class Person:\n   ...     first_name: str\n   ...     second_name: str\n   ...     age: int\n\n\nWe want to have a mapper from the source data structure, a class called ``ContactInfo``.\nNotice that the attribute ``second_name`` of ``Person`` is called ``surname`` in ``ContactInfo``.\nOther than that, all the attribute names are the same.\n\nInstead of writing a mapper function by hand, you can let it autogenerate one using this library:\n\n.. code-block:: python\n\n   >>> from dataclass_mapper import map_to, mapper\n   >>>\n   >>> @mapper(Person, {"second_name": "surname"})\n   ... @dataclass\n   ... class ContactInfo:\n   ...     first_name: str\n   ...     surname: str\n   ...     age: int\n   >>>\n   >>> contact = ContactInfo(first_name="Henry", surname="Kaye", age=42)\n   >>> map_to(contact, Person)\n   Person(first_name=\'Henry\', second_name=\'Kaye\', age=42)\n\nThe ``dataclass-mapper`` library autogenerated a mapper, that can be used with the ``map_to`` function.\nAll we had to specify was the name of the target class, and optionally specify which fields map to which other fields.\nNotice that we only had to specify that the ``second_name`` field has to be mapped to ``surname``,\nall other fields were mapped automatically because the field names didn\'t change.\n\nAnd the ``dataclass-mapper`` library will perform a lot of checks around this mapping.\nIt will check if the data types match, if some fields would be left uninitialized, etc.\n\nFeatures\n--------\n\nThe current version has support for:\n\n* Python\'s ``dataclass`` (with recursive models, update existing models, custom initializers, optional types, extra-context, ...): see `Supported features <https://dataclass-mapper.readthedocs.io/en/latest/features.html>`_ for the full list and examples\n* Mappings between Enum classes:  see `Enum mappings <https://dataclass-mapper.readthedocs.io/en/latest/enums.html>`_\n* Pydantic models:  see `Pydantic models <https://dataclass-mapper.readthedocs.io/en/latest/pydantic.html>`_\n* SQLAlchemy ORM models:  see `SQLAlchemy ORM models <https://dataclass-mapper.readthedocs.io/en/latest/sqlalchemy.html>`_\n* Type/Value checks:  see `Type safety <https://dataclass-mapper.readthedocs.io/en/latest/type_safety.html>`_\n\nDemo project\n------------\n\nWe maintain a small demo project, whichs shows some of the interworkings of the library together with a FastAPI API and SQLAlchemy ORM: `todo-app <https://github.com/dataclass-mapper/todo-app-demo>`_.\n\nContributing\n------------\n\nSee `CONTRIBUTING.rst <https://github.com/dataclass-mapper/dataclass-mapper/blob/develop/CONTRIBUTING.rst>`_.\n\nLicense\n-------\n\nThe project is released under the `MIT license <https://github.com/dataclass-mapper/dataclass-mapper/blob/develop/LICENSE.md>`_.\n',
     'author': 'Jakob Kogler',
     'author_email': 'jakob.kogler@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://dataclass-mapper.readthedocs.io',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `dataclass_mapper-2.0.0a0/PKG-INFO` & `dataclass_mapper-2.0.0a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-mapper
-Version: 2.0.0a0
+Version: 2.0.0a1
 Summary: Autogenerate mappings between dataclasses
 Home-page: https://dataclass-mapper.readthedocs.io
 License: MIT
 Keywords: dataclass,pydantic,python,automation
 Author: Jakob Kogler
 Author-email: jakob.kogler@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -162,14 +162,19 @@
 
 * Python's ``dataclass`` (with recursive models, update existing models, custom initializers, optional types, extra-context, ...): see `Supported features <https://dataclass-mapper.readthedocs.io/en/latest/features.html>`_ for the full list and examples
 * Mappings between Enum classes:  see `Enum mappings <https://dataclass-mapper.readthedocs.io/en/latest/enums.html>`_
 * Pydantic models:  see `Pydantic models <https://dataclass-mapper.readthedocs.io/en/latest/pydantic.html>`_
 * SQLAlchemy ORM models:  see `SQLAlchemy ORM models <https://dataclass-mapper.readthedocs.io/en/latest/sqlalchemy.html>`_
 * Type/Value checks:  see `Type safety <https://dataclass-mapper.readthedocs.io/en/latest/type_safety.html>`_
 
+Demo project
+------------
+
+We maintain a small demo project, whichs shows some of the interworkings of the library together with a FastAPI API and SQLAlchemy ORM: `todo-app <https://github.com/dataclass-mapper/todo-app-demo>`_.
+
 Contributing
 ------------
 
 See `CONTRIBUTING.rst <https://github.com/dataclass-mapper/dataclass-mapper/blob/develop/CONTRIBUTING.rst>`_.
 
 License
 -------
```

