# Comparing `tmp/haystack_extensions-0.0.3.tar.gz` & `tmp/haystack_extensions-0.0.4.tar.gz`

## Comparing `haystack_extensions-0.0.3.tar` & `haystack_extensions-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 haystack_extensions-0.0.3/src/haystack_extensions/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_extensions-0.0.3/src/haystack_extensions/components/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 haystack_extensions-0.0.3/src/haystack_extensions/components/concurrent_runner/__init__.py
--rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 haystack_extensions-0.0.3/src/haystack_extensions/components/concurrent_runner/runner.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_extensions-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0    10852 2020-02-02 00:00:00.000000 haystack_extensions-0.0.3/tests/test_runner.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 haystack_extensions-0.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 haystack_extensions-0.0.3/LICENSE
--rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 haystack_extensions-0.0.3/README.md
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 haystack_extensions-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 haystack_extensions-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 haystack_extensions-0.0.4/src/haystack_extensions/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_extensions-0.0.4/src/haystack_extensions/components/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 haystack_extensions-0.0.4/src/haystack_extensions/components/concurrent_runner/__init__.py
+-rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 haystack_extensions-0.0.4/src/haystack_extensions/components/concurrent_runner/runner.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_extensions-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0    14327 2020-02-02 00:00:00.000000 haystack_extensions-0.0.4/tests/test_runner.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 haystack_extensions-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 haystack_extensions-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 haystack_extensions-0.0.4/README.md
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 haystack_extensions-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 haystack_extensions-0.0.4/PKG-INFO
```

### Comparing `haystack_extensions-0.0.3/src/haystack_extensions/components/concurrent_runner/runner.py` & `haystack_extensions-0.0.4/src/haystack_extensions/components/concurrent_runner/runner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from concurrent.futures import ThreadPoolExecutor
 from typing import Any, Dict, List, NamedTuple, Optional
 from haystack import Pipeline
 from haystack import component
 from haystack.core.component import Component
-
+from haystack.core.component.sockets import Sockets
+from haystack.core.component import InputSocket, OutputSocket
+from copy import deepcopy
 
 class NamedComponent(NamedTuple):
     name: str
     component: Component
 
 
 class NamedPipeline(NamedTuple):
@@ -30,50 +32,68 @@
             [type(named_component) != NamedComponent for named_component in named_components]
         ):
             raise ValueError("named_components must be a list of NamedComponent instances")
 
         names = [named_component.name for named_component in named_components]
         if len(names) != len(set(names)):
             raise ValueError("All components must have unique names")
+        
+        self._create_input_types(named_components)
+        self._create_output_types(named_components)
 
-        input_types: Dict = {}
-        for named_component in named_components:
-            input_types[named_component.name] = {}
-            socket_dict = named_component.component.__haystack_input__._sockets_dict
-            
-            for key, value in socket_dict.items():
-                input_types[named_component.name][key] = value.type
+        self.executor = executor
+        self.components = named_components
 
-        component.set_input_types(self, **input_types)
 
-        output_types: Dict = {}
+    def _create_input_types(self, named_components: List[NamedComponent]):
+        if not hasattr(self, "__haystack_input__"):
+            self.__haystack_input__ = Sockets(self, {}, InputSocket)
+        
         for named_component in named_components:
-            output_types[named_component.name] = {}
-
-            socket_dict = named_component.component.__haystack_output__._sockets_dict
-
-            for key, value in socket_dict.items():
-                output_types[named_component.name][key] = value.type
-
-        component.set_output_types(self, **output_types)
+            socket_dict = deepcopy(named_component.component.__haystack_input__._sockets_dict)
 
