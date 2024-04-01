# Comparing `tmp/cbrkit-0.7.0.tar.gz` & `tmp/cbrkit-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbrkit-0.7.0.tar", max compression
+gzip compressed data, was "cbrkit-0.8.0.tar", max compression
```

## Comparing `cbrkit-0.7.0.tar` & `cbrkit-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1067 2024-03-26 10:20:37.259163 cbrkit-0.7.0/LICENSE
--rw-r--r--   0        0        0    10939 2024-03-26 10:20:37.259163 cbrkit-0.7.0/README.md
--rw-r--r--   0        0        0      247 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/__init__.py
--rw-r--r--   0        0        0       34 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/__main__.py
--rw-r--r--   0        0        0     1680 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/api.py
--rw-r--r--   0        0        0      814 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/cli.py
--rw-r--r--   0        0        0     4383 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/helpers.py
--rw-r--r--   0        0        0     8736 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/loaders.py
--rw-r--r--   0        0        0        0 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/py.typed
--rw-r--r--   0        0        0     7551 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/retrieval.py
--rw-r--r--   0        0        0      814 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/sim/__init__.py
--rw-r--r--   0        0        0     2997 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/sim/_aggregator.py
--rw-r--r--   0        0        0     4805 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/sim/_attribute_value.py
--rw-r--r--   0        0        0      683 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/sim/collections.py
--rw-r--r--   0        0        0     1559 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/sim/generic.py
--rw-r--r--   0        0        0      386 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/sim/graph/__init__.py
--rw-r--r--   0        0        0     9987 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/sim/graph/_astar.py
--rw-r--r--   0        0        0      685 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/sim/graph/_model.py
--rw-r--r--   0        0        0     2511 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/sim/numbers.py
--rw-r--r--   0        0        0     9225 2024-03-26 10:20:37.259163 cbrkit-0.7.0/cbrkit/sim/strings/__init__.py
--rw-r--r--   0        0        0    10258 2024-03-26 10:20:37.263163 cbrkit-0.7.0/cbrkit/sim/strings/taxonomy.py
--rw-r--r--   0        0        0     1896 2024-03-26 10:20:37.263163 cbrkit-0.7.0/cbrkit/typing.py
--rw-r--r--   0        0        0     2773 2024-03-26 10:21:32.831289 cbrkit-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    13256 1970-01-01 00:00:00.000000 cbrkit-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-01 20:16:08.744656 cbrkit-0.8.0/LICENSE
+-rw-r--r--   0        0        0    10939 2024-04-01 20:16:08.744656 cbrkit-0.8.0/README.md
+-rw-r--r--   0        0        0      246 2024-04-01 20:16:08.744656 cbrkit-0.8.0/cbrkit/__init__.py
+-rw-r--r--   0        0        0       34 2024-04-01 20:16:08.744656 cbrkit-0.8.0/cbrkit/__main__.py
+-rw-r--r--   0        0        0     1680 2024-04-01 20:16:08.744656 cbrkit-0.8.0/cbrkit/api.py
+-rw-r--r--   0        0        0      813 2024-04-01 20:16:08.744656 cbrkit-0.8.0/cbrkit/cli.py
+-rw-r--r--   0        0        0     4383 2024-04-01 20:16:08.744656 cbrkit-0.8.0/cbrkit/helpers.py
+-rw-r--r--   0        0        0     8736 2024-04-01 20:16:08.744656 cbrkit-0.8.0/cbrkit/loaders.py
+-rw-r--r--   0        0        0        0 2024-04-01 20:16:08.744656 cbrkit-0.8.0/cbrkit/py.typed
+-rw-r--r--   0        0        0     7551 2024-04-01 20:16:08.744656 cbrkit-0.8.0/cbrkit/retrieval.py
+-rw-r--r--   0        0        0      814 2024-04-01 20:16:08.744656 cbrkit-0.8.0/cbrkit/sim/__init__.py
+-rw-r--r--   0        0        0     2997 2024-04-01 20:16:08.744656 cbrkit-0.8.0/cbrkit/sim/_aggregator.py
+-rw-r--r--   0        0        0     4805 2024-04-01 20:16:08.744656 cbrkit-0.8.0/cbrkit/sim/_attribute_value.py
+-rw-r--r--   0        0        0     2434 2024-04-01 20:16:08.744656 cbrkit-0.8.0/cbrkit/sim/collections.py
+-rw-r--r--   0        0        0     1559 2024-04-01 20:16:08.744656 cbrkit-0.8.0/cbrkit/sim/generic.py
+-rw-r--r--   0        0        0      386 2024-04-01 20:16:08.744656 cbrkit-0.8.0/cbrkit/sim/graph/__init__.py
+-rw-r--r--   0        0        0     9987 2024-04-01 20:16:08.744656 cbrkit-0.8.0/cbrkit/sim/graph/_astar.py
+-rw-r--r--   0        0        0      685 2024-04-01 20:16:08.748656 cbrkit-0.8.0/cbrkit/sim/graph/_model.py
+-rw-r--r--   0        0        0     2511 2024-04-01 20:16:08.748656 cbrkit-0.8.0/cbrkit/sim/numbers.py
+-rw-r--r--   0        0        0     9225 2024-04-01 20:16:08.748656 cbrkit-0.8.0/cbrkit/sim/strings/__init__.py
+-rw-r--r--   0        0        0    10258 2024-04-01 20:16:08.748656 cbrkit-0.8.0/cbrkit/sim/strings/taxonomy.py
+-rw-r--r--   0        0        0     1856 2024-04-01 20:16:08.748656 cbrkit-0.8.0/cbrkit/typing.py
+-rw-r--r--   0        0        0     2966 2024-04-01 20:17:13.284236 cbrkit-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    13438 1970-01-01 00:00:00.000000 cbrkit-0.8.0/PKG-INFO
```

### Comparing `cbrkit-0.7.0/LICENSE` & `cbrkit-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cbrkit-0.7.0/README.md` & `cbrkit-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `cbrkit-0.7.0/cbrkit/api.py` & `cbrkit-0.8.0/cbrkit/api.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.7.0/cbrkit/cli.py` & `cbrkit-0.8.0/cbrkit/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 .. include:: ../cli.md
 """
 
-
 from pathlib import Path
 
 try:
     from rich import print
     from typer import Typer
 except ModuleNotFoundError:
     print(
```

