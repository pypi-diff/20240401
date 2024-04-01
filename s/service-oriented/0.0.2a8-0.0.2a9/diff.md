# Comparing `tmp/service_oriented-0.0.2a8.tar.gz` & `tmp/service_oriented-0.0.2a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "service_oriented-0.0.2a8.tar", last modified: Sun Jan 28 13:14:18 2024, max compression
+gzip compressed data, was "service_oriented-0.0.2a9.tar", last modified: Sun Jan 28 14:12:50 2024, max compression
```

## Comparing `service_oriented-0.0.2a8.tar` & `service_oriented-0.0.2a9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 13:14:18.426633 service_oriented-0.0.2a8/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-28 13:13:37.000000 service_oriented-0.0.2a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-28 13:13:37.000000 service_oriented-0.0.2a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-01-28 13:14:18.426633 service_oriented-0.0.2a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-28 13:13:37.000000 service_oriented-0.0.2a8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-28 13:13:37.000000 service_oriented-0.0.2a8/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-28 13:13:37.000000 service_oriented-0.0.2a8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 13:14:18.418634 service_oriented-0.0.2a8/service_oriented/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-01-28 13:13:37.000000 service_oriented-0.0.2a8/service_oriented/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 13:14:18.422634 service_oriented-0.0.2a8/service_oriented/application/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-28 13:13:37.000000 service_oriented-0.0.2a8/service_oriented/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-01-28 13:13:37.000000 service_oriented-0.0.2a8/service_oriented/application/base_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 13:14:18.422634 service_oriented-0.0.2a8/service_oriented/application/config/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-28 13:13:37.000000 service_oriented-0.0.2a8/service_oriented/application/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-01-28 13:13:37.000000 service_oriented-0.0.2a8/service_oriented/application/config/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-01-28 13:13:37.000000 service_oriented-0.0.2a8/service_oriented/application/config/yaml_config_settings_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-01-28 13:13:37.000000 service_oriented-0.0.2a8/service_oriented/application/entry_point_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-01-28 13:13:37.000000 service_oriented-0.0.2a8/service_oriented/deployment_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 13:13:37.000000 service_oriented-0.0.2a8/service_oriented/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 13:14:18.422634 service_oriented-0.0.2a8/service_oriented.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-01-28 13:14:18.000000 service_oriented-0.0.2a8/service_oriented.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-01-28 13:14:18.000000 service_oriented-0.0.2a8/service_oriented.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 13:14:18.000000 service_oriented-0.0.2a8/service_oriented.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-01-28 13:14:18.000000 service_oriented-0.0.2a8/service_oriented.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-28 13:14:18.000000 service_oriented-0.0.2a8/service_oriented.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-28 13:14:18.426633 service_oriented-0.0.2a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-01-28 13:13:37.000000 service_oriented-0.0.2a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:12:50.990145 service_oriented-0.0.2a9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-01-28 14:12:50.990145 service_oriented-0.0.2a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:12:50.982145 service_oriented-0.0.2a9/service_oriented/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:12:50.982145 service_oriented-0.0.2a9/service_oriented/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/application/base_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:12:50.982145 service_oriented-0.0.2a9/service_oriented/application/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/application/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/application/config/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/application/config/yaml_config_settings_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/application/entry_point_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/deployment_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:12:50.982145 service_oriented-0.0.2a9/service_oriented.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-01-28 14:12:50.000000 service_oriented-0.0.2a9/service_oriented.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-01-28 14:12:50.000000 service_oriented-0.0.2a9/service_oriented.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 14:12:50.000000 service_oriented-0.0.2a9/service_oriented.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-01-28 14:12:50.000000 service_oriented-0.0.2a9/service_oriented.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-28 14:12:50.000000 service_oriented-0.0.2a9/service_oriented.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-28 14:12:50.990145 service_oriented-0.0.2a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/setup.py
```

### Comparing `service_oriented-0.0.2a8/LICENSE` & `service_oriented-0.0.2a9/LICENSE`

 * *Files identical despite different names*

### Comparing `service_oriented-0.0.2a8/PKG-INFO` & `service_oriented-0.0.2a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: service_oriented
-Version: 0.0.2a8
+Version: 0.0.2a9
 Summary: Toolkit for building service oriented applications in python
 Home-page: https://github.com/tdg5/service-oriented-py
 Author: Danny Guinther
 Author-email: dannyguinther@gmail.com
 License: MIT
 Keywords: [TODO]
 Classifier: Intended Audience :: Developers
