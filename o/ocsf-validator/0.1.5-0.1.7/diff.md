# Comparing `tmp/ocsf_validator-0.1.5.tar.gz` & `tmp/ocsf_validator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocsf_validator-0.1.5.tar", max compression
+gzip compressed data, was "ocsf_validator-0.1.7.tar", max compression
```

## Comparing `ocsf_validator-0.1.5.tar` & `ocsf_validator-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    10173 2024-01-08 22:46:31.782602 ocsf_validator-0.1.5/LICENSE
--rw-r--r--   0        0        0     4205 2024-03-12 19:08:15.440332 ocsf_validator-0.1.5/README.md
--rw-r--r--   0        0        0      241 2024-01-08 22:46:31.762238 ocsf_validator-0.1.5/ocsf_validator/__init__.py
--rw-r--r--   0        0        0      466 2024-01-08 22:46:31.766527 ocsf_validator-0.1.5/ocsf_validator/__main__.py
--rw-r--r--   0        0        0     6559 2024-03-12 19:08:15.440657 ocsf_validator-0.1.5/ocsf_validator/errors.py
--rw-r--r--   0        0        0     2875 2024-01-08 22:46:31.766194 ocsf_validator-0.1.5/ocsf_validator/matchers.py
--rw-r--r--   0        0        0    16455 2024-01-08 22:46:31.762493 ocsf_validator-0.1.5/ocsf_validator/processor.py
--rw-r--r--   0        0        0     6490 2024-01-08 22:46:31.765757 ocsf_validator-0.1.5/ocsf_validator/reader.py
--rw-r--r--   0        0        0        0 2024-01-08 22:46:31.766272 ocsf_validator-0.1.5/ocsf_validator/repository.py
--rw-r--r--   0        0        0    11510 2024-03-12 19:08:15.441045 ocsf_validator-0.1.5/ocsf_validator/runner.py
--rw-r--r--   0        0        0     1641 2024-01-08 22:46:31.761487 ocsf_validator-0.1.5/ocsf_validator/type_mapping.py
--rw-r--r--   0        0        0     5002 2024-03-12 19:08:15.441525 ocsf_validator-0.1.5/ocsf_validator/types.py
--rw-r--r--   0        0        0    16352 2024-03-12 19:08:15.441988 ocsf_validator-0.1.5/ocsf_validator/validators.py
--rw-r--r--   0        0        0      528 2024-03-12 19:08:15.442795 ocsf_validator-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4603 1970-01-01 00:00:00.000000 ocsf_validator-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-01-08 22:46:31.782602 ocsf_validator-0.1.7/LICENSE
+-rw-r--r--   0        0        0     4209 2024-03-22 16:43:23.019386 ocsf_validator-0.1.7/README.md
+-rw-r--r--   0        0        0      241 2024-01-08 22:46:31.762238 ocsf_validator-0.1.7/ocsf_validator/__init__.py
+-rw-r--r--   0        0        0      584 2024-03-22 16:43:23.019731 ocsf_validator-0.1.7/ocsf_validator/__main__.py
+-rw-r--r--   0        0        0     6728 2024-04-01 21:43:22.127009 ocsf_validator-0.1.7/ocsf_validator/errors.py
+-rw-r--r--   0        0        0     2875 2024-01-08 22:46:31.766194 ocsf_validator-0.1.7/ocsf_validator/matchers.py
+-rw-r--r--   0        0        0    16630 2024-03-22 16:43:23.020467 ocsf_validator-0.1.7/ocsf_validator/processor.py
+-rw-r--r--   0        0        0     6956 2024-03-22 16:43:23.020718 ocsf_validator-0.1.7/ocsf_validator/reader.py
+-rw-r--r--   0        0        0        0 2024-01-08 22:46:31.766272 ocsf_validator-0.1.7/ocsf_validator/repository.py
+-rw-r--r--   0        0        0    12831 2024-03-22 16:43:23.020982 ocsf_validator-0.1.7/ocsf_validator/runner.py
+-rw-r--r--   0        0        0     1641 2024-01-08 22:46:31.761487 ocsf_validator-0.1.7/ocsf_validator/type_mapping.py
+-rw-r--r--   0        0        0     5080 2024-03-22 16:43:23.021178 ocsf_validator-0.1.7/ocsf_validator/types.py
+-rw-r--r--   0        0        0    24002 2024-04-01 21:43:22.127216 ocsf_validator-0.1.7/ocsf_validator/validators.py
+-rw-r--r--   0        0        0      594 2024-04-01 21:43:22.128038 ocsf_validator-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4607 1970-01-01 00:00:00.000000 ocsf_validator-0.1.7/PKG-INFO
```

### Comparing `ocsf_validator-0.1.5/LICENSE` & `ocsf_validator-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ocsf_validator-0.1.5/README.md` & `ocsf_validator-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -75,16 +75,16 @@
 After checking out, you'll want to install dependencies:
 ```
 poetry install
 ```
 
 Before committing, run the formatters and tests:
 ```
-poetry run isort
-poetry run black
+poetry run isort .
+poetry run black .
 poetry run pyright
 poetry run pytest
 ```
 
 If you're adding a validator, do the following:
  - Write your `validate_` function in `validate.py` to apply a function to the relevant keys in a reader that will run your desired validation. See `validators.py` for examples.
  - Add any custom errors in `errors.py`.