### Comparing `cbrkit-0.7.0/cbrkit/helpers.py` & `cbrkit-0.8.0/cbrkit/helpers.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.7.0/cbrkit/loaders.py` & `cbrkit-0.8.0/cbrkit/loaders.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.7.0/cbrkit/retrieval.py` & `cbrkit-0.8.0/cbrkit/retrieval.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.7.0/cbrkit/sim/__init__.py` & `cbrkit-0.8.0/cbrkit/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.7.0/cbrkit/sim/_aggregator.py` & `cbrkit-0.8.0/cbrkit/sim/_aggregator.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.7.0/cbrkit/sim/_attribute_value.py` & `cbrkit-0.8.0/cbrkit/sim/_attribute_value.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.7.0/cbrkit/sim/generic.py` & `cbrkit-0.8.0/cbrkit/sim/generic.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.7.0/cbrkit/sim/graph/_astar.py` & `cbrkit-0.8.0/cbrkit/sim/graph/_astar.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.7.0/cbrkit/sim/graph/_model.py` & `cbrkit-0.8.0/cbrkit/sim/graph/_model.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.7.0/cbrkit/sim/numbers.py` & `cbrkit-0.8.0/cbrkit/sim/numbers.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.7.0/cbrkit/sim/strings/__init__.py` & `cbrkit-0.8.0/cbrkit/sim/strings/__init__.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.7.0/cbrkit/sim/strings/taxonomy.py` & `cbrkit-0.8.0/cbrkit/sim/strings/taxonomy.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.7.0/cbrkit/typing.py` & `cbrkit-0.8.0/cbrkit/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,46 +28,41 @@
 SimSeqOrMap = SimMap[KeyType, SimType] | SimSeq[SimType]
 
 
 # Parameter names must match so that the signature can be inspected, do not add `/` here!
 class SimMapFunc(Protocol[KeyType, ValueType_contra, SimType_cov]):
     def __call__(
         self, x_map: Mapping[KeyType, ValueType_contra], y: ValueType_contra
-    ) -> SimMap[KeyType, SimType_cov]:
-        ...
+    ) -> SimMap[KeyType, SimType_cov]: ...
 
 
 class SimSeqFunc(Protocol[ValueType_contra, SimType_cov]):
     def __call__(
         self, pairs: Sequence[tuple[ValueType_contra, ValueType_contra]], /
-    ) -> SimSeq[SimType_cov]:
-        ...
+    ) -> SimSeq[SimType_cov]: ...
 
 
 class SimPairFunc(Protocol[ValueType_contra, SimType_cov]):