-        self.components = named_components
-        self.executor = executor
+            for name, value in socket_dict.items():
+                value.name = f"{named_component.name}_{name}"
+                self.__haystack_input__[f"{named_component.name}_{name}"] = value
+    
+    def _create_output_types(self, named_components: List[NamedComponent]):
+        if not hasattr(self, "__haystack_output__"):
+            self.__haystack_output__ = Sockets(self, {}, OutputSocket)
+        
+        for named_component in named_components:
+            socket_dict = deepcopy(named_component.component.__haystack_output__._sockets_dict)
+            
+            for name, value in socket_dict.items():
+                value.name = f"{named_component.name}_{name}"
+                self.__haystack_output__[f"{named_component.name}_{name}"] = value
 
     def run(self, **inputs):
         if self.executor is None:
             with ThreadPoolExecutor() as executor:
                 final_results = self._run_in_executor(executor, inputs)
         else:
             final_results = self._run_in_executor(self.executor, inputs)
 
-        return {named_component.name: result for named_component, result in zip(self.components, final_results)}
+        outputs = {}
+        for named_component, result in zip(self.components, final_results):
+            for key, value in result.items():
+                outputs[f"{named_component.name}_{key}"] = value
+
+        return outputs
 
     def _run_in_executor(self, executor, inputs):
