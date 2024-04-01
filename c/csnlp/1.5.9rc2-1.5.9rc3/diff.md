# Comparing `tmp/csnlp-1.5.9rc2.tar.gz` & `tmp/csnlp-1.5.9rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csnlp-1.5.9rc2.tar", last modified: Mon Nov 20 16:37:52 2023, max compression
+gzip compressed data, was "csnlp-1.5.9rc3.tar", last modified: Wed Nov 29 13:03:06 2023, max compression
```

## Comparing `csnlp-1.5.9rc2.tar` & `csnlp-1.5.9rc3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-11-20 16:37:52.505167 csnlp-1.5.9rc2/
--rw-rw-rw-   0        0        0     1093 2022-11-02 20:11:46.000000 csnlp-1.5.9rc2/LICENSE
--rw-rw-rw-   0        0        0     7527 2023-11-20 16:37:52.499970 csnlp-1.5.9rc2/PKG-INFO
--rw-rw-rw-   0        0        0     6305 2023-10-27 18:09:23.000000 csnlp-1.5.9rc2/README.md
--rw-rw-rw-   0        0        0     2227 2023-10-27 18:06:59.000000 csnlp-1.5.9rc2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-11-20 16:37:52.506165 csnlp-1.5.9rc2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-11-20 16:37:52.289940 csnlp-1.5.9rc2/src/
-drwxrwxrwx   0        0        0        0 2023-11-20 16:37:52.325934 csnlp-1.5.9rc2/src/csnlp/
--rw-rw-rw-   0        0        0      204 2023-11-20 16:36:45.000000 csnlp-1.5.9rc2/src/csnlp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-20 16:37:52.373934 csnlp-1.5.9rc2/src/csnlp/core/
--rw-rw-rw-   0        0        0     4305 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/src/csnlp/core/cache.py
--rw-rw-rw-   0        0        0     3199 2023-10-26 05:53:02.000000 csnlp-1.5.9rc2/src/csnlp/core/data.py
--rw-rw-rw-   0        0        0     5982 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/src/csnlp/core/debug.py
--rw-rw-rw-   0        0        0     2068 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/src/csnlp/core/derivatives.py
--rw-rw-rw-   0        0        0     5228 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/src/csnlp/core/scaling.py
--rw-rw-rw-   0        0        0     6506 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/src/csnlp/core/solutions.py
-drwxrwxrwx   0        0        0        0 2023-11-20 16:37:52.384938 csnlp-1.5.9rc2/src/csnlp/multistart/
--rw-rw-rw-   0        0        0      393 2023-10-26 05:53:05.000000 csnlp-1.5.9rc2/src/csnlp/multistart/__init__.py
--rw-rw-rw-   0        0        0    15984 2023-10-27 18:09:23.000000 csnlp-1.5.9rc2/src/csnlp/multistart/multistart_nlp.py
--rw-rw-rw-   0        0        0     3671 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/src/csnlp/multistart/startpoints.py
-drwxrwxrwx   0        0        0        0 2023-11-20 16:37:52.405950 csnlp-1.5.9rc2/src/csnlp/nlps/
--rw-rw-rw-   0        0        0    18164 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/src/csnlp/nlps/constraints.py
--rw-rw-rw-   0        0        0     8964 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/src/csnlp/nlps/nlp.py
--rw-rw-rw-   0        0        0    11091 2023-10-27 18:09:23.000000 csnlp-1.5.9rc2/src/csnlp/nlps/objective.py
--rw-rw-rw-   0        0        0     1972 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/src/csnlp/nlps/parameters.py
--rw-rw-rw-   0        0        0     1972 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/src/csnlp/nlps/variables.py
-drwxrwxrwx   0        0        0        0 2023-11-20 16:37:52.423937 csnlp-1.5.9rc2/src/csnlp/util/
--rw-rw-rw-   0        0        0     5212 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/src/csnlp/util/docs.py
--rw-rw-rw-   0        0        0     9944 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/src/csnlp/util/io.py
--rw-rw-rw-   0        0        0     4449 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/src/csnlp/util/math.py
--rw-rw-rw-   0        0        0     4171 2023-10-27 15:56:10.000000 csnlp-1.5.9rc2/src/csnlp/util/plot.py
-drwxrwxrwx   0        0        0        0 2023-11-20 16:37:52.448932 csnlp-1.5.9rc2/src/csnlp/wrappers/
--rw-rw-rw-   0        0        0      350 2023-10-27 17:16:37.000000 csnlp-1.5.9rc2/src/csnlp/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-20 16:37:52.462932 csnlp-1.5.9rc2/src/csnlp/wrappers/mpc/
--rw-rw-rw-   0        0        0    16831 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/src/csnlp/wrappers/mpc/mpc.py
--rw-rw-rw-   0        0        0    16434 2023-11-20 16:34:32.000000 csnlp-1.5.9rc2/src/csnlp/wrappers/mpc/scenario_based_mpc.py
--rw-rw-rw-   0        0        0     7382 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/src/csnlp/wrappers/scaling.py
--rw-rw-rw-   0        0        0    16193 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/src/csnlp/wrappers/sensitivity.py
--rw-rw-rw-   0        0        0     3592 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/src/csnlp/wrappers/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-11-20 16:37:52.345933 csnlp-1.5.9rc2/src/csnlp.egg-info/
--rw-rw-rw-   0        0        0     7527 2023-11-20 16:37:52.000000 csnlp-1.5.9rc2/src/csnlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2023-11-20 16:37:52.000000 csnlp-1.5.9rc2/src/csnlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-20 16:37:52.000000 csnlp-1.5.9rc2/src/csnlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-11-20 16:37:52.000000 csnlp-1.5.9rc2/src/csnlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-11-20 16:37:52.000000 csnlp-1.5.9rc2/src/csnlp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-11-20 16:37:52.495932 csnlp-1.5.9rc2/tests/
--rw-rw-rw-   0        0        0    13922 2023-10-27 17:53:47.000000 csnlp-1.5.9rc2/tests/test_core.py
--rw-rw-rw-   0        0        0    10116 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/tests/test_examples.py
--rw-rw-rw-   0        0        0     7604 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/tests/test_multistart.py
--rw-rw-rw-   0        0        0    31820 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/tests/test_nlps.py
--rw-rw-rw-   0        0        0    27406 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/tests/test_quadrotor_mpc.py
--rw-rw-rw-   0        0        0     6273 2023-10-26 05:53:07.000000 csnlp-1.5.9rc2/tests/test_util.py
--rw-rw-rw-   0        0        0    20220 2023-10-26 05:51:18.000000 csnlp-1.5.9rc2/tests/test_wrappers.py
--rw-rw-rw-   0        0        0    16460 2023-10-26 05:51:24.000000 csnlp-1.5.9rc2/tests/test_wrappers_mpc.py
+drwxrwxrwx   0        0        0        0 2023-11-29 13:03:06.295076 csnlp-1.5.9rc3/
+-rw-rw-rw-   0        0        0     1093 2022-11-02 20:11:46.000000 csnlp-1.5.9rc3/LICENSE
+-rw-rw-rw-   0        0        0     7527 2023-11-29 13:03:06.290978 csnlp-1.5.9rc3/PKG-INFO
+-rw-rw-rw-   0        0        0     6305 2023-10-27 18:09:23.000000 csnlp-1.5.9rc3/README.md
+-rw-rw-rw-   0        0        0     2227 2023-10-27 18:06:59.000000 csnlp-1.5.9rc3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-11-29 13:03:06.295076 csnlp-1.5.9rc3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-11-29 13:03:06.157648 csnlp-1.5.9rc3/src/
+drwxrwxrwx   0        0        0        0 2023-11-29 13:03:06.173741 csnlp-1.5.9rc3/src/csnlp/
+-rw-rw-rw-   0        0        0      204 2023-11-29 13:02:50.000000 csnlp-1.5.9rc3/src/csnlp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-29 13:03:06.203612 csnlp-1.5.9rc3/src/csnlp/core/
+-rw-rw-rw-   0        0        0     4305 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/src/csnlp/core/cache.py
+-rw-rw-rw-   0        0        0     3199 2023-10-26 05:53:02.000000 csnlp-1.5.9rc3/src/csnlp/core/data.py
+-rw-rw-rw-   0        0        0     5982 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/src/csnlp/core/debug.py
+-rw-rw-rw-   0        0        0     2068 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/src/csnlp/core/derivatives.py
+-rw-rw-rw-   0        0        0     5228 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/src/csnlp/core/scaling.py
+-rw-rw-rw-   0        0        0     6506 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/src/csnlp/core/solutions.py
+drwxrwxrwx   0        0        0        0 2023-11-29 13:03:06.209603 csnlp-1.5.9rc3/src/csnlp/multistart/
+-rw-rw-rw-   0        0        0      393 2023-10-26 05:53:05.000000 csnlp-1.5.9rc3/src/csnlp/multistart/__init__.py
+-rw-rw-rw-   0        0        0    15984 2023-10-27 18:09:23.000000 csnlp-1.5.9rc3/src/csnlp/multistart/multistart_nlp.py
+-rw-rw-rw-   0        0        0     3908 2023-11-21 09:57:52.000000 csnlp-1.5.9rc3/src/csnlp/multistart/startpoints.py
+drwxrwxrwx   0        0        0        0 2023-11-29 13:03:06.228552 csnlp-1.5.9rc3/src/csnlp/nlps/
+-rw-rw-rw-   0        0        0    18164 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/src/csnlp/nlps/constraints.py
+-rw-rw-rw-   0        0        0     8964 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/src/csnlp/nlps/nlp.py
+-rw-rw-rw-   0        0        0    11091 2023-10-27 18:09:23.000000 csnlp-1.5.9rc3/src/csnlp/nlps/objective.py
+-rw-rw-rw-   0        0        0     1972 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/src/csnlp/nlps/parameters.py
+-rw-rw-rw-   0        0        0     1972 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/src/csnlp/nlps/variables.py
+drwxrwxrwx   0        0        0        0 2023-11-29 13:03:06.238984 csnlp-1.5.9rc3/src/csnlp/util/
+-rw-rw-rw-   0        0        0     5212 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/src/csnlp/util/docs.py
+-rw-rw-rw-   0        0        0     9944 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/src/csnlp/util/io.py
+-rw-rw-rw-   0        0        0     4449 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/src/csnlp/util/math.py
+-rw-rw-rw-   0        0        0     4171 2023-10-27 15:56:10.000000 csnlp-1.5.9rc3/src/csnlp/util/plot.py
+drwxrwxrwx   0        0        0        0 2023-11-29 13:03:06.250981 csnlp-1.5.9rc3/src/csnlp/wrappers/
+-rw-rw-rw-   0        0        0      350 2023-10-27 17:16:37.000000 csnlp-1.5.9rc3/src/csnlp/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-29 13:03:06.256981 csnlp-1.5.9rc3/src/csnlp/wrappers/mpc/
+-rw-rw-rw-   0        0        0    16831 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/src/csnlp/wrappers/mpc/mpc.py
+-rw-rw-rw-   0        0        0    16415 2023-11-21 09:20:03.000000 csnlp-1.5.9rc3/src/csnlp/wrappers/mpc/scenario_based_mpc.py
+-rw-rw-rw-   0        0        0     7382 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/src/csnlp/wrappers/scaling.py
+-rw-rw-rw-   0        0        0    16193 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/src/csnlp/wrappers/sensitivity.py
+-rw-rw-rw-   0        0        0     3592 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/src/csnlp/wrappers/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-11-29 13:03:06.286979 csnlp-1.5.9rc3/src/csnlp.egg-info/
+-rw-rw-rw-   0        0        0     7527 2023-11-29 13:03:06.000000 csnlp-1.5.9rc3/src/csnlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2023-11-29 13:03:06.000000 csnlp-1.5.9rc3/src/csnlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-29 13:03:06.000000 csnlp-1.5.9rc3/src/csnlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-11-29 13:03:06.000000 csnlp-1.5.9rc3/src/csnlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-11-29 13:03:06.000000 csnlp-1.5.9rc3/src/csnlp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-11-29 13:03:06.279048 csnlp-1.5.9rc3/tests/
+-rw-rw-rw-   0        0        0    13922 2023-10-27 17:53:47.000000 csnlp-1.5.9rc3/tests/test_core.py
+-rw-rw-rw-   0        0        0    10116 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/tests/test_examples.py
+-rw-rw-rw-   0        0        0     7604 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/tests/test_multistart.py
+-rw-rw-rw-   0        0        0    31820 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/tests/test_nlps.py
+-rw-rw-rw-   0        0        0    27406 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/tests/test_quadrotor_mpc.py
+-rw-rw-rw-   0        0        0     6273 2023-10-26 05:53:07.000000 csnlp-1.5.9rc3/tests/test_util.py
+-rw-rw-rw-   0        0        0    20220 2023-10-26 05:51:18.000000 csnlp-1.5.9rc3/tests/test_wrappers.py
+-rw-rw-rw-   0        0        0    16460 2023-10-26 05:51:24.000000 csnlp-1.5.9rc3/tests/test_wrappers_mpc.py
```

### Comparing `csnlp-1.5.9rc2/LICENSE` & `csnlp-1.5.9rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/PKG-INFO` & `csnlp-1.5.9rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csnlp
-Version: 1.5.9rc2
+Version: 1.5.9rc3
 Summary: Nonlinear Progamming with CasADi
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/casadi-nlp
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/casadi-nlp/issues
 Keywords: nonlinear-optimization,casadi,sensitivity-analysis
 Classifier: Programming Language :: Python
