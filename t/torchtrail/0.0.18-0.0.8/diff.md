# Comparing `tmp/torchtrail-0.0.18.tar.gz` & `tmp/torchtrail-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchtrail-0.0.18.tar", last modified: Mon Apr  1 17:44:10 2024, max compression
+gzip compressed data, was "torchtrail-0.0.8.tar", last modified: Wed Feb  7 19:13:07 2024, max compression
```

## Comparing `torchtrail-0.0.18.tar` & `torchtrail-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 arakhmati   (502) staff       (20)        0 2024-04-01 17:44:10.047656 torchtrail-0.0.18/
--rw-r--r--   0 arakhmati   (502) staff       (20)     1072 2024-01-31 21:17:24.000000 torchtrail-0.0.18/LICENSE
--rw-r--r--   0 arakhmati   (502) staff       (20)     4041 2024-04-01 17:44:10.047508 torchtrail-0.0.18/PKG-INFO
--rw-r--r--   0 arakhmati   (502) staff       (20)     3537 2024-03-30 23:17:45.000000 torchtrail-0.0.18/README.md
--rw-r--r--   0 arakhmati   (502) staff       (20)       38 2024-04-01 17:44:10.047701 torchtrail-0.0.18/setup.cfg
--rw-r--r--   0 arakhmati   (502) staff       (20)     2445 2024-04-01 17:43:07.000000 torchtrail-0.0.18/setup.py
-drwxr-xr-x   0 arakhmati   (502) staff       (20)        0 2024-04-01 17:44:10.045714 torchtrail-0.0.18/tests/
--rw-r--r--   0 arakhmati   (502) staff       (20)     1318 2024-03-30 23:17:45.000000 torchtrail-0.0.18/tests/test_bert.py
--rw-r--r--   0 arakhmati   (502) staff       (20)     4988 2024-04-01 07:34:00.000000 torchtrail-0.0.18/tests/test_falcon.py
--rw-r--r--   0 arakhmati   (502) staff       (20)     1694 2024-03-30 23:17:45.000000 torchtrail-0.0.18/tests/test_functions.py
--rw-r--r--   0 arakhmati   (502) staff       (20)      983 2024-04-01 07:34:00.000000 torchtrail-0.0.18/tests/test_modules.py
--rw-r--r--   0 arakhmati   (502) staff       (20)     1358 2024-02-13 06:14:10.000000 torchtrail-0.0.18/tests/test_resnet.py
--rw-r--r--   0 arakhmati   (502) staff       (20)     6216 2024-02-13 07:17:28.000000 torchtrail-0.0.18/tests/test_vit.py
-drwxr-xr-x   0 arakhmati   (502) staff       (20)        0 2024-04-01 17:44:10.046348 torchtrail-0.0.18/torchtrail/
--rw-r--r--   0 arakhmati   (502) staff       (20)     1155 2024-03-26 21:12:45.000000 torchtrail-0.0.18/torchtrail/__init__.py
--rw-r--r--   0 arakhmati   (502) staff       (20)    38245 2024-04-01 17:41:05.000000 torchtrail-0.0.18/torchtrail/tracer.py
-drwxr-xr-x   0 arakhmati   (502) staff       (20)        0 2024-04-01 17:44:10.047291 torchtrail-0.0.18/torchtrail.egg-info/
--rw-r--r--   0 arakhmati   (502) staff       (20)     4041 2024-04-01 17:44:10.000000 torchtrail-0.0.18/torchtrail.egg-info/PKG-INFO
--rw-r--r--   0 arakhmati   (502) staff       (20)      364 2024-04-01 17:44:10.000000 torchtrail-0.0.18/torchtrail.egg-info/SOURCES.txt
--rw-r--r--   0 arakhmati   (502) staff       (20)        1 2024-04-01 17:44:10.000000 torchtrail-0.0.18/torchtrail.egg-info/dependency_links.txt
--rw-r--r--   0 arakhmati   (502) staff       (20)      196 2024-04-01 17:44:10.000000 torchtrail-0.0.18/torchtrail.egg-info/requires.txt
--rw-r--r--   0 arakhmati   (502) staff       (20)       11 2024-04-01 17:44:10.000000 torchtrail-0.0.18/torchtrail.egg-info/top_level.txt
+drwxr-xr-x   0 arakhmati   (502) staff       (20)        0 2024-02-07 19:13:07.038494 torchtrail-0.0.8/
+-rw-r--r--   0 arakhmati   (502) staff       (20)     1072 2024-01-31 21:17:24.000000 torchtrail-0.0.8/LICENSE
+-rw-r--r--   0 arakhmati   (502) staff       (20)     2767 2024-02-07 19:13:07.038351 torchtrail-0.0.8/PKG-INFO
+-rw-r--r--   0 arakhmati   (502) staff       (20)     2486 2024-02-07 19:05:43.000000 torchtrail-0.0.8/README.md
+-rw-r--r--   0 arakhmati   (502) staff       (20)       38 2024-02-07 19:13:07.038544 torchtrail-0.0.8/setup.cfg
+-rw-r--r--   0 arakhmati   (502) staff       (20)     2056 2024-02-07 19:02:14.000000 torchtrail-0.0.8/setup.py
+drwxr-xr-x   0 arakhmati   (502) staff       (20)        0 2024-02-07 19:13:07.036111 torchtrail-0.0.8/tests/
+-rw-r--r--   0 arakhmati   (502) staff       (20)      867 2024-02-06 19:21:54.000000 torchtrail-0.0.8/tests/test_functions.py
+-rw-r--r--   0 arakhmati   (502) staff       (20)     2501 2024-02-07 19:12:35.000000 torchtrail-0.0.8/tests/test_modules.py
+-rw-r--r--   0 arakhmati   (502) staff       (20)     5165 2024-02-05 20:40:26.000000 torchtrail-0.0.8/tests/test_vit.py
+drwxr-xr-x   0 arakhmati   (502) staff       (20)        0 2024-02-07 19:13:07.037099 torchtrail-0.0.8/torchtrail/
+-rw-r--r--   0 arakhmati   (502) staff       (20)     1159 2024-02-05 20:40:26.000000 torchtrail-0.0.8/torchtrail/__init__.py
+-rw-r--r--   0 arakhmati   (502) staff       (20)    13806 2024-02-07 19:02:14.000000 torchtrail-0.0.8/torchtrail/multidigraph.py
+-rw-r--r--   0 arakhmati   (502) staff       (20)    26573 2024-02-07 19:02:14.000000 torchtrail-0.0.8/torchtrail/tracer.py
+drwxr-xr-x   0 arakhmati   (502) staff       (20)        0 2024-02-07 19:13:07.038127 torchtrail-0.0.8/torchtrail.egg-info/
+-rw-r--r--   0 arakhmati   (502) staff       (20)     2767 2024-02-07 19:13:07.000000 torchtrail-0.0.8/torchtrail.egg-info/PKG-INFO
+-rw-r--r--   0 arakhmati   (502) staff       (20)      330 2024-02-07 19:13:07.000000 torchtrail-0.0.8/torchtrail.egg-info/SOURCES.txt
+-rw-r--r--   0 arakhmati   (502) staff       (20)        1 2024-02-07 19:13:07.000000 torchtrail-0.0.8/torchtrail.egg-info/dependency_links.txt
+-rw-r--r--   0 arakhmati   (502) staff       (20)      168 2024-02-07 19:13:07.000000 torchtrail-0.0.8/torchtrail.egg-info/requires.txt
+-rw-r--r--   0 arakhmati   (502) staff       (20)       11 2024-02-07 19:13:07.000000 torchtrail-0.0.8/torchtrail.egg-info/top_level.txt
```

### Comparing `torchtrail-0.0.18/LICENSE` & `torchtrail-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `torchtrail-0.0.18/PKG-INFO` & `torchtrail-0.0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: torchtrail
-Version: 0.0.18
+Version: 0.0.8
 Summary: A library for tracing the execution of Pytorch operations and modules
-Home-page: https://github.com/arakhmati/torchtrail
 Author: Akhmed Rakhmati
 Author-email: akhmed.rakhmati@gmail.com
-Keywords: pytorch,tracing,tracing library,tracing tool,tracing module,tracing operations,visualize,visualize pytorch,visualize pytorch operations,visualize pytorch modules
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # torchtrail
 
 [![PyPI version](https://badge.fury.io/py/torchtrail.svg)](https://badge.fury.io/py/torchtrail)
@@ -36,25 +34,20 @@
 
 ### Tracing a function
 ```python
 import torch
 import torchtrail
 
 with torchtrail.trace():
