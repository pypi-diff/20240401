# Comparing `tmp/agogos-0.3.2.tar.gz` & `tmp/agogos-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agogos-0.3.2.tar", last modified: Mon Apr  1 00:00:01 2024, max compression
+gzip compressed data, was "agogos-0.3.3.tar", last modified: Mon Apr  1 19:51:06 2024, max compression
```

## Comparing `agogos-0.3.2.tar` & `agogos-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:01.557573 agogos-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-31 23:59:58.000000 agogos-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-01 00:00:01.557573 agogos-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-31 23:59:58.000000 agogos-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:01.553573 agogos-0.3.2/agogos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 23:59:58.000000 agogos-0.3.2/agogos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-03-31 23:59:58.000000 agogos-0.3.2/agogos/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14750 2024-03-31 23:59:58.000000 agogos-0.3.2/agogos/training.py
--rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-03-31 23:59:58.000000 agogos-0.3.2/agogos/transforming.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:01.557573 agogos-0.3.2/agogos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-01 00:00:01.000000 agogos-0.3.2/agogos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-01 00:00:01.000000 agogos-0.3.2/agogos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 00:00:01.000000 agogos-0.3.2/agogos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 00:00:01.000000 agogos-0.3.2/agogos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 00:00:01.000000 agogos-0.3.2/agogos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-31 23:59:58.000000 agogos-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 00:00:01.557573 agogos-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:01.557573 agogos-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-03-31 23:59:58.000000 agogos-0.3.2/tests/test__core.py
--rw-r--r--   0 runner    (1001) docker     (127)    17074 2024-03-31 23:59:58.000000 agogos-0.3.2/tests/test_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-03-31 23:59:58.000000 agogos-0.3.2/tests/test_transforming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:05.996141 agogos-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-01 19:51:02.000000 agogos-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-01 19:51:05.996141 agogos-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-01 19:51:02.000000 agogos-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:05.992141 agogos-0.3.3/agogos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:02.000000 agogos-0.3.3/agogos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7577 2024-04-01 19:51:02.000000 agogos-0.3.3/agogos/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-04-01 19:51:02.000000 agogos-0.3.3/agogos/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-01 19:51:02.000000 agogos-0.3.3/agogos/transforming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:05.996141 agogos-0.3.3/agogos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-01 19:51:05.000000 agogos-0.3.3/agogos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-01 19:51:05.000000 agogos-0.3.3/agogos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:51:05.000000 agogos-0.3.3/agogos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 19:51:05.000000 agogos-0.3.3/agogos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 19:51:05.000000 agogos-0.3.3/agogos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-01 19:51:02.000000 agogos-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 19:51:05.996141 agogos-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:05.992141 agogos-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-01 19:51:02.000000 agogos-0.3.3/tests/test__core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17074 2024-04-01 19:51:02.000000 agogos-0.3.3/tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-04-01 19:51:02.000000 agogos-0.3.3/tests/test_transforming.py
```

### Comparing `agogos-0.3.2/LICENSE` & `agogos-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agogos-0.3.2/PKG-INFO` & `agogos-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agogos
-Version: 0.3.2
+Version: 0.3.3
 Summary: Package that creates the underlying construction of a machine learning pipeline
 Author-email: Jasper van Selm <jmvanselm@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `agogos-0.3.2/README.md` & `agogos-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `agogos-0.3.2/agogos/_core.py` & `agogos-0.3.3/agogos/_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -157,14 +157,23 @@
 
         # Set parent and children
         for step in self.steps:
             step._set_parent(self)
 
         self._set_children(self.steps)
 
+    def get_steps(self) -> list[_Base]:
+        """Return list of steps of _ParallelSystem
+
+        :return: List of steps
+        """
+        if self.steps is None:
+            return []
+        return self.steps
+
     def _set_hash(self, prev_hash: str) -> None:
         """Set the hash of the system.
 
         :param prev_hash: The hash of the previous block.
         """
         self._hash = prev_hash
 
@@ -233,14 +242,23 @@
 
         # Set parent and children
         for step in self.steps:
             step._set_parent(self)
 
         self._set_children(self.steps)
 
+    def get_steps(self) -> list[_Base]:
+        """Return list of steps of _ParallelSystem
+
+        :return: List of steps
+        """
+        if self.steps is None:
+            return []
+        return self.steps
+
     def _set_hash(self, prev_hash: str) -> None:
         """Set the hash of the system.
 
         :param prev_hash: The hash of the previous block.
         """
         self._hash = prev_hash
```

### Comparing `agogos-0.3.2/agogos/training.py` & `agogos-0.3.3/agogos/training.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,39 @@
 from joblib import hash
 from typing import Any
 from dataclasses import dataclass
 from agogos._core import _Block, _SequentialSystem, _ParallelSystem, _Base
 from agogos.transforming import TransformingSystem
 
 