```

### Comparing `ocsf_validator-0.1.5/ocsf_validator/errors.py` & `ocsf_validator-0.1.7/ocsf_validator/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,9 +233,14 @@
         super().__init__(cause)
 
 
 class ObservableTypeIDCollisionError(ValidationError):
     def __init__(self, type_id: int, this_def: str, other_defs: list[str], file: str):
         super().__init__(
             f"Collision with observable type_id {type_id} between {this_def}"
-            f" in file {file} and {', '.join(other_defs)}"
+            f" in file {file} and {', '.join(other_defs)}."
         )
+
+
+class UnknownCategoryError(ValidationError):
+    def __init__(self, category: str, file: str):
+        super().__init__(f'Unknown category "{category}" in "{file}"')
```

### Comparing `ocsf_validator-0.1.5/ocsf_validator/matchers.py` & `ocsf_validator-0.1.7/ocsf_validator/matchers.py`

 * *Files identical despite different names*

### Comparing `ocsf_validator-0.1.5/ocsf_validator/processor.py` & `ocsf_validator-0.1.7/ocsf_validator/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from pathlib import Path
 from typing import Any, Callable, Optional
 
 from ocsf_validator.errors import *
 from ocsf_validator.reader import Reader
 from ocsf_validator.type_mapping import TypeMapping