-    def __call__(self, x: ValueType_contra, y: ValueType_contra, /) -> SimType_cov:
-        ...
+    def __call__(self, x: ValueType_contra, y: ValueType_contra, /) -> SimType_cov: ...
 
 
 AnySimFunc = (
     SimMapFunc[KeyType, ValueType, SimType]
     | SimSeqFunc[ValueType, SimType]
     | SimPairFunc[ValueType, SimType]
 )
 
 
 class AggregatorFunc(Protocol[KeyType, SimType_contra]):
     def __call__(
         self,
         similarities: SimSeqOrMap[KeyType, SimType_contra],
         /,
-    ) -> float:
-        ...
+    ) -> float: ...
 
 
 class PoolingFunc(Protocol):
     def __call__(
         self,
         similarities: SimSeq[float],
         /,
-    ) -> float:
-        ...
+    ) -> float: ...
```

### Comparing `cbrkit-0.7.0/pyproject.toml` & `cbrkit-0.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cbrkit"
-version = "0.7.0"
+version = "0.8.0"
 description = "Customizable Case-Based Reasoning (CBR) toolkit for Python with a built-in API and CLI."
 authors = ["Mirko Lenz <mirko@mirkolenz.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "cbrkit" }]
 repository = "https://github.com/wi2trier/cbrkit"
 homepage = "https://wi2trier.github.io/cbrkit/"
@@ -50,41 +50,46 @@
 pyyaml = "^6.0"
 sentence-transformers = { version = "^2.2", optional = true }
 spacy = { version = "^3.7", optional = true }
 torch = { version = "^2.1.1", optional = true }
 transformers = { version = "^4.35", optional = true }
 typer = { version = ">=0.9, <1.0", extras = ["all"], optional = true }
 uvicorn = { version = ">=0.24, <1.0", optional = true, extras = ["standard"] }
+dtaidistance = { version = "^2.3.11", optional = true }
+minineedle ={ version = "^3.1.5", optional = true }
 xmltodict = ">=0.13, <1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^5.0.0"
+ruff = "^0.3.4"
 
 [tool.poetry.group.docs.dependencies]
 pdoc = "^14.4"
 
 [tool.poetry.extras]
 all = [
     "fastapi",
     "levenshtein",
     "nltk",
     "openai",
     "sentence-transformers",
     "spacy",
-    "spacy",
     "torch",
     "transformers",
     "typer",
     "uvicorn",
+    "minineedle",
+    "dtaidistance",
 ]
 cli = ["typer"]
 api = ["fastapi", "uvicorn"]
 nlp = ["levenshtein", "nltk", "openai", "spacy"]
 transformers = ["sentence-transformers", "torch", "transformers"]
+timeseries = ["minineedle", "dtaidistance"]
 
 [tool.pytest.ini_options]
 addopts = "--cov cbrkit --cov-report term-missing --doctest-modules --ignore cbrkit/cli.py --ignore cbrkit/api.py --ignore result"
 doctest_optionflags = "NORMALIZE_WHITESPACE IGNORE_EXCEPTION_DETAIL ELLIPSIS"
 
 [tool.ruff]
 target-version = "py311"
```

### Comparing `cbrkit-0.7.0/PKG-INFO` & `cbrkit-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbrkit
-Version: 0.7.0
+Version: 0.8.0
 Summary: Customizable Case-Based Reasoning (CBR) toolkit for Python with a built-in API and CLI.
 Home-page: https://wi2trier.github.io/cbrkit/
 License: MIT
 Keywords: cbr,case-based reasoning,api,similarity,nlp,retrieval,cli,tool,library
 Author: Mirko Lenz
 Author-email: mirko@mirkolenz.com
 Requires-Python: >=3.11,<3.13
@@ -24,25 +24,28 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Provides-Extra: all
 Provides-Extra: api
 Provides-Extra: cli
 Provides-Extra: nlp
+Provides-Extra: timeseries
 Provides-Extra: transformers
+Requires-Dist: dtaidistance (>=2.3.11,<3.0.0) ; extra == "all" or extra == "timeseries"
 Requires-Dist: fastapi[all] (>=0.100,<1.0) ; extra == "all" or extra == "api"
 Requires-Dist: levenshtein (>=0.23,<1.0) ; extra == "all" or extra == "nlp"
+Requires-Dist: minineedle (>=3.1.5,<4.0.0) ; extra == "all" or extra == "timeseries"
 Requires-Dist: nltk (>=3.8,<4.0) ; extra == "all" or extra == "nlp"
 Requires-Dist: openai (>=1.5,<2.0) ; extra == "all" or extra == "nlp"
 Requires-Dist: orjson (>=3.9,<4.0)
 Requires-Dist: pandas (>=2.1,<3.0)
 Requires-Dist: pyarrow (>=13.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: sentence-transformers (>=2.2,<3.0) ; extra == "all" or extra == "transformers"
-Requires-Dist: spacy (>=3.7,<4.0) ; extra == "all" or extra == "all" or extra == "nlp"
+Requires-Dist: spacy (>=3.7,<4.0) ; extra == "all" or extra == "nlp"
 Requires-Dist: torch (>=2.1.1,<3.0.0) ; extra == "all" or extra == "transformers"
 Requires-Dist: transformers (>=4.35,<5.0) ; extra == "all" or extra == "transformers"
 Requires-Dist: typer[all] (>=0.9,<1.0) ; extra == "all" or extra == "cli"
 Requires-Dist: uvicorn[standard] (>=0.24,<1.0) ; extra == "all" or extra == "api"
 Requires-Dist: xmltodict (>=0.13,<1.0)
 Project-URL: Repository, https://github.com/wi2trier/cbrkit
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cbrkit Version: 0.7.0 Summary: Customizable Case-
+Metadata-Version: 2.1 Name: cbrkit Version: 0.8.0 Summary: Customizable Case-
 Based Reasoning (CBR) toolkit for Python with a built-in API and CLI. Home-
 page: https://wi2trier.github.io/cbrkit/ License: MIT Keywords: cbr,case-based
 reasoning,api,similarity,nlp,retrieval,cli,tool,library Author: Mirko Lenz
 Author-email: mirko@mirkolenz.com Requires-Python: >=3.11,<3.13 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Framework :: Pytest Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
@@ -10,29 +10,31 @@
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
 Information Analysis Classifier: Topic :: Software Development :: Libraries ::
 Python Modules Classifier: Topic :: Utilities Classifier: Typing :: Typed
 Provides-Extra: all Provides-Extra: api Provides-Extra: cli Provides-Extra: nlp
-Provides-Extra: transformers Requires-Dist: fastapi[all] (>=0.100,<1.0) ; extra
-== "all" or extra == "api" Requires-Dist: levenshtein (>=0.23,<1.0) ; extra ==
-"all" or extra == "nlp" Requires-Dist: nltk (>=3.8,<4.0) ; extra == "all" or
-extra == "nlp" Requires-Dist: openai (>=1.5,<2.0) ; extra == "all" or extra ==
-"nlp" Requires-Dist: orjson (>=3.9,<4.0) Requires-Dist: pandas (>=2.1,<3.0)
-Requires-Dist: pyarrow (>=13.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-
-Dist: sentence-transformers (>=2.2,<3.0) ; extra == "all" or extra ==
-"transformers" Requires-Dist: spacy (>=3.7,<4.0) ; extra == "all" or extra ==
-"all" or extra == "nlp" Requires-Dist: torch (>=2.1.1,<3.0.0) ; extra == "all"
-or extra == "transformers" Requires-Dist: transformers (>=4.35,<5.0) ; extra ==
-"all" or extra == "transformers" Requires-Dist: typer[all] (>=0.9,<1.0) ; extra
-== "all" or extra == "cli" Requires-Dist: uvicorn[standard] (>=0.24,<1.0) ;
-extra == "all" or extra == "api" Requires-Dist: xmltodict (>=0.13,<1.0)
-Project-URL: Repository, https://github.com/wi2trier/cbrkit Description-
-Content-Type: text/markdown
+Provides-Extra: timeseries Provides-Extra: transformers Requires-Dist:
+dtaidistance (>=2.3.11,<3.0.0) ; extra == "all" or extra == "timeseries"
+Requires-Dist: fastapi[all] (>=0.100,<1.0) ; extra == "all" or extra == "api"
+Requires-Dist: levenshtein (>=0.23,<1.0) ; extra == "all" or extra == "nlp"
+Requires-Dist: minineedle (>=3.1.5,<4.0.0) ; extra == "all" or extra ==
+"timeseries" Requires-Dist: nltk (>=3.8,<4.0) ; extra == "all" or extra ==
+"nlp" Requires-Dist: openai (>=1.5,<2.0) ; extra == "all" or extra == "nlp"
+Requires-Dist: orjson (>=3.9,<4.0) Requires-Dist: pandas (>=2.1,<3.0) Requires-
+Dist: pyarrow (>=13.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist:
+sentence-transformers (>=2.2,<3.0) ; extra == "all" or extra == "transformers"
+Requires-Dist: spacy (>=3.7,<4.0) ; extra == "all" or extra == "nlp" Requires-
+Dist: torch (>=2.1.1,<3.0.0) ; extra == "all" or extra == "transformers"
+Requires-Dist: transformers (>=4.35,<5.0) ; extra == "all" or extra ==
+"transformers" Requires-Dist: typer[all] (>=0.9,<1.0) ; extra == "all" or extra
+== "cli" Requires-Dist: uvicorn[standard] (>=0.24,<1.0) ; extra == "all" or
+extra == "api" Requires-Dist: xmltodict (>=0.13,<1.0) Project-URL: Repository,
+https://github.com/wi2trier/cbrkit Description-Content-Type: text/markdown
 ********** CCBBRRkkiitt **********
                                  [cbrkit logo]
                              _P_y_P_I | _D_o_c_s | _E_x_a_m_p_l_e
 Customizable Case-Based Reasoning (CBR) toolkit for Python with a built-in API
                                    and CLI.
 --- # CBRkit CBRkit is a customizable and modular toolkit for Case-Based
 Reasoning (CBR) in Python. It provides a set of tools for loading cases and
```

