# Comparing `tmp/kolmogorov-abacus-0.0.5.tar.gz` & `tmp/kolmogorov-abacus-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolmogorov-abacus-0.0.5.tar", last modified: Wed Feb  7 19:42:05 2024, max compression
+gzip compressed data, was "kolmogorov-abacus-0.0.6.tar", last modified: Mon Apr  1 18:02:37 2024, max compression
```

## Comparing `kolmogorov-abacus-0.0.5.tar` & `kolmogorov-abacus-0.0.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:42:05.493104 kolmogorov-abacus-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-02-07 19:42:05.493104 kolmogorov-abacus-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:42:05.485104 kolmogorov-abacus-0.0.5/abacus/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:42:05.489104 kolmogorov-abacus-0.0.5/abacus/auto_ab/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/auto_ab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51032 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/auto_ab/abtest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/auto_ab/graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/auto_ab/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/auto_ab/variance_reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:42:05.489104 kolmogorov-abacus-0.0.5/abacus/mde_researcher/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/mde_researcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/mde_researcher/_abstract_mde_experiment_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/mde_researcher/_experiment_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)    15323 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/mde_researcher/mde_research_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/mde_researcher/multiple_split_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/mde_researcher/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:42:05.489104 kolmogorov-abacus-0.0.5/abacus/resplitter/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/resplitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/resplitter/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/resplitter/resplit_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:42:05.489104 kolmogorov-abacus-0.0.5/abacus/splitter/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/splitter/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/splitter/split_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-07 19:41:51.000000 kolmogorov-abacus-0.0.5/abacus/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:42:05.489104 kolmogorov-abacus-0.0.5/kolmogorov_abacus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-02-07 19:42:05.000000 kolmogorov-abacus-0.0.5/kolmogorov_abacus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-02-07 19:42:05.000000 kolmogorov-abacus-0.0.5/kolmogorov_abacus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 19:42:05.000000 kolmogorov-abacus-0.0.5/kolmogorov_abacus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-07 19:42:05.000000 kolmogorov-abacus-0.0.5/kolmogorov_abacus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-07 19:42:05.000000 kolmogorov-abacus-0.0.5/kolmogorov_abacus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-02-07 19:41:52.000000 kolmogorov-abacus-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-07 19:41:52.000000 kolmogorov-abacus-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 19:42:05.493104 kolmogorov-abacus-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:42:05.489104 kolmogorov-abacus-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-02-07 19:41:52.000000 kolmogorov-abacus-0.0.5/tests/test_experiment_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-02-07 19:41:52.000000 kolmogorov-abacus-0.0.5/tests/test_experiment_initialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:02:37.486542 kolmogorov-abacus-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-01 18:02:37.486542 kolmogorov-abacus-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:02:37.482542 kolmogorov-abacus-0.0.6/abacus/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:02:37.482542 kolmogorov-abacus-0.0.6/abacus/auto_ab/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/auto_ab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51208 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/auto_ab/abtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/auto_ab/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/auto_ab/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/auto_ab/variance_reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:02:37.486542 kolmogorov-abacus-0.0.6/abacus/mde_researcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/mde_researcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/mde_researcher/_abstract_mde_experiment_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/mde_researcher/_experiment_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15323 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/mde_researcher/mde_research_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/mde_researcher/multiple_split_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/mde_researcher/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:02:37.486542 kolmogorov-abacus-0.0.6/abacus/resplitter/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/resplitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/resplitter/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/resplitter/resplit_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:02:37.486542 kolmogorov-abacus-0.0.6/abacus/splitter/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/splitter/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/splitter/split_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-01 18:02:26.000000 kolmogorov-abacus-0.0.6/abacus/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:02:37.486542 kolmogorov-abacus-0.0.6/kolmogorov_abacus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-01 18:02:37.000000 kolmogorov-abacus-0.0.6/kolmogorov_abacus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-01 18:02:37.000000 kolmogorov-abacus-0.0.6/kolmogorov_abacus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:02:37.000000 kolmogorov-abacus-0.0.6/kolmogorov_abacus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-01 18:02:37.000000 kolmogorov-abacus-0.0.6/kolmogorov_abacus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 18:02:37.000000 kolmogorov-abacus-0.0.6/kolmogorov_abacus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-01 18:02:27.000000 kolmogorov-abacus-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-01 18:02:27.000000 kolmogorov-abacus-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 18:02:37.486542 kolmogorov-abacus-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:02:37.486542 kolmogorov-abacus-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-01 18:02:27.000000 kolmogorov-abacus-0.0.6/tests/test_experiment_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-01 18:02:27.000000 kolmogorov-abacus-0.0.6/tests/test_experiment_initialization.py
```

### Comparing `kolmogorov-abacus-0.0.5/LICENSE` & `kolmogorov-abacus-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kolmogorov-abacus-0.0.5/PKG-INFO` & `kolmogorov-abacus-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolmogorov-abacus
-Version: 0.0.5
+Version: 0.0.6
 Summary: A/B experiments planning and evaluation tool
 Author-email: Vadim Glukhov <educauchy@gmail.com>, Egor Shishkovets <egor.shishkovets@glowbyteconsulting.com>, Dmitry Zabavin <dmitriy.zabavin@glowbyteconsulting.com>
 License: MIT License
         
         Copyright (c) 2023 Kolmogorov AI Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `kolmogorov-abacus-0.0.5/README.md` & `kolmogorov-abacus-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `kolmogorov-abacus-0.0.5/abacus/__init__.py` & `kolmogorov-abacus-0.0.6/abacus/__init__.py`

 * *Files identical despite different names*

### Comparing `kolmogorov-abacus-0.0.5/abacus/auto_ab/abtest.py` & `kolmogorov-abacus-0.0.6/abacus/auto_ab/abtest.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,16 +165,20 @@
             }
         elif method == "resplit_df":
             cols = {"strata_col": self.params.data_params.strata_col}
 
         not_correct_fields = []
         df_cols = df.columns
         for field, value in cols.items():