-    input_tensor = torch.rand(1, 64)
-    output_tensor = torch.exp(input_tensor)
-torchtrail.visualize(output_tensor, file_name="exp.svg")
+    tensor = torch.rand(1, 64)
+    tensor = torch.exp(tensor)
+torchtrail.visualize(tensor, file_name="exp.svg")
 ```
 ![](https://raw.githubusercontent.com/arakhmati/torchtrail/main/docs/images/exp.svg)
 
-The graph could be obtained as a `networkx.MultiDiGraph` using `torchtrail.get_graph`:
-```python
-graph: "networkx.MultiDiGraph" = torchtrail.get_graph(output_tensor)
-```
-
 
 ### Tracing a module
 
 ```python
 import torch
 import transformers
 
@@ -70,44 +63,28 @@
     output = model(input_tensor).last_hidden_state
 
 torchtrail.visualize(output, max_depth=1, file_name="bert_max_depth_1.svg")
 ```
 
 ![](https://raw.githubusercontent.com/arakhmati/torchtrail/main/docs/images/bert_max_depth_1.svg)
 
-
 ```python
 torchtrail.visualize(output, max_depth=2, file_name="bert_max_depth_2.svg")
 ```
 
 ![](https://raw.githubusercontent.com/arakhmati/torchtrail/main/docs/images/bert_max_depth_2.svg)
 
 The graph of the full module can be visualized by omitting `max_depth` argument
 
 ```python
 torchtrail.visualize(output, file_name="bert.svg")
 ```
 
 ![](https://raw.githubusercontent.com/arakhmati/torchtrail/main/docs/images/bert.svg)
 
-The graph could be obtained as a `networkx.MultiDiGraph` using `torchtrail.get_graph`:
-```python
-graph: "networkx.MultiDiGraph" = torchtrail.get_graph(output_tensor)
-```
-
 Alternatively, visualization of the modules can be turned off completely using `show_modules=False`
 
 ```python
 torchtrail.visualize(output, show_modules=False, file_name="bert_show_modules_False.svg")
 ```
 
 ![](https://raw.githubusercontent.com/arakhmati/torchtrail/main/docs/images/bert_show_modules_False.svg)
-
-The flattened graph could be obtained as a `networkx.MultiDiGraph` using `torchtrail.get_graph`:
-```python
-graph: "networkx.MultiDiGraph" = torchtrail.get_graph(output_tensor, flatten=True)
-```
-
-
-## Reference
-- `torchtrail` was inspired by [torchview](https://github.com/mert-kurttutan/torchview). [mert-kurttutan](https://github.com/mert-kurttutan) did an amazing job with displaying torch graphs. However, one of the goals of `torchtrail` included producing [networkx](https://networkx.org)-compatible graph, therefore `torchtrail` was written.
-- The idea to use persistent MultiDiGraph to trace torch operations was taken from [composit](https://github.com/arakhmati/composit)
```

