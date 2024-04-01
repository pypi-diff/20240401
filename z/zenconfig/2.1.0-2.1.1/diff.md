# Comparing `tmp/zenconfig-2.1.0.tar.gz` & `tmp/zenconfig-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenconfig-2.1.0.tar", max compression
+gzip compressed data, was "zenconfig-2.1.1.tar", max compression
```

## Comparing `zenconfig-2.1.0.tar` & `zenconfig-2.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1064 2023-09-09 09:18:04.764479 zenconfig-2.1.0/LICENSE
--rw-r--r--   0        0        0     3578 2023-09-09 09:18:04.764479 zenconfig-2.1.0/README.md
--rw-r--r--   0        0        0     1115 2023-09-09 09:18:04.764479 zenconfig-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      263 2023-09-09 09:18:04.764479 zenconfig-2.1.0/zenconfig/__init__.py
--rw-r--r--   0        0        0     4775 2023-09-09 09:18:04.764479 zenconfig-2.1.0/zenconfig/base.py
--rw-r--r--   0        0        0     1917 2023-09-09 09:18:04.764479 zenconfig-2.1.0/zenconfig/encoder.py
--rw-r--r--   0        0        0      244 2023-09-09 09:18:04.764479 zenconfig-2.1.0/zenconfig/formats/__init__.py
--rw-r--r--   0        0        0      731 2023-09-09 09:18:04.764479 zenconfig-2.1.0/zenconfig/formats/json.py
--rw-r--r--   0        0        0      537 2023-09-09 09:18:04.764479 zenconfig-2.1.0/zenconfig/formats/toml.py
--rw-r--r--   0        0        0      669 2023-09-09 09:18:04.764479 zenconfig-2.1.0/zenconfig/formats/yaml.py
--rw-r--r--   0        0        0        0 2023-09-09 09:18:04.764479 zenconfig-2.1.0/zenconfig/py.typed
--rw-r--r--   0        0        0     1902 2023-09-09 09:18:04.764479 zenconfig-2.1.0/zenconfig/read.py
--rw-r--r--   0        0        0      310 2023-09-09 09:18:04.764479 zenconfig-2.1.0/zenconfig/schemas/__init__.py
--rw-r--r--   0        0        0     1018 2023-09-09 09:18:04.764479 zenconfig-2.1.0/zenconfig/schemas/attrs.py
--rw-r--r--   0        0        0     1209 2023-09-09 09:18:04.764479 zenconfig-2.1.0/zenconfig/schemas/dataclass.py
--rw-r--r--   0        0        0      562 2023-09-09 09:18:04.764479 zenconfig-2.1.0/zenconfig/schemas/dict.py
--rw-r--r--   0        0        0     1588 2023-09-09 09:18:04.764479 zenconfig-2.1.0/zenconfig/schemas/pydantic.py
--rw-r--r--   0        0        0     1915 2023-09-09 09:18:04.764479 zenconfig-2.1.0/zenconfig/write.py
--rw-r--r--   0        0        0     4519 1970-01-01 00:00:00.000000 zenconfig-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-01 15:44:06.571236 zenconfig-2.1.1/LICENSE
+-rw-r--r--   0        0        0     3593 2024-04-01 15:44:06.571236 zenconfig-2.1.1/README.md
+-rw-r--r--   0        0        0     1133 2024-04-01 15:44:06.571236 zenconfig-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      263 2024-04-01 15:44:06.571236 zenconfig-2.1.1/zenconfig/__init__.py
+-rw-r--r--   0        0        0     4775 2024-04-01 15:44:06.571236 zenconfig-2.1.1/zenconfig/base.py
+-rw-r--r--   0        0        0     1917 2024-04-01 15:44:06.571236 zenconfig-2.1.1/zenconfig/encoder.py
+-rw-r--r--   0        0        0      244 2024-04-01 15:44:06.571236 zenconfig-2.1.1/zenconfig/formats/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-01 15:44:06.571236 zenconfig-2.1.1/zenconfig/formats/json.py
+-rw-r--r--   0        0        0      537 2024-04-01 15:44:06.571236 zenconfig-2.1.1/zenconfig/formats/toml.py
+-rw-r--r--   0        0        0      669 2024-04-01 15:44:06.571236 zenconfig-2.1.1/zenconfig/formats/yaml.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:44:06.571236 zenconfig-2.1.1/zenconfig/py.typed
+-rw-r--r--   0        0        0     1902 2024-04-01 15:44:06.571236 zenconfig-2.1.1/zenconfig/read.py
+-rw-r--r--   0        0        0      310 2024-04-01 15:44:06.571236 zenconfig-2.1.1/zenconfig/schemas/__init__.py
+-rw-r--r--   0        0        0     1018 2024-04-01 15:44:06.571236 zenconfig-2.1.1/zenconfig/schemas/attrs.py
+-rw-r--r--   0        0        0     1209 2024-04-01 15:44:06.571236 zenconfig-2.1.1/zenconfig/schemas/dataclass.py
+-rw-r--r--   0        0        0      562 2024-04-01 15:44:06.571236 zenconfig-2.1.1/zenconfig/schemas/dict.py
+-rw-r--r--   0        0        0     1588 2024-04-01 15:44:06.571236 zenconfig-2.1.1/zenconfig/schemas/pydantic.py
+-rw-r--r--   0        0        0     1915 2024-04-01 15:44:06.571236 zenconfig-2.1.1/zenconfig/write.py
+-rw-r--r--   0        0        0     4627 1970-01-01 00:00:00.000000 zenconfig-2.1.1/PKG-INFO
```

### Comparing `zenconfig-2.1.0/LICENSE` & `zenconfig-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zenconfig-2.1.0/README.md` & `zenconfig-2.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # zen-config
 