-from ocsf_validator.types import (ATTRIBUTES_KEY, EXTENDS_KEY, INCLUDE_KEY,
-                                  PROFILES_KEY, OcsfDictionary, OcsfEvent,
-                                  OcsfObject)
+from ocsf_validator.types import (
+    ATTRIBUTES_KEY,
+    EXTENDS_KEY,
+    INCLUDE_KEY,
+    PROFILES_KEY,
+    OcsfDictionary,
+    OcsfEvent,
+    OcsfObject,
+)
 
 
 def deep_merge(
     subj: dict[str, Any], other: dict[str, Any], exclude: Optional[set[str]] = None
 ):
     """Recursive merging of dictionary keys.
 
@@ -60,15 +66,16 @@
 
         filenames = [target]
         if Path(target).suffix != ".json":
             filenames.append(target + ".json")
 
         for file in filenames:
             if relative_to is not None:
-                # Search extension for relative include path, e.g. /includes/thing.json -> /extensions/stuff/includes/thing.json
+                # Search extension for relative include path,
+                # e.g. /includes/thing.json -> /extensions/stuff/includes/thing.json
                 extn = self._types.extension(relative_to)
                 if extn is not None:
                     k = self._reader.key("extensions", extn, file)
                     if k in self._reader:
                         return k
 
             k = self._reader.key(file)
@@ -243,16 +250,18 @@
 
         return []
 
 
 class ProfilesParser(MergeParser):
     def applies_to(self, t: type) -> bool:
         if hasattr(t, "__required_keys__") or hasattr(t, "__optional_keys"):
-            return PROFILES_KEY in t.__required_keys__ or PROFILES_KEY in t.__optional_keys__  # type: ignore
-
+            return (
+                PROFILES_KEY in t.__required_keys__
+                or PROFILES_KEY in t.__optional_keys__  # type: ignore
+            )
         else:
             return False
 
     def found_in(self, path: str) -> bool:
         return PROFILES_KEY in self._reader[path]
 
     def extract_targets(self, path: str) -> list[str]:
@@ -271,15 +280,18 @@
 
         return targets
 
 
 class AttributesParser(MergeParser):
     def applies_to(self, t: type) -> bool:
         if hasattr(t, "__required_keys__") or hasattr(t, "__optional_keys"):
-            return ATTRIBUTES_KEY in t.__required_keys__ or ATTRIBUTES_KEY in t.__optional_keys__  # type: ignore
+            return (
+                ATTRIBUTES_KEY in t.__required_keys__
+                or ATTRIBUTES_KEY in t.__optional_keys__  # type: ignore
+            )
         else:
             return False
 
     def found_in(self, path: str) -> bool:
         return ATTRIBUTES_KEY in self._reader[path]
 
     def extract_targets(self, path: str) -> list[str]:
@@ -304,25 +316,32 @@
         return {}
 
     def apply(self, path: str):
         attrs = self._reader[path][ATTRIBUTES_KEY]
         root = self._root_dict()
         extn = self._extn_dict(path)
 
-        # TODO is the dict name comparison enough or do we need to find by the `name` key?
+        # TODO is the dict name comparison enough
+        #      or do we need to find by the `name` key?
         for name, attr in attrs.items():
             if name in extn:
                 deep_merge(attrs[name], extn[name])
             if name in root:
                 deep_merge(attrs[name], root[name])
 
 
 class IncludeParser(MergeParser):
     def applies_to(self, t: type) -> bool:
-        return ("__required_keys__" in t.__dict__ and INCLUDE_KEY in t.__required_keys__) or ("__optional_keys__" in t.__dict__ and INCLUDE_KEY in t.__optional_keys__)  # type: ignore
+        return (
+            "__required_keys__" in t.__dict__
+            and INCLUDE_KEY in t.__required_keys__  # type: ignore
+        ) or (
+            "__optional_keys__" in t.__dict__
+            and INCLUDE_KEY in t.__optional_keys__  # type: ignore
+        )
 
     def _has_includes(self, defn: dict[str, Any]) -> bool:
         """Recursively search for $include directives."""
         keys = list(defn.keys())
         for k in keys:
             if k == INCLUDE_KEY:
                 return True
```

### Comparing `ocsf_validator-0.1.5/ocsf_validator/reader.py` & `ocsf_validator-0.1.7/ocsf_validator/reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,24 +2,21 @@
 
 This module contains tools to work with the JSON files that define the OCSF
 schema. The most important export is the `Reader` class, which allows convenient
 access to the OCSF schema as its represented in the definition files.
 """
 
 import json
-import re
 from abc import ABC
 from dataclasses import dataclass
-from enum import IntEnum
-from pathlib import Path, PurePath
+from pathlib import Path
 from typing import Any, Callable, Dict, Iterable, Optional
 
 from ocsf_validator.errors import InvalidBasePathError
 from ocsf_validator.matchers import Matcher
-from ocsf_validator.types import *
 
 # TODO would os.PathLike be better?
 Pathable = str | Path
 
 # TODO refine Any in type signature
 SchemaData = Dict[str, Any]
 
@@ -29,14 +26,17 @@
 @dataclass
 class ReaderOptions:
     """Options to control the behavior of a Reader."""
 
     base_path: Optional[Path] = None
     """The base path from which to load the schema."""
 
