# Comparing `tmp/retrack-2.3.2.tar.gz` & `tmp/retrack-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retrack-2.3.2.tar", max compression
+gzip compressed data, was "retrack-2.4.0.tar", max compression
```

## Comparing `retrack-2.3.2.tar` & `retrack-2.4.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1072 2024-03-12 17:34:44.856879 retrack-2.3.2/LICENSE
--rw-r--r--   0        0        0     4374 2024-03-12 17:34:44.856879 retrack-2.3.2/README.md
--rw-r--r--   0        0        0      869 2024-03-12 17:34:44.856879 retrack-2.3.2/pyproject.toml
--rw-r--r--   0        0        0      617 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/__init__.py
--rw-r--r--   0        0        0        0 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/engine/__init__.py
--rw-r--r--   0        0        0     2954 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/engine/base.py
--rw-r--r--   0        0        0     1689 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/engine/constructor.py
--rw-r--r--   0        0        0     8654 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/engine/executor.py
--rw-r--r--   0        0        0     4688 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/engine/request_manager.py
--rw-r--r--   0        0        0     3561 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/engine/rule.py
--rw-r--r--   0        0        0     2639 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/engine/schemas.py
--rw-r--r--   0        0        0     2590 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/__init__.py
--rw-r--r--   0        0        0     2197 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/base.py
--rw-r--r--   0        0        0     2681 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/check.py
--rw-r--r--   0        0        0      689 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/connectors.py
--rw-r--r--   0        0        0     3879 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/constants.py
--rw-r--r--   0        0        0      873 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/contains.py
--rw-r--r--   0        0        0      950 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/datetime.py
--rw-r--r--   0        0        0      657 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/dynamic/__init__.py
--rw-r--r--   0        0        0      813 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/dynamic/base.py
--rw-r--r--   0        0        0     2597 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/dynamic/csv_table.py
--rw-r--r--   0        0        0     2462 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/dynamic/flow.py
--rw-r--r--   0        0        0      910 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/endswith.py
--rw-r--r--   0        0        0      941 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/endswithany.py
--rw-r--r--   0        0        0      687 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/getchar.py
--rw-r--r--   0        0        0     1009 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/inputs.py
--rw-r--r--   0        0        0     1606 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/logic.py
--rw-r--r--   0        0        0      580 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/lowercase.py
--rw-r--r--   0        0        0     1054 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/match.py
--rw-r--r--   0        0        0     3035 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/math.py
--rw-r--r--   0        0        0     1102 2024-03-12 17:34:44.856879 retrack-2.3.2/retrack/nodes/outputs.py
--rw-r--r--   0        0        0      581 2024-03-12 17:34:44.860879 retrack-2.3.2/retrack/nodes/start.py
--rw-r--r--   0        0        0      926 2024-03-12 17:34:44.860879 retrack-2.3.2/retrack/nodes/startswith.py
--rw-r--r--   0        0        0      957 2024-03-12 17:34:44.860879 retrack-2.3.2/retrack/nodes/startswithany.py
--rw-r--r--   0        0        0     1072 2024-03-12 17:34:44.860879 retrack-2.3.2/retrack/nodes/substring.py
--rw-r--r--   0        0        0        0 2024-03-12 17:34:44.860879 retrack-2.3.2/retrack/utils/__init__.py
--rw-r--r--   0        0        0     5198 2024-03-12 17:34:44.860879 retrack-2.3.2/retrack/utils/component_registry.py
--rw-r--r--   0        0        0      204 2024-03-12 17:34:44.860879 retrack-2.3.2/retrack/utils/constants.py
--rw-r--r--   0        0        0     3685 2024-03-12 17:34:44.860879 retrack-2.3.2/retrack/utils/exceptions.py
--rw-r--r--   0        0        0     3585 2024-03-12 17:34:44.860879 retrack-2.3.2/retrack/utils/graph.py
--rw-r--r--   0        0        0     1324 2024-03-12 17:34:44.860879 retrack-2.3.2/retrack/utils/registry.py
--rw-r--r--   0        0        0      154 2024-03-12 17:34:44.860879 retrack-2.3.2/retrack/utils/transformers.py
--rw-r--r--   0        0        0      521 2024-03-12 17:34:44.860879 retrack-2.3.2/retrack/validators/__init__.py
--rw-r--r--   0        0        0      267 2024-03-12 17:34:44.860879 retrack-2.3.2/retrack/validators/base.py
--rw-r--r--   0        0        0      407 2024-03-12 17:34:44.860879 retrack-2.3.2/retrack/validators/check_is_dag.py
--rw-r--r--   0        0        0     1296 2024-03-12 17:34:44.860879 retrack-2.3.2/retrack/validators/node_exists.py
--rw-r--r--   0        0        0     5215 1970-01-01 00:00:00.000000 retrack-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-01 19:49:57.475275 retrack-2.4.0/LICENSE
+-rw-r--r--   0        0        0     4374 2024-04-01 19:49:57.475275 retrack-2.4.0/README.md
+-rw-r--r--   0        0        0      869 2024-04-01 19:49:57.475275 retrack-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      617 2024-04-01 19:49:57.475275 retrack-2.4.0/retrack/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:49:57.475275 retrack-2.4.0/retrack/engine/__init__.py
+-rw-r--r--   0        0        0     2954 2024-04-01 19:49:57.475275 retrack-2.4.0/retrack/engine/base.py
+-rw-r--r--   0        0        0     1689 2024-04-01 19:49:57.475275 retrack-2.4.0/retrack/engine/constructor.py
+-rw-r--r--   0        0        0     8654 2024-04-01 19:49:57.475275 retrack-2.4.0/retrack/engine/executor.py
+-rw-r--r--   0        0        0     4678 2024-04-01 19:49:57.475275 retrack-2.4.0/retrack/engine/request_manager.py
+-rw-r--r--   0        0        0     3561 2024-04-01 19:49:57.475275 retrack-2.4.0/retrack/engine/rule.py
+-rw-r--r--   0        0        0     2639 2024-04-01 19:49:57.475275 retrack-2.4.0/retrack/engine/schemas.py
+-rw-r--r--   0        0        0     2552 2024-04-01 19:49:57.475275 retrack-2.4.0/retrack/nodes/__init__.py
+-rw-r--r--   0        0        0     2197 2024-04-01 19:49:57.475275 retrack-2.4.0/retrack/nodes/base.py
+-rw-r--r--   0        0        0     2681 2024-04-01 19:49:57.475275 retrack-2.4.0/retrack/nodes/check.py
+-rw-r--r--   0        0        0      449 2024-04-01 19:49:57.475275 retrack-2.4.0/retrack/nodes/connectors.py
+-rw-r--r--   0        0        0     3879 2024-04-01 19:49:57.475275 retrack-2.4.0/retrack/nodes/constants.py
+-rw-r--r--   0        0        0      873 2024-04-01 19:49:57.475275 retrack-2.4.0/retrack/nodes/contains.py
+-rw-r--r--   0        0        0      950 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/datetime.py
+-rw-r--r--   0        0        0      657 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/dynamic/__init__.py
+-rw-r--r--   0        0        0      813 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/dynamic/base.py
+-rw-r--r--   0        0        0     2597 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/dynamic/csv_table.py
+-rw-r--r--   0        0        0     2462 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/dynamic/flow.py
+-rw-r--r--   0        0        0      910 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/endswith.py
+-rw-r--r--   0        0        0      941 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/endswithany.py
+-rw-r--r--   0        0        0      709 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/getchar.py
+-rw-r--r--   0        0        0     1009 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/inputs.py
+-rw-r--r--   0        0        0     1606 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/logic.py
+-rw-r--r--   0        0        0      580 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/lowercase.py
+-rw-r--r--   0        0        0     1054 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/match.py
+-rw-r--r--   0        0        0     3035 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/math.py
+-rw-r--r--   0        0        0     1102 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/outputs.py
+-rw-r--r--   0        0        0      581 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/start.py
+-rw-r--r--   0        0        0      926 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/startswith.py
+-rw-r--r--   0        0        0      957 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/startswithany.py
+-rw-r--r--   0        0        0     1072 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/nodes/substring.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/utils/__init__.py
+-rw-r--r--   0        0        0     5198 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/utils/component_registry.py
+-rw-r--r--   0        0        0      204 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/utils/constants.py
+-rw-r--r--   0        0        0     3685 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/utils/exceptions.py
+-rw-r--r--   0        0        0     3585 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/utils/graph.py
+-rw-r--r--   0        0        0     1324 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/utils/registry.py
+-rw-r--r--   0        0        0      154 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/utils/transformers.py
+-rw-r--r--   0        0        0      521 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/validators/__init__.py
+-rw-r--r--   0        0        0      267 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/validators/base.py
+-rw-r--r--   0        0        0      407 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/validators/check_is_dag.py
+-rw-r--r--   0        0        0     1296 2024-04-01 19:49:57.479275 retrack-2.4.0/retrack/validators/node_exists.py
+-rw-r--r--   0        0        0     5215 1970-01-01 00:00:00.000000 retrack-2.4.0/PKG-INFO
```

### Comparing `retrack-2.3.2/LICENSE` & `retrack-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/README.md` & `retrack-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/pyproject.toml` & `retrack-2.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "retrack"
-version = "2.3.2"
+version = "2.4.0"
 description = "A business rules engine"
 authors = ["Gabriel Guarisa <gabriel.guarisa@pier.digital>", "Nathalia Trotte <nathaliatrotte@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pier-digital/retrack"
 homepage = "https://github.com/pier-digital/retrack"
 keywords = ["rules", "models", "business", "node", "graph"]
```

### Comparing `retrack-2.3.2/retrack/__init__.py` & `retrack-2.4.0/retrack/__init__.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/engine/base.py` & `retrack-2.4.0/retrack/engine/base.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/engine/constructor.py` & `retrack-2.4.0/retrack/engine/constructor.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/engine/executor.py` & `retrack-2.4.0/retrack/engine/executor.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/engine/request_manager.py` & `retrack-2.4.0/retrack/engine/request_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         input_names = set()
         formated_inputs = []
 
         for i in range(len(inputs)):
             if not isinstance(inputs[i], BaseNode):
                 raise TypeError(
-                    f"inputs[{i}] must be a dict or an InputModel, not {type(inputs[i])}"
+                    f"inputs[{i}] must be an InputModel, not {type(inputs[i])}"
                 )
 
             if inputs[i].kind() != NodeKind.INPUT:
                 raise TypeError(
                     f"inputs[{i}] must be an InputModel, not {type(inputs[i])}"
                 )
```

### Comparing `retrack-2.3.2/retrack/engine/rule.py` & `retrack-2.4.0/retrack/engine/rule.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/engine/schemas.py` & `retrack-2.4.0/retrack/engine/schemas.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/__init__.py` & `retrack-2.4.0/retrack/nodes/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from retrack.nodes.base import BaseNode
 from retrack.nodes.check import Check
-from retrack.nodes.connectors import BaseConnector, VirtualConnector
+from retrack.nodes.connectors import BaseConnector
 from retrack.nodes.constants import Bool, Constant, IntervalCatV0, List
 from retrack.nodes.contains import Contains
 from retrack.nodes.datetime import CurrentYear
 from retrack.nodes.dynamic import BaseDynamicNode
 from retrack.nodes.dynamic import registry as dynamic_nodes_registry
 from retrack.nodes.endswith import EndsWith
 from retrack.nodes.endswithany import EndsWithAny
@@ -23,19 +23,17 @@
 
 
 def registry() -> Registry:
     """Create a registry with all the nodes available in the library."""
     _registry = Registry()
 
     _registry.register("Input", Input)
+    _registry.register("Connector", BaseConnector)  # By default, Connector is an Input
     _registry.register(
-        "Connector", VirtualConnector
-    )  # By default, Connector is an Input
-    _registry.register(
-        "ConnectorV0", VirtualConnector
+        "ConnectorV0", BaseConnector
     )  # By default, Connector is an Input
     _registry.register("Start", Start)
     _registry.register("Constant", Constant)
     _registry.register("List", List)
     _registry.register("Bool", Bool)
     _registry.register("Output", Output)
     _registry.register("Check", Check)
```

### Comparing `retrack-2.3.2/retrack/nodes/base.py` & `retrack-2.4.0/retrack/nodes/base.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/check.py` & `retrack-2.4.0/retrack/nodes/check.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/constants.py` & `retrack-2.4.0/retrack/nodes/constants.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/contains.py` & `retrack-2.4.0/retrack/nodes/contains.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/datetime.py` & `retrack-2.4.0/retrack/nodes/datetime.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/dynamic/__init__.py` & `retrack-2.4.0/retrack/nodes/dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/dynamic/base.py` & `retrack-2.4.0/retrack/nodes/dynamic/base.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/dynamic/csv_table.py` & `retrack-2.4.0/retrack/nodes/dynamic/csv_table.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/dynamic/flow.py` & `retrack-2.4.0/retrack/nodes/dynamic/flow.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/endswith.py` & `retrack-2.4.0/retrack/nodes/endswith.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/endswithany.py` & `retrack-2.4.0/retrack/nodes/endswithany.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/getchar.py` & `retrack-2.4.0/retrack/nodes/getchar.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,8 +23,10 @@
     outputs: GetCharOutputsModel
     data: GetCharMetadataModel
 
     def run(
         self,
         input_value: pd.Series,
     ) -> typing.Dict[str, pd.Series]:
-        return {"output_value": input_value.apply(lambda x: str(x)[self.data.index - 1])}
+        return {
+            "output_value": input_value.apply(lambda x: str(x)[self.data.index - 1])
+        }
```

### Comparing `retrack-2.3.2/retrack/nodes/inputs.py` & `retrack-2.4.0/retrack/nodes/inputs.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/logic.py` & `retrack-2.4.0/retrack/nodes/logic.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/lowercase.py` & `retrack-2.4.0/retrack/nodes/lowercase.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/match.py` & `retrack-2.4.0/retrack/nodes/match.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/math.py` & `retrack-2.4.0/retrack/nodes/math.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/outputs.py` & `retrack-2.4.0/retrack/nodes/outputs.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/start.py` & `retrack-2.4.0/retrack/nodes/start.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/startswith.py` & `retrack-2.4.0/retrack/nodes/startswith.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/startswithany.py` & `retrack-2.4.0/retrack/nodes/startswithany.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/nodes/substring.py` & `retrack-2.4.0/retrack/nodes/substring.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/utils/component_registry.py` & `retrack-2.4.0/retrack/utils/component_registry.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/utils/exceptions.py` & `retrack-2.4.0/retrack/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/utils/graph.py` & `retrack-2.4.0/retrack/utils/graph.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/utils/registry.py` & `retrack-2.4.0/retrack/utils/registry.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/validators/__init__.py` & `retrack-2.4.0/retrack/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/retrack/validators/node_exists.py` & `retrack-2.4.0/retrack/validators/node_exists.py`

 * *Files identical despite different names*

### Comparing `retrack-2.3.2/PKG-INFO` & `retrack-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retrack
-Version: 2.3.2
+Version: 2.4.0
 Summary: A business rules engine
 Home-page: https://github.com/pier-digital/retrack
 License: MIT
 Keywords: rules,models,business,node,graph
 Author: Gabriel Guarisa
 Author-email: gabriel.guarisa@pier.digital
 Requires-Python: >=3.9,<4.0.0
```