-            if value == "" or value not in df_cols:
-                not_correct_fields.append(field)
+            if isinstance(value, list):
+                if not all(x in df_cols for x in value):
+                    not_correct_fields.append(field)
+            else:
+                if value == "" or value not in df_cols:
+                    not_correct_fields.append(field)
 
         if len(not_correct_fields) > 0:
             raise ValueError(
                 f"You did not provide or provide incorrectly following data attributes: {not_correct_fields}"
             )
 
     def __get_group(
```

### Comparing `kolmogorov-abacus-0.0.5/abacus/auto_ab/graphics.py` & `kolmogorov-abacus-0.0.6/abacus/auto_ab/graphics.py`

 * *Files identical despite different names*

### Comparing `kolmogorov-abacus-0.0.5/abacus/auto_ab/params.py` & `kolmogorov-abacus-0.0.6/abacus/auto_ab/params.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,44 @@
 from __future__ import annotations
-from typing import Dict, Any, Optional
+from typing import Dict, Any, Optional, List, Tuple
 
 from pydantic.dataclasses import dataclass
 from pydantic import validator, Field
 import numpy as np
 
+
+
+
 from abacus.types import (
     ColumnNameType,
     ColumnNamesType,
     ArrayNumType,
     ArrayStrType,
     MetricType,
     MetricTransformType,
 )
 
+class MismatchMetricError(Exception):
+    """
+    Checks if user assigns custom metric functin along with custom metric name
+    Args:
+    metric_name:str
+    Metric name assigned by user via metric_name attr
+    msg: str
+    Error message template (default: 'You use default metric function with custom metric name "{}"! Reassign it with "metric" parameter.')
+    """
+    def __init__(
+        self,
+        metric_name:str,
+        msg:str='You use default metric function with custom metric name "{}"! Reassign it with "metric" parameter.'
+        ):
+        self.metric_name = metric_name
+        self.msg = msg.format(self.metric_name)
+        super().__init__(self.msg)
+        
 
 class ValidationConfig:
     validate_assignment = True
     arbitrary_types_allowed = True
 
 
 @dataclass(config=ValidationConfig)
@@ -75,16 +96,17 @@
         metric_transform (Callable[[np.ndarray], np.ndarray], Optional): applied transformations to experiment.
         metric_transform_info (Dict[str, Dict[str, Any]], Optional): information of applied transformations.
         filter_method (str, Optional): method for filtering outliers: top_5, isolation_forest.
         n_boot_samples (int, Optional): number of bootstrap iterations.
         n_buckets (int, Optional): number of buckets.
         strata (str, Optional): stratification column.
         strata_weights (Dict[str, float], Optional): historical strata weights.
+        default_metrics: Optional[Tuple[str]] : default metric with autoselected metric functions
     """
-
+    
     alpha: Optional[float] = 0.05
     beta: Optional[float] = 0.2
     alternative: Optional[str] = "two-sided"  # less, greater, two-sided
     metric_type: Optional[str] = "continuous"  # continuous, binary, ratio
     metric_name: Optional[str] = "mean"  # mean, median
     metric: Optional[MetricType] = np.mean
     metric_transform: Optional[MetricTransformType] = np.mean
@@ -92,20 +114,25 @@
         default_factory=dict
     )
     filter_method: Optional[str] = "top_5"  # top_5, isolation_forest
     n_boot_samples: Optional[int] = 200
     n_buckets: Optional[int] = 100
     strata: Optional[str] = ""
     strata_weights: Optional[Dict[str, float]] = Field(default_factory=dict)
+    default_metrics: Optional[Tuple[str, ...]] = ('mean', 'median')
 
     def __post_init__(self):
+        if self.metric_name not in self.default_metrics \
+            and self.metric is np.mean:
+                raise MismatchMetricError(self.metric_name)
         if self.metric_name == "mean":
             self.metric = np.mean
         if self.metric_name == "median":
             self.metric = np.median
+            
 
     @validator("alpha", always=True, allow_reuse=True)
     @classmethod
     def alpha_validator(cls, alpha: float) -> float:
         assert 1 > alpha > 0, "alpha is not in range [0, 1]"
         return alpha
```

### Comparing `kolmogorov-abacus-0.0.5/abacus/auto_ab/variance_reduction.py` & `kolmogorov-abacus-0.0.6/abacus/auto_ab/variance_reduction.py`

 * *Files identical despite different names*

### Comparing `kolmogorov-abacus-0.0.5/abacus/mde_researcher/_abstract_mde_experiment_builder.py` & `kolmogorov-abacus-0.0.6/abacus/mde_researcher/_abstract_mde_experiment_builder.py`

 * *Files identical despite different names*

### Comparing `kolmogorov-abacus-0.0.5/abacus/mde_researcher/_experiment_structures.py` & `kolmogorov-abacus-0.0.6/abacus/mde_researcher/_experiment_structures.py`

 * *Files identical despite different names*

### Comparing `kolmogorov-abacus-0.0.5/abacus/mde_researcher/mde_research_builder.py` & `kolmogorov-abacus-0.0.6/abacus/mde_researcher/mde_research_builder.py`

 * *Files identical despite different names*

### Comparing `kolmogorov-abacus-0.0.5/abacus/mde_researcher/multiple_split_builder.py` & `kolmogorov-abacus-0.0.6/abacus/mde_researcher/multiple_split_builder.py`

 * *Files identical despite different names*

### Comparing `kolmogorov-abacus-0.0.5/abacus/mde_researcher/params.py` & `kolmogorov-abacus-0.0.6/abacus/mde_researcher/params.py`

 * *Files identical despite different names*

### Comparing `kolmogorov-abacus-0.0.5/abacus/resplitter/params.py` & `kolmogorov-abacus-0.0.6/abacus/resplitter/params.py`

 * *Files identical despite different names*

### Comparing `kolmogorov-abacus-0.0.5/abacus/resplitter/resplit_builder.py` & `kolmogorov-abacus-0.0.6/abacus/resplitter/resplit_builder.py`

 * *Files identical despite different names*

### Comparing `kolmogorov-abacus-0.0.5/abacus/splitter/params.py` & `kolmogorov-abacus-0.0.6/abacus/splitter/params.py`

 * *Files identical despite different names*

### Comparing `kolmogorov-abacus-0.0.5/abacus/splitter/split_builder.py` & `kolmogorov-abacus-0.0.6/abacus/splitter/split_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         if len(self.params.cols) > 0:
             additional_strata = (
                 (
                     clean_df.groupby("strata", as_index=False).apply(
                         lambda group: self._clusterize(
                             df=group,
                             strata="strata",
-                            columns=self.params.cols,
+                            columns=self.params.cols + self.params.cat_cols,
                             min_cluster_size=self.params.min_cluster_size,
                         )
                     )
                 )
                 .astype(str)
                 .droplevel(0)
             )
```

### Comparing `kolmogorov-abacus-0.0.5/abacus/types.py` & `kolmogorov-abacus-0.0.6/abacus/types.py`

 * *Files identical despite different names*

### Comparing `kolmogorov-abacus-0.0.5/kolmogorov_abacus.egg-info/PKG-INFO` & `kolmogorov-abacus-0.0.6/kolmogorov_abacus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolmogorov-abacus
-Version: 0.0.5
+Version: 0.0.6
 Summary: A/B experiments planning and evaluation tool
 Author-email: Vadim Glukhov <educauchy@gmail.com>, Egor Shishkovets <egor.shishkovets@glowbyteconsulting.com>, Dmitry Zabavin <dmitriy.zabavin@glowbyteconsulting.com>
 License: MIT License
         
         Copyright (c) 2023 Kolmogorov AI Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `kolmogorov-abacus-0.0.5/kolmogorov_abacus.egg-info/SOURCES.txt` & `kolmogorov-abacus-0.0.6/kolmogorov_abacus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kolmogorov-abacus-0.0.5/pyproject.toml` & `kolmogorov-abacus-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kolmogorov-abacus-0.0.5/tests/test_experiment_evaluation.py` & `kolmogorov-abacus-0.0.6/tests/test_experiment_evaluation.py`

 * *Files identical despite different names*

### Comparing `kolmogorov-abacus-0.0.5/tests/test_experiment_initialization.py` & `kolmogorov-abacus-0.0.6/tests/test_experiment_initialization.py`

 * *Files identical despite different names*