+    metaschema_path: Optional[Path] = None
+    """The metaschema path from which to load the metaschema."""
+
     read_extensions: bool = True
     """Recurse extensions."""
 
 
 class Reader(ABC):
     """An in-memory copy of the raw OCSF schema definition.
 
@@ -54,27 +54,33 @@
     def __init__(self, options: ReaderOptions | Pathable | None = None) -> None:
         if options is not None:
             if not isinstance(options, ReaderOptions):
                 if isinstance(options, str):
                     path = Path(options)
                 else:
                     path = options
-                options = ReaderOptions(base_path=path)
+                options = ReaderOptions(
+                    base_path=path, metaschema_path=(path / "metaschema")
+                )
 
             self._options = options
         else:
             self._options = ReaderOptions()
 
         self._data: SchemaData = {}
         self._root: str = ""
 
     @property
     def base_path(self):
         return self._options.base_path
 
+    @property
+    def metaschema_path(self):
+        return self._options.metaschema_path
+
     def contents(self, path: Pathable) -> SchemaData:
         """Retrieve the parsed JSON data in a given file."""
         if isinstance(path, Path):
             path = str(path)
 
         # Can raise KeyError
         return self.__getitem__(path)
@@ -152,14 +158,23 @@
 
 
 class DictReader(Reader):
     """A Reader that works from a `dict` without reading the filesystem.
 
     Useful (hopefully) for testing and debugging."""
 
+    def __init__(
+        self, options: ReaderOptions | Pathable | SchemaData | None = None
+    ) -> None:
+        if isinstance(options, dict):
+            super().__init__(None)
+            self.set_data(options)
+        else:
+            super().__init__(options)
+
     def set_data(self, data: SchemaData):
         self._data = data.copy()
         self._root = Path(next(iter(self._data.keys()))).root
 
 
 class FileReader(Reader):
     """A Reader that reads schema definitions from JSON files."""
```

### Comparing `ocsf_validator-0.1.5/ocsf_validator/runner.py` & `ocsf_validator-0.1.7/ocsf_validator/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-"""Validate OCSF Schema definitions.
-
+"""
+Validate OCSF Schema definitions.
 """
 
 import traceback
 from dataclasses import dataclass
 from enum import IntEnum
 from pathlib import Path
 from typing import Callable
@@ -12,14 +12,15 @@
 
 import ocsf_validator.errors as errors
 from ocsf_validator.processor import process_includes
 from ocsf_validator.reader import FileReader, ReaderOptions
 from ocsf_validator.type_mapping import TypeMapping
 from ocsf_validator.validators import (
     validate_attr_types,
+    validate_event_categories,
     validate_include_targets,
     validate_intra_type_collisions,
     validate_metaschemas,
     validate_no_unknown_keys,
     validate_observables,
     validate_required_keys,
     validate_undefined_attrs,
@@ -37,14 +38,17 @@
 @dataclass
 class ValidatorOptions:
     """Configure validator behavior."""
 
     base_path: str = "."
     """The base path of the schema."""
 
+    metaschema_path: str = None
+    """The path to the schema's metaschema."""
+
     extensions: bool = True
     """Include the contents of extensions."""
 
     strict: bool = False
     """When True, exit with a non-zero exit code when warnings are encountered."""
 
     show_info: bool = False
@@ -62,15 +66,16 @@
     missing_profile: int = Severity.ERROR
     """A `profiles` target is missing."""
 
     missing_inheritance: int = Severity.ERROR
     """An `extends` inheritance target is missing."""
 
     imprecise_inheritance: int = Severity.INFO
-    """An `extends` inheritance target is resolvable but imprecise and possibly ambiguous."""
+    """An `extends` inheritance target is resolvable
+    but imprecise and possibly ambiguous."""
 
     missing_key: int = Severity.ERROR
     """A required key is missing."""
 
     unknown_key: int = Severity.ERROR
     """An unrecognized key was found."""
 
@@ -103,14 +108,17 @@
 
     illegal_observable: int = Severity.ERROR
     """Observable type_id illegally defined."""
 
     observable_collision: int = Severity.ERROR
     """Colliding observable type_id defined."""
 
+    unknown_category: int = Severity.ERROR
+    """Unknown category."""
+
     def severity(self, err: Exception):
         match type(err):
             case errors.MissingRequiredKeyError:
                 return self.missing_key
             case errors.UnknownKeyError:
                 return self.unknown_key
             case errors.MissingIncludeError:
@@ -143,14 +151,16 @@
                 return self.invalid_metaschema_file
             case errors.InvalidAttributeTypeError:
                 return self.invalid_attr_types
             case errors.IllegalObservableTypeIDError:
                 return self.illegal_observable
             case errors.ObservableTypeIDCollisionError:
                 return self.observable_collision
+            case errors.UnknownCategoryError:
+                return self.unknown_category
             case _:
                 return Severity.INFO
 
 
 class ValidationRunner:
     def __init__(self, pathOrOptions: str | ValidatorOptions):
         if isinstance(pathOrOptions, str):
@@ -229,20 +239,37 @@
 
             if message:
                 print(message)
 
         try:
             print(self.txt_emphasize("===[ OCSF Schema Validator ]==="))
             print(
-                "Validating OCSF Schema at", self.txt_highlight(self.options.base_path)
+                "Validating OCSF Schema at:", self.txt_highlight(self.options.base_path)
             )
+            b_path = Path(self.options.base_path)
+            if not b_path.is_absolute():
+                print("  Absolute path:", str(b_path.resolve()))
+            if self.options.metaschema_path is not None:
+                print(
+                    "Using metaschema at:",
+                    self.txt_highlight(self.options.metaschema_path),
+                )
+                m_path = Path(self.options.metaschema_path)
+                if not m_path.is_absolute():
+                    print("  Absolute path:", str(m_path.resolve()))
 
             # Setup the reader
+            base_path = Path(self.options.base_path)
+            if self.options.metaschema_path is None:
+                metaschema_path = base_path / "metaschema"
+            else:
+                metaschema_path = Path(self.options.metaschema_path)
             opts = ReaderOptions(
-                base_path=Path(self.options.base_path),
+                base_path=base_path,
+                metaschema_path=metaschema_path,
                 read_extensions=self.options.extensions,
             )
             reader = None
             try:
                 reader = FileReader(opts)
             except errors.ValidationError as err:
                 collector.handle(err)
@@ -310,14 +337,21 @@
 
             test(
                 "Attribute type references are defined",
                 lambda: validate_attr_types(reader, collector=collector, types=types),
             )
 
             test(
+                "Event class categories are defined",
+                lambda: validate_event_categories(
+                    reader, collector=collector, types=types
+                ),
+            )
+
+            test(
                 "JSON files match their metaschema definitions",
                 lambda: validate_metaschemas(reader, collector=collector, types=types),
             )
 
         except Exception as err:
             print("Encountered an unexpected exception:")
             traceback.print_exception(err)
```

### Comparing `ocsf_validator-0.1.5/ocsf_validator/type_mapping.py` & `ocsf_validator-0.1.7/ocsf_validator/type_mapping.py`

 * *Files identical despite different names*

### Comparing `ocsf_validator-0.1.5/ocsf_validator/types.py` & `ocsf_validator-0.1.7/ocsf_validator/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     Sequence,
     TypedDict,
     TypeVar,
     Union,
 )
 
 ATTRIBUTES_KEY = "attributes"