### Comparing `torchtrail-0.0.18/README.md` & `torchtrail-0.0.8/torchtrail.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: torchtrail
+Version: 0.0.8
+Summary: A library for tracing the execution of Pytorch operations and modules
+Author: Akhmed Rakhmati
+Author-email: akhmed.rakhmati@gmail.com
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # torchtrail
 
 [![PyPI version](https://badge.fury.io/py/torchtrail.svg)](https://badge.fury.io/py/torchtrail)
 [![Build Status](https://github.com/arakhmati/torchtrail/actions/workflows/python-package.yml/badge.svg)](https://github.com/arakhmati/torchtrail/actions/workflows/python-package.yml)
 [![GitHub license](https://img.shields.io/github/license/arakhmati/torchtrail)](https://github.com/arakhmati/torchtrail/blob/main/LICENSE)
 
 `torchtrail` provides an external API to trace pytorch models and extract the graph of torch functions and modules that were executed. The graphs can then be visualized or used for other purposes.
@@ -24,25 +34,20 @@
 
 ### Tracing a function
 ```python
 import torch
 import torchtrail
 
 with torchtrail.trace():
-    input_tensor = torch.rand(1, 64)
-    output_tensor = torch.exp(input_tensor)
-torchtrail.visualize(output_tensor, file_name="exp.svg")
+    tensor = torch.rand(1, 64)
+    tensor = torch.exp(tensor)
+torchtrail.visualize(tensor, file_name="exp.svg")
 ```
 ![](https://raw.githubusercontent.com/arakhmati/torchtrail/main/docs/images/exp.svg)
 
-The graph could be obtained as a `networkx.MultiDiGraph` using `torchtrail.get_graph`:
-```python
-graph: "networkx.MultiDiGraph" = torchtrail.get_graph(output_tensor)
-```
-
 
 ### Tracing a module
 
 ```python
 import torch
 import transformers
 
@@ -58,44 +63,28 @@
     output = model(input_tensor).last_hidden_state
 
 torchtrail.visualize(output, max_depth=1, file_name="bert_max_depth_1.svg")
 ```
 
 ![](https://raw.githubusercontent.com/arakhmati/torchtrail/main/docs/images/bert_max_depth_1.svg)
 
-
 ```python
 torchtrail.visualize(output, max_depth=2, file_name="bert_max_depth_2.svg")
 ```
 
 ![](https://raw.githubusercontent.com/arakhmati/torchtrail/main/docs/images/bert_max_depth_2.svg)
 
 The graph of the full module can be visualized by omitting `max_depth` argument
 
 ```python
 torchtrail.visualize(output, file_name="bert.svg")
 ```
 
 ![](https://raw.githubusercontent.com/arakhmati/torchtrail/main/docs/images/bert.svg)
 
-The graph could be obtained as a `networkx.MultiDiGraph` using `torchtrail.get_graph`:
-```python
-graph: "networkx.MultiDiGraph" = torchtrail.get_graph(output_tensor)
-```
-
 Alternatively, visualization of the modules can be turned off completely using `show_modules=False`
 
 ```python
 torchtrail.visualize(output, show_modules=False, file_name="bert_show_modules_False.svg")
 ```
 
 ![](https://raw.githubusercontent.com/arakhmati/torchtrail/main/docs/images/bert_show_modules_False.svg)
-
-The flattened graph could be obtained as a `networkx.MultiDiGraph` using `torchtrail.get_graph`:
-```python
-graph: "networkx.MultiDiGraph" = torchtrail.get_graph(output_tensor, flatten=True)
-```
-
-
-## Reference
-- `torchtrail` was inspired by [torchview](https://github.com/mert-kurttutan/torchview). [mert-kurttutan](https://github.com/mert-kurttutan) did an amazing job with displaying torch graphs. However, one of the goals of `torchtrail` included producing [networkx](https://networkx.org)-compatible graph, therefore `torchtrail` was written.
-- The idea to use persistent MultiDiGraph to trace torch operations was taken from [composit](https://github.com/arakhmati/composit)
```

### Comparing `torchtrail-0.0.18/setup.py` & `torchtrail-0.0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,45 +27,31 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="torchtrail",
-    version="0.0.18",
+    version="0.0.8",
     author="Akhmed Rakhmati",
     author_email="akhmed.rakhmati@gmail.com",
     description="A library for tracing the execution of Pytorch operations and modules",
     packages=find_packages(),
     install_requires=[
         "torch>=1.3.0",
-        "networkx>=3.1",
-        "pyrsistent>=0.20.0",
-        "graphviz>=0.20.1",
-        "loguru>=0.6.0",
+        "networkx==3.1",
+        "pyrsistent==0.20.0",
+        "graphviz==0.20.1",
+        "loguru==0.6.0",
     ],
     extras_require={
         "dev": [
-            "accelerate==0.27.0",
-            "black[jupyter]==24.1.1",
-            "pillow==10.2.0",
+            "black==24.1.1",
             "pytest==8.0.0",
-            "torchvision==0.17.0",
             "transformers==4.37.2",
+            "pillow==10.2.0",
+            "torchvision==0.17.0",
         ]
     },
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/arakhmati/torchtrail",
-    keywords=[
-        "pytorch",
-        "tracing",
-        "tracing library",
-        "tracing tool",
-        "tracing module",
-        "tracing operations",
-        "visualize",
-        "visualize pytorch",
-        "visualize pytorch operations",
-        "visualize pytorch modules",
-    ],
 )
```

### Comparing `torchtrail-0.0.18/tests/test_vit.py` & `torchtrail-0.0.8/tests/test_vit.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,16 +20,14 @@
     with torchtrail.trace():
         input_tensor = torch.randn(batch_size, num_channels, height, width)
         output = model(input_tensor)
 
     torchtrail.visualize(
         output, show_modules=show_modules, file_name=tmp_path / "vit_embeddings.svg"
     )
-    assert len(torchtrail.get_graph(output)) == 2
-    assert len(torchtrail.get_graph(output, flatten=True)) == 11
 
 
 @pytest.mark.parametrize("show_modules", [True, False])
 def test_vit_self_attention(tmp_path, show_modules):
     model_name = "google/vit-base-patch16-224"
     batch_size = 1
     sequence_size = 197
@@ -41,16 +39,14 @@
     with torchtrail.trace():
         input_tensor = torch.randn(batch_size, sequence_size, hidden_size)
         output = model(input_tensor)
 
     torchtrail.visualize(
         output, show_modules=show_modules, file_name=tmp_path / "vit_self_attention.svg"
     )
-    assert len(torchtrail.get_graph(output)) == 2
-    assert len(torchtrail.get_graph(output, flatten=True)) == 25
 
 
 @pytest.mark.parametrize("show_modules", [True, False])
 def test_vit_self_output(tmp_path, show_modules):
     model_name = "google/vit-base-patch16-224"
     batch_size = 1
     sequence_size = 197
@@ -63,16 +59,14 @@
         input_tensor = torch.randn(batch_size, sequence_size, hidden_size)
         residual_input_tensor = torch.randn(batch_size, sequence_size, hidden_size)
         output = model(input_tensor, residual_input_tensor)
 
     torchtrail.visualize(
         output, show_modules=show_modules, file_name=tmp_path / "vit_self_output.svg"
     )
-    assert len(torchtrail.get_graph(output)) == 3
-    assert len(torchtrail.get_graph(output, flatten=True)) in {6, 7}
 
 
 @pytest.mark.parametrize("show_modules", [True, False])
 def test_vit_attention(tmp_path, show_modules):
     model_name = "google/vit-base-patch16-224"
     batch_size = 1
     sequence_size = 197
@@ -84,16 +78,14 @@
     with torchtrail.trace():
         input_tensor = torch.randn(batch_size, sequence_size, hidden_size)
         output = model(input_tensor)
 
     torchtrail.visualize(
         output, show_modules=show_modules, file_name=tmp_path / "vit_attention.svg"
     )
-    assert len(torchtrail.get_graph(output)) == 2
-    assert len(torchtrail.get_graph(output, flatten=True)) in {29, 30}
 
 
 @pytest.mark.parametrize("show_modules", [True, False])
 def test_vit_intermediate(tmp_path, show_modules):
     model_name = "google/vit-base-patch16-224"
     batch_size = 1
     sequence_size = 197
@@ -105,16 +97,14 @@
     with torchtrail.trace():
         input_tensor = torch.randn(batch_size, sequence_size, hidden_size)
         output = model(input_tensor)
 
     torchtrail.visualize(
         output, show_modules=show_modules, file_name=tmp_path / "vit_intermediate.svg"
     )
-    assert len(torchtrail.get_graph(output)) == 2
-    assert len(torchtrail.get_graph(output, flatten=True)) == 5
 
 
 @pytest.mark.parametrize("show_modules", [True, False])
 def test_vit_layer(tmp_path, show_modules):
     model_name = "google/vit-base-patch16-224"
     batch_size = 1
     sequence_size = 197
@@ -126,16 +116,14 @@
     with torchtrail.trace():
         input_tensor = torch.randn(batch_size, sequence_size, hidden_size)
         output = model(input_tensor)
 
     torchtrail.visualize(
         output, show_modules=show_modules, file_name=tmp_path / "vit_layer.svg"
     )
-    assert len(torchtrail.get_graph(output)) == 2
-    assert len(torchtrail.get_graph(output, flatten=True)) in {45, 46}
 
 
 @pytest.mark.parametrize("show_modules", [True, False])
 def test_vit_encoder(tmp_path, show_modules):
     model_name = "google/vit-base-patch16-224"
     batch_size = 1
     sequence_size = 197
@@ -147,19 +135,14 @@
     with torchtrail.trace():
         input_tensor = torch.randn(batch_size, sequence_size, hidden_size)
         output = model(input_tensor).last_hidden_state
 
     torchtrail.visualize(
         output, show_modules=show_modules, file_name=tmp_path / "vit_encoder.svg"
     )
-    assert len(torchtrail.get_graph(output)) == 2
-    assert len(torchtrail.get_graph(output, flatten=True)) in {
-        541 - config.num_hidden_layers,
-        541,
-    }
 
 
 @pytest.mark.parametrize("show_modules", [True, False])
 def test_vit(tmp_path, show_modules):
     model_name = "google/vit-base-patch16-224"
     batch_size = 1
     num_channels = 3
@@ -172,12 +155,7 @@
     with torchtrail.trace():
         input_tensor = torch.randn(batch_size, num_channels, height, width)
         output = model(input_tensor).pooler_output
 
     torchtrail.visualize(
         output, show_modules=show_modules, file_name=tmp_path / "vit.svg"
     )
-    assert len(torchtrail.get_graph(output)) == 2
-    assert len(torchtrail.get_graph(output, flatten=True)) in {
-        559 - config.num_hidden_layers,
-        559,
-    }
```

### Comparing `torchtrail-0.0.18/torchtrail/__init__.py` & `torchtrail-0.0.8/torchtrail/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from .tracer import trace, visualize, get_graph
+from .tracer import trace, visualize, flatten_graph
```