-[![tests](https://github.com/gpajot/zen-config/workflows/Test/badge.svg?branch=main&event=push)](https://github.com/gpajot/zen-config/actions?query=workflow%3ATest+branch%3Amain+event%3Apush)
+[![tests](https://github.com/gpajot/zen-config/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/gpajot/zen-config/actions/workflows/test.yml?query=branch%3Amain+event%3Apush)
 [![version](https://img.shields.io/pypi/v/zenconfig?label=stable)](https://pypi.org/project/zenconfig/)
 [![python](https://img.shields.io/pypi/pyversions/zenconfig)](https://pypi.org/project/zenconfig/)
 
 Simple configuration loader for python.
 
 Compared to other solutions, the goal is to bring:
 - simple usage for simple use cases
```

### Comparing `zenconfig-2.1.0/pyproject.toml` & `zenconfig-2.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "zenconfig"
-version = "2.1.0"
+version = "2.1.1"
 description = "Simple configuration loader for python."
 authors = ["Gabriel Pajot <gab@les-cactus.co>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gpajot/zen-config"
 include = ["zenconfig/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
+typing-extensions = ">=4.10"
 
 PyYAML = { version = ">=6,<7", optional = true }
 
 tomlkit = { version = ">=0,<1", optional = true }
 
 pydantic = { version = ">=1,<3", optional = true }
 
@@ -22,30 +23,29 @@
 [tool.poetry.extras]
 yaml = ["PyYAML"]
 toml = ["tomlkit"]
 pydantic = ["pydantic"]
 attrs = ["attrs"]
 
 [tool.poetry.group.test.dependencies]
-pytest = "==7.4.0"
-pytest-mock = "==3.11.1"
-ruff = "==0.0.275"
-mypy = "==1.4.1"
-black = "==23.3.0"
-pre-commit = "==3.3.3"
+pytest = "==8.1.1"
+pytest-mock = "==3.14.0"
+ruff = "==0.3.4"
+mypy = "==1.9.0"
+pre-commit = "==3.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 ignore_missing_imports = true
 install_types = true
 non_interactive = true
 check_untyped_defs = true
 
-[tool.ruff]
+[tool.ruff.lint]
 select = ["A", "B", "E", "F", "I", "PT"]
 ignore = ["E501"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
```

### Comparing `zenconfig-2.1.0/zenconfig/base.py` & `zenconfig-2.1.1/zenconfig/base.py`

 * *Files identical despite different names*

### Comparing `zenconfig-2.1.0/zenconfig/encoder.py` & `zenconfig-2.1.1/zenconfig/encoder.py`

 * *Files identical despite different names*

### Comparing `zenconfig-2.1.0/zenconfig/formats/json.py` & `zenconfig-2.1.1/zenconfig/formats/json.py`

 * *Files identical despite different names*

### Comparing `zenconfig-2.1.0/zenconfig/formats/toml.py` & `zenconfig-2.1.1/zenconfig/formats/toml.py`

 * *Files identical despite different names*

### Comparing `zenconfig-2.1.0/zenconfig/formats/yaml.py` & `zenconfig-2.1.1/zenconfig/formats/yaml.py`

 * *Files identical despite different names*

### Comparing `zenconfig-2.1.0/zenconfig/read.py` & `zenconfig-2.1.1/zenconfig/read.py`

 * *Files identical despite different names*

### Comparing `zenconfig-2.1.0/zenconfig/schemas/attrs.py` & `zenconfig-2.1.1/zenconfig/schemas/attrs.py`

 * *Files identical despite different names*

### Comparing `zenconfig-2.1.0/zenconfig/schemas/dataclass.py` & `zenconfig-2.1.1/zenconfig/schemas/dataclass.py`

 * *Files identical despite different names*

### Comparing `zenconfig-2.1.0/zenconfig/schemas/dict.py` & `zenconfig-2.1.1/zenconfig/schemas/dict.py`

 * *Files identical despite different names*

### Comparing `zenconfig-2.1.0/zenconfig/schemas/pydantic.py` & `zenconfig-2.1.1/zenconfig/schemas/pydantic.py`

 * *Files identical despite different names*

### Comparing `zenconfig-2.1.0/zenconfig/write.py` & `zenconfig-2.1.1/zenconfig/write.py`

 * *Files identical despite different names*

### Comparing `zenconfig-2.1.0/PKG-INFO` & `zenconfig-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: zenconfig
-Version: 2.1.0
+Version: 2.1.1
 Summary: Simple configuration loader for python.
 Home-page: https://github.com/gpajot/zen-config
 License: MIT
 Author: Gabriel Pajot
 Author-email: gab@les-cactus.co
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: attrs
 Provides-Extra: pydantic
 Provides-Extra: toml
 Provides-Extra: yaml
 Requires-Dist: PyYAML (>=6,<7) ; extra == "yaml"
 Requires-Dist: attrs (>=22.2,<24) ; extra == "attrs"
 Requires-Dist: pydantic (>=1,<3) ; extra == "pydantic"
 Requires-Dist: tomlkit (>=0,<1) ; extra == "toml"
+Requires-Dist: typing-extensions (>=4.10)
 Project-URL: Repository, https://github.com/gpajot/zen-config
 Description-Content-Type: text/markdown
 
 # zen-config
 
-[![tests](https://github.com/gpajot/zen-config/workflows/Test/badge.svg?branch=main&event=push)](https://github.com/gpajot/zen-config/actions?query=workflow%3ATest+branch%3Amain+event%3Apush)
+[![tests](https://github.com/gpajot/zen-config/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/gpajot/zen-config/actions/workflows/test.yml?query=branch%3Amain+event%3Apush)
 [![version](https://img.shields.io/pypi/v/zenconfig?label=stable)](https://pypi.org/project/zenconfig/)
 [![python](https://img.shields.io/pypi/pyversions/zenconfig)](https://pypi.org/project/zenconfig/)
 
 Simple configuration loader for python.
 
 Compared to other solutions, the goal is to bring:
 - simple usage for simple use cases
```