```

### Comparing `service_oriented-0.0.2a8/pyproject.toml` & `service_oriented-0.0.2a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `service_oriented-0.0.2a8/service_oriented/application/base_application.py` & `service_oriented-0.0.2a9/service_oriented/application/base_application.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,37 @@
-from typing import Dict, Generic, TypeVar
+from typing import Any, Dict, Generic, Optional, TypeVar
 
 from service_oriented.application.config import BaseConfig
 from service_oriented.application.entry_point_spec import EntryPointSpec
 
 
 C = TypeVar("C", bound=BaseConfig)
-E = TypeVar("E", bound=EntryPointSpec)
 
 
 class BaseApplication(Generic[C]):
+    default_entry_points: Dict[str, EntryPointSpec] = {}
+
+    @classmethod
+    def __init_subclass__(
+        cls,
+        entry_points: Optional[Dict[str, EntryPointSpec]] = None,
+        **kwargs: Any,
+    ):
+        super().__init_subclass__(**kwargs)
+        _entry_points = entry_points or {}
+        cls.default_entry_points = _entry_points
+
     def __init__(
         self,
         config: C,
-        entry_points: Dict[str, E],
+        entry_points: Optional[Dict[str, EntryPointSpec]] = None,
     ):
         self.config: C = config
-        self.entry_points: Dict[str, E] = entry_points
+        _entry_points = entry_points or {}
+        self.entry_points = {**self.default_entry_points, **_entry_points}
 
     def run(self) -> None:
         entry_point_name = self.config.entry_point
         entry_point_spec = self.entry_points.get(entry_point_name)
         if entry_point_spec is None:
             raise RuntimeError(
                 f"No mapping found for entry point named '{entry_point_name}'"
```

### Comparing `service_oriented-0.0.2a8/service_oriented/application/config/base_config.py` & `service_oriented-0.0.2a9/service_oriented/application/config/base_config.py`

 * *Files identical despite different names*

### Comparing `service_oriented-0.0.2a8/service_oriented/application/config/yaml_config_settings_source.py` & `service_oriented-0.0.2a9/service_oriented/application/config/yaml_config_settings_source.py`

 * *Files identical despite different names*

### Comparing `service_oriented-0.0.2a8/service_oriented/application/entry_point_spec.py` & `service_oriented-0.0.2a9/service_oriented/application/entry_point_spec.py`

 * *Files identical despite different names*

### Comparing `service_oriented-0.0.2a8/service_oriented/deployment_environment.py` & `service_oriented-0.0.2a9/service_oriented/deployment_environment.py`

 * *Files identical despite different names*

### Comparing `service_oriented-0.0.2a8/service_oriented.egg-info/PKG-INFO` & `service_oriented-0.0.2a9/service_oriented.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: service_oriented
-Version: 0.0.2a8
+Version: 0.0.2a9
 Summary: Toolkit for building service oriented applications in python
 Home-page: https://github.com/tdg5/service-oriented-py
 Author: Danny Guinther
 Author-email: dannyguinther@gmail.com
 License: MIT
 Keywords: [TODO]
 Classifier: Intended Audience :: Developers
```

### Comparing `service_oriented-0.0.2a8/service_oriented.egg-info/SOURCES.txt` & `service_oriented-0.0.2a9/service_oriented.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `service_oriented-0.0.2a8/service_oriented.egg-info/requires.txt` & `service_oriented-0.0.2a9/service_oriented.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `service_oriented-0.0.2a8/setup.py` & `service_oriented-0.0.2a9/setup.py`

 * *Files identical despite different names*