```

### Comparing `csnlp-1.5.9rc2/README.md` & `csnlp-1.5.9rc3/README.md`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/pyproject.toml` & `csnlp-1.5.9rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/core/cache.py` & `csnlp-1.5.9rc3/src/csnlp/core/cache.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/core/data.py` & `csnlp-1.5.9rc3/src/csnlp/core/data.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/core/debug.py` & `csnlp-1.5.9rc3/src/csnlp/core/debug.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/core/derivatives.py` & `csnlp-1.5.9rc3/src/csnlp/core/derivatives.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/core/scaling.py` & `csnlp-1.5.9rc3/src/csnlp/core/scaling.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/core/solutions.py` & `csnlp-1.5.9rc3/src/csnlp/core/solutions.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/multistart/multistart_nlp.py` & `csnlp-1.5.9rc3/src/csnlp/multistart/multistart_nlp.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/multistart/startpoints.py` & `csnlp-1.5.9rc3/src/csnlp/multistart/startpoints.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from collections.abc import Generator
-from typing import Any, NamedTuple, Optional
+from collections.abc import Generator, Sequence
+from typing import Any, NamedTuple, Union
 
 import numpy as np
 import numpy.typing as npt
 
 
 class RandomStartPoint:
     """Class containing all the information to guide the random generation of this
@@ -29,26 +29,33 @@
     """Class that can be iterated to yield a set of random start points for a multistart
     NLP optimization problem."""
 
     def __init__(
         self,
         points: dict[str, RandomStartPoint],
         multistarts: int,
-        seed: Optional[int] = None,
+        seed: Union[
+            None,
+            int,
+            Sequence[int],
+            np.random.SeedSequence,
+            np.random.BitGenerator,
+            np.random.Generator,
+        ] = None,
     ) -> None:
         """Instantiates the generator of random start points for multistarting.
 
         Parameters
         ----------
         points : dict of (str, RandomStartPoint)
             Dictionary containing the name of each variable, and how to generate random
             starting points for it (in the form of a `RandomStartPoint` object).
         multistarts : int
             The number of multiple start points.
-        seed : int, optional
+        seed : None, int, array_like[ints], SeedSequence, BitGenerator, Generator
             RNG seed.
         """
         self.points = points
         self.multistarts = multistarts
         self.np_random = np.random.default_rng(seed)
 
     def __iter__(self) -> Generator[dict[str, npt.ArrayLike], None, None]:
```