-class Trainer(_Block):
+class TrainType(_Base):
+    """Abstract train type describing a class that implements two functions train and predict"""
+
+    @abstractmethod
+    def train(self, x: Any, y: Any, **train_args: Any) -> tuple[Any, Any]:
+        """Train the block.
+
+        :param x: The input data.
+        :param y: The target variable."""
+        raise NotImplementedError(
+            f"{self.__class__.__name__} does not implement train method."
+        )
+
+    @abstractmethod
+    def predict(self, x: Any, **pred_args: Any) -> Any:
+        """Predict the target variable.
+
+        :param x: The input data.
+        :return: The predictions."""
+        raise NotImplementedError(
+            f"{self.__class__.__name__} does not implement predict method."
+        )
+
+
+class Trainer(TrainType, _Block):
     """The trainer block is for blocks that need to train on two inputs and predict on one.
 
     Methods:
     .. code-block:: python
         @abstractmethod
         def train(self, x: Any, y: Any, **train_args: Any) -> tuple[Any, Any]:
             # Train the block.
@@ -46,40 +70,20 @@
                 return x
 
         my_trainer = MyTrainer()
         predictions, labels = my_trainer.train(x, y)
         predictions = my_trainer.predict(x)
     """
 
-    @abstractmethod
-    def train(self, x: Any, y: Any, **train_args: Any) -> tuple[Any, Any]:
-        """Train the block.
-
-        :param x: The input data.
-        :param y: The target variable."""
-        raise NotImplementedError(
-            f"{self.__class__.__name__} does not implement train method."
-        )
 
-    @abstractmethod
-    def predict(self, x: Any, **pred_args: Any) -> Any:
-        """Predict the target variable.
-
-        :param x: The input data.
-        :return: The predictions."""
-        raise NotImplementedError(
-            f"{self.__class__.__name__} does not implement predict method."
-        )
-
-
-class TrainingSystem(_SequentialSystem):
+class TrainingSystem(TrainType, _SequentialSystem):
     """A system that trains on the input data and labels.
 
     Parameters:
-    - steps (list[Trainer | TrainingSystem | ParallelTrainingSystem]): The steps in the system.
+    - steps (list[TrainType]): The steps in the system.
 
     Methods:
     .. code-block:: python
         def train(self, x: Any, y: Any, **train_args: Any) -> tuple[Any, Any]: # Train the system.
 
         def predict(self, x: Any, **pred_args: Any) -> Any: # Predict the output of the system.
 
@@ -110,17 +114,17 @@
     def __post_init__(self) -> None:
         """Post init method for the TrainingSystem class."""
 
         # Assert all steps are a subclass of Trainer
         for step in self.steps:
             if not isinstance(
                 step,
-                (Trainer, TrainingSystem, ParallelTrainingSystem, Pipeline),
+                (TrainType),
             ):
-                raise TypeError(f"step: {step} is not an instance of a trainer")
+                raise TypeError(f"step: {step} is not an instance of TrainType")
 
         super().__post_init__()
 
     def train(self, x: Any, y: Any, **train_args: Any) -> tuple[Any, Any]:
         """Train the system.
 
         :param x: The input to the system.
@@ -128,20 +132,18 @@
         :return: The input and output of the system."""
 
         # Loop through each step and call the train method
         for step in self.steps:
             step_name = step.__class__.__name__
 
             step_args = train_args.get(step_name, {})
-            if isinstance(
-                step, (Trainer, TrainingSystem, ParallelTrainingSystem, Pipeline)
-            ):
+            if isinstance(step, (TrainType)):
                 x, y = step.train(x, y, **step_args)
             else:
-                raise TypeError(f"{step} is not a subclass of Trainer")
+                raise TypeError(f"{step} is not an instance of TrainType")
 
         return x, y
 
     def predict(self, x: Any, **pred_args: Any) -> Any:
         """Predict the output of the system.
 
         :param x: The input to the system.
@@ -150,25 +152,23 @@
 
         # Loop through each step and call the predict method
         for step in self.steps:
             step_name = step.__class__.__name__
 
             step_args = pred_args.get(step_name, {})
 
-            if isinstance(
-                step, (Trainer, TrainingSystem, ParallelTrainingSystem, Pipeline)
-            ):
+            if isinstance(step, (TrainType)):
                 x = step.predict(x, **step_args)
             else:
-                raise TypeError(f"{step} is not a subclass of Trainer")
+                raise TypeError(f"{step} is not an instance of TrainType")
 
         return x
 
 
-class ParallelTrainingSystem(_ParallelSystem):
+class ParallelTrainingSystem(TrainType, _ParallelSystem):
     """A system that trains the input data in parallel.
 
     Parameters:
     - steps (list[Trainer | TrainingSystem | ParallelTrainingSystem]): The steps in the system.
 
     Methods:
     .. code-block:: python
@@ -201,18 +201,16 @@
     """
 
     def __post_init__(self) -> None:
         """Post init method for the ParallelTrainingSystem class."""
 
         # Assert all steps correct instances
         for step in self.steps:
-            if not isinstance(
-                step, (Trainer, TrainingSystem, ParallelTrainingSystem, Pipeline)
-            ):
-                raise TypeError(f"{step} is not an instance of a trainer")
+            if not isinstance(step, (TrainType)):
+                raise TypeError(f"{step} is not an instance of TrainType")
 
         super().__post_init__()
 
     def train(self, x: Any, y: Any, **train_args: Any) -> tuple[Any, Any]:
         """Train the system.
 
         :param x: The input to the system.
@@ -224,26 +222,22 @@
         num_steps = len(self.steps)
         out_x, out_y = None, None
         for i, step in enumerate(self.steps):
             step_name = step.__class__.__name__
 
             step_args = train_args.get(step_name, {})
 
-            if isinstance(
-                step, (Trainer, TrainingSystem, ParallelTrainingSystem, Pipeline)
-            ):
+            if isinstance(step, (TrainType)):
                 step_x, step_y = step.train(x, y, **step_args)
                 out_x, out_y = (
                     self.concat(out_x, step_x, 1 / num_steps),
                     self.concat_labels(out_y, step_y, 1 / num_steps),
                 )
             else:
-                raise TypeError(
-                    f"{step} is not a subclass of Trainer, TrainingSystem, ParallelTrainingSystem or Pipeline"
-                )
+                raise TypeError(f"{step} is not an instance of TrainType")
 
         return out_x, out_y
 
     def predict(self, x: Any, **pred_args: Any) -> Any:
         """Predict the output of the system.
 
         :param x: The input to the system.
@@ -254,21 +248,19 @@
         num_steps = len(self.steps)
         out_x = None
         for i, step in enumerate(self.steps):
             step_name = step.__class__.__name__
 
             step_args = pred_args.get(step_name, {})
 
-            if isinstance(
-                step, (Trainer, TrainingSystem, ParallelTrainingSystem, Pipeline)
-            ):
+            if isinstance(step, (TrainType)):
                 step_x = step.predict(x, **step_args)
                 out_x = self.concat(out_x, step_x, 1 / num_steps)
             else:
-                raise TypeError(f"{step} is not an instance of a trainer")
+                raise TypeError(f"{step} is not an instance of TrainType")
 
         return out_x
 
     def concat_labels(
         self, original_data: Any, data_to_concat: Any, weight: float = 1.0
     ) -> Any:
         """Concatenate the transformed labels. Will use concat method if not overridden.
@@ -278,15 +270,15 @@
         :param weight: Weight of data to concat
         :return: The concatenated data.
         """
         return self.concat(original_data, data_to_concat, weight)
 
 
 @dataclass
-class Pipeline(_Base):
+class Pipeline(TrainType):
     """A pipeline of systems that can be trained and predicted.
 
     Parameters:
     - x_sys (TransformingSystem | None): The system to transform the input data.
     - y_sys (TransformingSystem | None): The system to transform the labelled data.
     - train_sys (TrainingSystem | None): The system to train the data.
     - pred_sys (TransformingSystem | None): The system to transform the predictions.
```

### Comparing `agogos-0.3.2/agogos/transforming.py` & `agogos-0.3.3/agogos/transforming.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,29 @@
 from abc import abstractmethod
 from typing import Any
 
-from agogos._core import _Block, _SequentialSystem, _ParallelSystem
+from agogos._core import _Block, _SequentialSystem, _ParallelSystem, _Base
 
 
-class Transformer(_Block):
+class TransformType(_Base):
+    """Abstract transform type describing a class that implements the transform function"""
+
+    @abstractmethod
+    def transform(self, data: Any, **transform_args: Any) -> Any:
+        """Transform the input data.
+
+        :param data: The input data.
+        :param transform_args: Keyword arguments.
+        :return: The transformed data."""
+        raise NotImplementedError(
+            f"{self.__class__.__name__} does not implement transform method."
+        )
+
+
+class Transformer(TransformType, _Block):
     """The transformer block transforms any data it could be x or y data.
 
     Methods:
     .. code-block:: python
         @abstractmethod
         def transform(self, data: Any, **transform_args: Any) -> Any:
             # Transform the input data.
@@ -34,27 +49,16 @@
                 # Transform the input data.
                 return data
 
         my_transformer = MyTransformer()
         transformed_data = my_transformer.transform(data)
     """
 
-    @abstractmethod
-    def transform(self, data: Any, **transform_args: Any) -> Any:
-        """Transform the input data.
-
-        :param data: The input data.
-        :param transform_args: Keyword arguments.
-        :return: The transformed data."""
-        raise NotImplementedError(
-            f"{self.__class__.__name__} does not implement transform method."
-        )
-
 
-class TransformingSystem(_SequentialSystem):
+class TransformingSystem(TransformType, _SequentialSystem):
     """A system that transforms the input data.
 
     Parameters:
     - steps (list[Transformer | TransformingSystem | ParallelTransformingSystem]): The steps in the system.
 
     Implements the following methods:
     .. code-block:: python