-        results = executor.map(lambda c: c[0].component.run(**inputs[c[1]]), zip(self.components, inputs.keys()))
+
+        def _get_real_input(component_name, inputs):
+            real_input = {}
+            for key, value in inputs.items():
+                if key.startswith(component_name):
+                    real_input[key.replace(f"{component_name}_", "")] = value
+            return real_input
+
+        results = executor.map(lambda c: c.component.run(**_get_real_input(c.name, inputs)), self.components)
         return [result for result in results]
 
 
 @component
 class ConcurrentPipelineRunner:
     """
     This component allows you to run multiple pipelines concurrently in a thread pool.
```

### Comparing `haystack_extensions-0.0.3/tests/test_runner.py` & `haystack_extensions-0.0.4/tests/test_runner.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pytest
 from haystack_extensions.components.concurrent_runner.runner import (
     ConcurrentComponentRunner,
     NamedComponent,
     NamedPipeline,
     ConcurrentPipelineRunner,
 )
-from haystack.core.component import Component
+from haystack.components.others import Multiplexer
 from haystack.components.retrievers import InMemoryEmbeddingRetriever
 from haystack.document_stores.in_memory import InMemoryDocumentStore
 
 @component
 class SimpleComponent:
     def __init__(self, wait_time: float, callback: Callable) -> None:
         self.wait_time = wait_time
@@ -32,14 +32,22 @@
     def run(self, some_dict: Dict[str, List[int]], increment: int, number: int = 5) -> Dict[str, Any]:
         return {
             "number": number + increment,
             "as_list": [number + increment],
             "as_dict_of_lists": {key: [number + increment] for key in some_dict.keys()},
         }
 
+@component
+class SimplePrintAndReturnInputComponent:
+    
+    @component.output_types(value=Any)
+    def run(self, value: Any) -> Any:
+        print(value)
+        return {"value": value}
+
 
 class TestConcurrentComponentRunner:
     def test_concurrent_component_runner_with_external_executor(self):
         with ThreadPoolExecutor(max_workers=3) as executor:
             component_call_stack = []
 
             def callback(component):
@@ -55,26 +63,28 @@
 
             pipe = Pipeline()
             pipe.add_component("concurrent_runner", runner)
 
             results = pipe.run(
                 data={
                     "concurrent_runner": {
-                        "component1": {"increment": 1},
-                        "component2": {"increment": 2, "number": 10},
-                        "component3": {"increment": 3, "number": 20},
+                        "component1_increment": 1,
+                        "component2_increment": 2,
+                        "component2_number": 10,
+                        "component3_increment": 3,
+                        "component3_number": 20
                     }
                 }
             )
 
             assert results == {
-                'concurrent_runner': {
-                    'component1': {'number': 6},
-                    'component2': {'number': 12},
-                    'component3': {'number': 23},
+                "concurrent_runner": {
+                    "component1_number": 6,
+                    "component2_number": 12,
+                    "component3_number": 23
                 }
             }
 
             assert len(component_call_stack) == 3
             assert component_call_stack[0] == named_components[2].component
             assert component_call_stack[1] == named_components[0].component
             assert component_call_stack[2] == named_components[1].component
@@ -82,65 +92,161 @@
     def test_concurrent_component_runner(self):
         component_call_stack = []
 
         def callback(component):
             component_call_stack.append(component)
 
         named_components = [
+            NamedComponent(name="c1", component=SimpleComponent(wait_time=0.05, callback=callback)),
+            NamedComponent(name="c2", component=SimpleComponent(wait_time=0.09, callback=callback)),
+            NamedComponent(name="c3", component=SimpleComponent(wait_time=0.01, callback=callback)),
+        ]
+
+        runner = ConcurrentComponentRunner(named_components)
+
+        pipe = Pipeline()
+        pipe.add_component("concurrent_runner", instance=runner)
+
+        results = pipe.run(
+            data={
+                "concurrent_runner": {
+                    "c1_increment": 1,
+                    "c2_increment": 2,
+                    "c2_number": 10,
+                    "c3_increment": 3,
+                    "c3_number": 20
+                }
+            }
+        )
+
+        assert results == {
+            "concurrent_runner": {
+                "c1_number": 6,
+                "c2_number": 12,
+                "c3_number": 23,
+            }
+        }
+
+        assert len(component_call_stack) == 3
+        assert component_call_stack[0] == named_components[2].component
+        assert component_call_stack[1] == named_components[0].component
+        assert component_call_stack[2] == named_components[1].component
+
+    def test_concurrent_component_with_output_connections_runner(self):
+        component_call_stack = []
+
+        def callback(component):
+            component_call_stack.append(component)
+
+        named_components = [
             NamedComponent(name="component1", component=SimpleComponent(wait_time=0.05, callback=callback)),
             NamedComponent(name="component2", component=SimpleComponent(wait_time=0.09, callback=callback)),
             NamedComponent(name="component3", component=SimpleComponent(wait_time=0.01, callback=callback)),
         ]
 
         runner = ConcurrentComponentRunner(named_components)
 
         pipe = Pipeline()
         pipe.add_component("concurrent_runner", runner)
+        pipe.add_component("print_input", SimplePrintAndReturnInputComponent())
+
+        pipe.connect("concurrent_runner.component1_number", "print_input")
 
         results = pipe.run(
             data={
                 "concurrent_runner": {
-                    "component1": {"increment": 1},
-                    "component2": {"increment": 2, "number": 10},
-                    "component3": {"increment": 3, "number": 20},
+                    "component1_increment": 1,
+                    "component2_increment": 2,
+                    "component2_number": 10,
+                    "component3_increment": 3,
+                    "component3_number": 20
                 }
             }
         )
 
         assert results == {
             'concurrent_runner': {
-                'component1': {'number': 6},
-                'component2': {'number': 12},
-                'component3': {'number': 23},
+                'component2_number': 12,
+                'component3_number': 23,
+            },
+            'print_input': {
+                'value': 6
+            }
+        }
+
+    def test_concurrent_component_with_input_connections_runner(self):
+        component_call_stack = []
+
+        def callback(component):
+            component_call_stack.append(component)
+
+        named_components = [
+            NamedComponent(name="component1", component=SimpleComponent(wait_time=0.05, callback=callback)),
+            NamedComponent(name="component2", component=SimpleComponent(wait_time=0.09, callback=callback)),
+            NamedComponent(name="component3", component=SimpleComponent(wait_time=0.01, callback=callback)),
+        ]
+
+        runner = ConcurrentComponentRunner(named_components)
+
+        pipe = Pipeline()
+        pipe.add_component("concurrent_runner", runner)
+        pipe.add_component("multiplexer", Multiplexer(int))
+
+        pipe.connect("multiplexer.value", "concurrent_runner.component1_number")
+
+        results = pipe.run(
+            data={
+                "concurrent_runner": {
+                    "component1_increment": 1,
+                    "component2_increment": 2,
+                    "component2_number": 10,
+                    "component3_increment": 3,
+                    "component3_number": 20,
+                },
+                "multiplexer": {
+                    "value": 12
+                }
+            }
+        )
+
+        assert results == {
+            'concurrent_runner': {
+                'component1_number': 13,
+                'component2_number': 12,
+                'component3_number': 23,
             }
         }
 
-        assert len(component_call_stack) == 3
-        assert component_call_stack[0] == named_components[2].component
-        assert component_call_stack[1] == named_components[0].component
-        assert component_call_stack[2] == named_components[1].component
 
     def test_same_component_name_raises_error(self):
         component1 = NamedComponent("component", SimpleComponent(wait_time=0.1, callback=lambda x: None))
         component2 = NamedComponent("component", SimpleComponent(wait_time=0.1, callback=lambda x: None))
         with pytest.raises(ValueError):
             ConcurrentComponentRunner([component1, component2])
 
     def test_complex_input_output_working(self):
         component = NamedComponent("component", ComplexInputOutputComponent())
         runner = ConcurrentComponentRunner([component])
         pipeline = Pipeline()
         pipeline.add_component("concurrent_runner", runner)
 
         results = pipeline.run(
-            data={"concurrent_runner": {"component": {"some_dict": {"a": [1, 2, 3]}, "increment": 1}}}
+            data={"concurrent_runner": {
+                    "component_some_dict": {"a": [1, 2, 3]},
+                    "component_increment": 1
+                    }
+            }
         )
 
         assert results == {
-            'concurrent_runner': {'component': {'number': 6, 'as_list': [6], 'as_dict_of_lists': {'a': [6]}}}
+            "concurrent_runner": {
+                "component_number": 6,
+                "component_as_list": [6],
+                "component_as_dict_of_lists": {"a": [6]}
+            }
         }
 
     @pytest.mark.parametrize(
         "input",
         [
             ("component", SimpleComponent(wait_time=0.1, callback=lambda x: None)),
             {"component": SimpleComponent(wait_time=0.1, callback=lambda x: None)},
@@ -154,25 +260,27 @@
 
     def test_default_values_are_respected(self):
         component = NamedComponent("component", SimpleComponent(wait_time=0.1, callback=lambda x: None))
         runner = ConcurrentComponentRunner([component])
         pipeline = Pipeline()
         pipeline.add_component("concurrent_runner", runner)
 
-        results = pipeline.run(data={"concurrent_runner": {"component": {"increment": 1}}})
-        assert results == {'concurrent_runner': {'component': {'number': 6}}}
+        results = pipeline.run(data={"concurrent_runner": 
+                                         {"component_increment": 1}
+                                     })
+        assert results == {'concurrent_runner': {'component_number': 6}}
 
     def test_all_retriever_values_copied(self):
         retriever = InMemoryEmbeddingRetriever(InMemoryDocumentStore())
 
         concurrent_retriever = ConcurrentComponentRunner([NamedComponent("retriever", retriever)])
 
         concurrent_retriever.__haystack_input__._sockets_dict
 
-        assert len(retriever.__haystack_input__._sockets_dict) == len(concurrent_retriever.__haystack_input__._sockets_dict["retriever"].type)
+        assert len(retriever.__haystack_input__._sockets_dict) == len(concurrent_retriever.__haystack_input__._sockets_dict)
     
 
 class TestConcurrentPipelineRunner:
     def test_concurrent_pipeline_with_external_executor(self):
         with ThreadPoolExecutor(max_workers=2) as executor:
             component_call_stack = []
 
@@ -262,7 +370,11 @@
             ConcurrentPipelineRunner([("pipeline", [input])])
 
     def test_same_pipeline_name_raises_error(self):
         pipeline1 = NamedPipeline("pipeline", Pipeline())
         pipeline2 = NamedPipeline("pipeline", Pipeline())
         with pytest.raises(ValueError):
             ConcurrentPipelineRunner([pipeline1, pipeline2])
+
+
+if __name__ == "__main__": 
+    TestConcurrentComponentRunner().test_concurrent_component_with_input_connections_runner
```

### Comparing `haystack_extensions-0.0.3/.gitignore` & `haystack_extensions-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `haystack_extensions-0.0.3/LICENSE` & `haystack_extensions-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `haystack_extensions-0.0.3/README.md` & `haystack_extensions-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -55,21 +55,24 @@
 
 
 if __name__ == "__main__":
     comp1 = SimplePrintStringWithWaitComponent(wait_time=10)
     comp2 = SimplePrintStringWithWaitComponent(wait_time=3)
     comp3 = SimplePrintStringWithWaitComponent(wait_time=5)
 
+    named_components = [NamedComponent("one", comp1), NamedComponent("two", comp2), NamedComponent("three", comp3)]
+    concurrent_component_runner = ConcurrentComponentRunner(named_components)
+
     p = Pipeline()
-    p.add_component("multithreaded_component", multithreaded_component)
+    p.add_component("concurrent_component_runner", concurrent_component_runner)
 
-    result = p.run(data={ "multithreaded_component": {
-                    "one": {"text": "Hello"}, 
-                    "two": {"text": "World"}, 
-                    "three": {"text": "!"}
+    result = p.run(data={ "concurrent_component_runner": {
+                    "one_text": "Hello",
+                    "two_text": "World",
+                    "three_text": "!"
                 }
             })
 
     print(result)
 ```
 
 This will lead to the following output and result: 
@@ -79,15 +82,15 @@
 World  <<== waited for 3 seconds
 !  <<== waited for 5 seconds
 Hello  <<== waited for 10 seconds
 ```
 
 **Result:**
 ```python
-result = {'multithreaded_component': {'one': {'text': 'Hello'}, 'two': {'text': 'World'}, 'three': {'text': '!'}}}
+result = {'multithreaded_component': {'one_text': 'Hello', 'two_text': 'World', 'three_text': '!'}}
 ```
 
 ### Subpipelines
 
 ```python
 import time
 from haystack import component, Pipeline
```

### Comparing `haystack_extensions-0.0.3/pyproject.toml` & `haystack_extensions-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `haystack_extensions-0.0.3/PKG-INFO` & `haystack_extensions-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: haystack_extensions
-Version: 0.0.3
+Version: 0.0.4
 Summary: An set of useful extensions for the Haystack AI library.
 Project-URL: Documentation, https://github.com/Redna/haystack-extensions#readme
 Project-URL: Issues, https://github.com/Redna/haystack-extensions/issues
 Project-URL: Source, https://github.com/Redna/haystack-extensions/tree/main/integrations/amazon_bedrock
 Author-email: Alexander Gruhl <gruhl.alexander@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -78,21 +78,24 @@
 
 
 if __name__ == "__main__":
     comp1 = SimplePrintStringWithWaitComponent(wait_time=10)
     comp2 = SimplePrintStringWithWaitComponent(wait_time=3)
     comp3 = SimplePrintStringWithWaitComponent(wait_time=5)
 
+    named_components = [NamedComponent("one", comp1), NamedComponent("two", comp2), NamedComponent("three", comp3)]
+    concurrent_component_runner = ConcurrentComponentRunner(named_components)
+
     p = Pipeline()
-    p.add_component("multithreaded_component", multithreaded_component)
+    p.add_component("concurrent_component_runner", concurrent_component_runner)
 
-    result = p.run(data={ "multithreaded_component": {
-                    "one": {"text": "Hello"}, 
-                    "two": {"text": "World"}, 
-                    "three": {"text": "!"}
+    result = p.run(data={ "concurrent_component_runner": {
+                    "one_text": "Hello",
+                    "two_text": "World",
+                    "three_text": "!"
                 }
             })
 
     print(result)
 ```
 
 This will lead to the following output and result: 
@@ -102,15 +105,15 @@
 World  <<== waited for 3 seconds
 !  <<== waited for 5 seconds
 Hello  <<== waited for 10 seconds
 ```
 
 **Result:**
 ```python
-result = {'multithreaded_component': {'one': {'text': 'Hello'}, 'two': {'text': 'World'}, 'three': {'text': '!'}}}
+result = {'multithreaded_component': {'one_text': 'Hello', 'two_text': 'World', 'three_text': '!'}}
 ```
 
 ### Subpipelines
 
 ```python
 import time
 from haystack import component, Pipeline
```