+CATEGORY_KEY = "category"
 PROFILES_KEY = "profiles"
 EXTENDS_KEY = "extends"
 INCLUDE_KEY = "$include"
 OBSERVABLE_KEY = "observable"
 OBSERVABLES_KEY = "observables"
 TYPES_KEY = "types"
 
@@ -127,14 +128,15 @@
         "description": str,
         "name": str,
         "attributes": Dict[str, OcsfAttr],
         "extends": NotRequired[Union[str, list[Optional[str]]]],
         "observable": NotRequired[int],
         "profiles": NotRequired[Sequence[str]],
         "constraints": NotRequired[Dict[str, Sequence[str]]],
+        "observables": NotRequired[Dict[str, int]],
         "$include": NotRequired[Union[str, Sequence[str]]],
         "@deprecated": NotRequired[OcsfDeprecationInfo],
     },
 )
 
 
 OcsfEvent = TypedDict(
```

### Comparing `ocsf_validator-0.1.5/PKG-INFO` & `ocsf_validator-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocsf-validator
-Version: 0.1.5
+Version: 0.1.7
 Summary: OCSF Schema Validation
 Author: Jeremy Fisher
 Author-email: jeremy@query.ai
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jsonschema (>=4.21.1,<5.0.0)
@@ -88,16 +88,16 @@
 After checking out, you'll want to install dependencies:
 ```
 poetry install
 ```
 
 Before committing, run the formatters and tests:
 ```
-poetry run isort
-poetry run black
+poetry run isort .
+poetry run black .
 poetry run pyright
 poetry run pytest
 ```
 
 If you're adding a validator, do the following:
  - Write your `validate_` function in `validate.py` to apply a function to the relevant keys in a reader that will run your desired validation. See `validators.py` for examples.
  - Add any custom errors in `errors.py`.
```