@@ -87,18 +91,16 @@
     """
 
     def __post_init__(self) -> None:
         """Post init method for the TransformingSystem class."""
 
         # Assert all steps are a subclass of Transformer
         for step in self.steps:
-            if not isinstance(
-                step, (Transformer, TransformingSystem, ParallelTransformingSystem)
-            ):
-                raise TypeError(f"{step} is not an instance of a transformer")
+            if not isinstance(step, (TransformType)):
+                raise TypeError(f"{step} is not an instance of TransformType")
 
         super().__post_init__()
 
     def transform(self, data: Any, **transform_args: Any) -> Any:
         """Transform the input data.
 
         :param data: The input data.
@@ -106,25 +108,23 @@
         """
 
         # Loop through each step and call the transform method
         for step in self.steps:
             step_name = step.__class__.__name__
 
             step_args = transform_args.get(step_name, {})
-            if isinstance(
-                step, (Transformer, TransformingSystem, ParallelTransformingSystem)
-            ):
+            if isinstance(step, (TransformType)):
                 data = step.transform(data, **step_args)
             else:
-                raise TypeError(f"{step} is not an instance of a transformer")
+                raise TypeError(f"{step} is not an instance of TransformType")
 
         return data
 
 
-class ParallelTransformingSystem(_ParallelSystem):
+class ParallelTransformingSystem(TransformType, _ParallelSystem):
     """A system that transforms the input data in parallel.
 
     Parameters:
     - steps (list[Transformer | TransformingSystem | ParallelTransformingSystem]): The steps in the system.
 
     Methods:
     .. code-block:: python
@@ -162,35 +162,32 @@
     """
 
     def __post_init__(self) -> None:
         """Post init method for the ParallelTransformingSystem class."""
 
         # Assert all steps are a subclass of Transformer or TransformingSystem
         for step in self.steps:
-            assert issubclass(step.__class__, Transformer) or issubclass(
-                step.__class__, TransformingSystem
-            ), f"{step} is not a subclass of Transformer or TransformingSystem"
+            if not isinstance(step, (TransformType)):
+                raise TypeError(f"{step} is not an instance of TransformType")
 
         super().__post_init__()
 
     def transform(self, data: Any, **transform_args: Any) -> Any:
         """Transform the input data.
 
         :param data: The input data.
         :return: The transformed data.
         """
         # Loop through each step and call the transform method
         for i, step in enumerate(self.steps):
             step_name = step.__class__.__name__
 
             step_args = transform_args.get(step_name, {})
-            if isinstance(
-                step, (Transformer, TransformingSystem, ParallelTransformingSystem)
-            ):
+            if isinstance(step, (TransformType)):
                 if i == 0:
                     data = step.transform(data, **step_args)
                 else:
                     data = self.concat(data, step.transform(data, **step_args))
             else:
-                raise TypeError(f"{step} is not a subclass of Transformer")
+                raise TypeError(f"{step} is not an instance of TransformType")
 
         return data
```

### Comparing `agogos-0.3.2/agogos.egg-info/PKG-INFO` & `agogos-0.3.3/agogos.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agogos
-Version: 0.3.2
+Version: 0.3.3
 Summary: Package that creates the underlying construction of a machine learning pipeline
 Author-email: Jasper van Selm <jmvanselm@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `agogos-0.3.2/tests/test__core.py` & `agogos-0.3.3/tests/test__core.py`

 * *Files identical despite different names*

### Comparing `agogos-0.3.2/tests/test_training.py` & `agogos-0.3.3/tests/test_training.py`

 * *Files identical despite different names*

### Comparing `agogos-0.3.2/tests/test_transforming.py` & `agogos-0.3.3/tests/test_transforming.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,22 @@
         # Create an instance of the system
         system = ParallelTransformingSystem()
 
         # Assert the system is an instance of ParallelTransformingSystem
         assert isinstance(system, ParallelTransformingSystem)
         assert system is not None
 
+    def test_parallel_transforming_system_wrong_step(self):
+        class SubTransformer:
+            def transform(self, x):
+                return x
+
+        with pytest.raises(TypeError):
+            ParallelTransformingSystem(steps=[SubTransformer()])
+
     def test_parallel_transforming_system_transformers(self):
         transformer1 = Transformer()
         transformer2 = TransformingSystem()
 
         system = ParallelTransformingSystem(steps=[transformer1, transformer2])
         assert system is not None
```