### Comparing `csnlp-1.5.9rc2/src/csnlp/nlps/constraints.py` & `csnlp-1.5.9rc3/src/csnlp/nlps/constraints.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/nlps/nlp.py` & `csnlp-1.5.9rc3/src/csnlp/nlps/nlp.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/nlps/objective.py` & `csnlp-1.5.9rc3/src/csnlp/nlps/objective.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/nlps/parameters.py` & `csnlp-1.5.9rc3/src/csnlp/nlps/parameters.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/nlps/variables.py` & `csnlp-1.5.9rc3/src/csnlp/nlps/variables.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/util/docs.py` & `csnlp-1.5.9rc3/src/csnlp/util/docs.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/util/io.py` & `csnlp-1.5.9rc3/src/csnlp/util/io.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/util/math.py` & `csnlp-1.5.9rc3/src/csnlp/util/math.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/util/plot.py` & `csnlp-1.5.9rc3/src/csnlp/util/plot.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/wrappers/mpc/mpc.py` & `csnlp-1.5.9rc3/src/csnlp/wrappers/mpc/mpc.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/wrappers/mpc/scenario_based_mpc.py` & `csnlp-1.5.9rc3/src/csnlp/wrappers/mpc/scenario_based_mpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,19 +310,19 @@
         scheme. However, instead of manually creating the objective for each scenario,
         this method allows to define only one expression for a single scenario, which is
         then automatically declined and summed for all scenarios. The symbolical
         expression must be made up of the single scenario states, disturbances, and
         slacks, returned as first output by the methods `state`, `disturbance`, and
         `constraint_from_single`, respectively.
         """
-        objective = cs.simplify(cs.cse(objective)) / self._n_scenarios
+        objective_ = objective / self._n_scenarios
         return self.nlp.minimize(
             sum(
                 _chained_subevalf(
-                    objective,
+                    objective_,
                     self.single_states,
                     self.states_i(i),
                     self.single_disturbances,
                     self.disturbances_i(i),
                     self.single_slacks,
                     self.slacks_i(i),
                     eval=False,
```

### Comparing `csnlp-1.5.9rc2/src/csnlp/wrappers/scaling.py` & `csnlp-1.5.9rc3/src/csnlp/wrappers/scaling.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/wrappers/sensitivity.py` & `csnlp-1.5.9rc3/src/csnlp/wrappers/sensitivity.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp/wrappers/wrapper.py` & `csnlp-1.5.9rc3/src/csnlp/wrappers/wrapper.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/src/csnlp.egg-info/PKG-INFO` & `csnlp-1.5.9rc3/src/csnlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csnlp
-Version: 1.5.9rc2
+Version: 1.5.9rc3
 Summary: Nonlinear Progamming with CasADi
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/casadi-nlp
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/casadi-nlp/issues
 Keywords: nonlinear-optimization,casadi,sensitivity-analysis
 Classifier: Programming Language :: Python
```

### Comparing `csnlp-1.5.9rc2/src/csnlp.egg-info/SOURCES.txt` & `csnlp-1.5.9rc3/src/csnlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/tests/test_core.py` & `csnlp-1.5.9rc3/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/tests/test_examples.py` & `csnlp-1.5.9rc3/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/tests/test_multistart.py` & `csnlp-1.5.9rc3/tests/test_multistart.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/tests/test_nlps.py` & `csnlp-1.5.9rc3/tests/test_nlps.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/tests/test_quadrotor_mpc.py` & `csnlp-1.5.9rc3/tests/test_quadrotor_mpc.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/tests/test_util.py` & `csnlp-1.5.9rc3/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/tests/test_wrappers.py` & `csnlp-1.5.9rc3/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.9rc2/tests/test_wrappers_mpc.py` & `csnlp-1.5.9rc3/tests/test_wrappers_mpc.py`

 * *Files identical despite different names*

