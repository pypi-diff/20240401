# Comparing `tmp/flake8_pytest_style-1.7.2.tar.gz` & `tmp/flake8_pytest_style-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_pytest_style-1.7.2.tar", max compression
+gzip compressed data, was "flake8_pytest_style-2.0.0.tar", max compression
```

## Comparing `flake8_pytest_style-1.7.2.tar` & `flake8_pytest_style-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     1074 2021-06-18 10:06:28.450716 flake8_pytest_style-1.7.2/LICENSE
--rw-r--r--   0        0        0     9904 2023-02-15 07:38:51.419749 flake8_pytest_style-1.7.2/README-pypi.md
--rw-r--r--   0        0        0        0 2021-06-18 10:06:28.455085 flake8_pytest_style-1.7.2/flake8_pytest_style/__init__.py
--rw-r--r--   0        0        0     1148 2021-06-18 10:06:28.455225 flake8_pytest_style-1.7.2/flake8_pytest_style/config.py
--rw-r--r--   0        0        0     3884 2023-02-09 20:52:07.327124 flake8_pytest_style-1.7.2/flake8_pytest_style/errors.py
--rw-r--r--   0        0        0     4027 2023-02-15 07:38:24.694676 flake8_pytest_style-1.7.2/flake8_pytest_style/plugin.py
--rw-r--r--   0        0        0        0 2022-07-11 16:32:23.780000 flake8_pytest_style-1.7.2/flake8_pytest_style/py.typed
--rw-r--r--   0        0        0     9328 2021-06-18 10:06:28.455726 flake8_pytest_style-1.7.2/flake8_pytest_style/utils.py
--rw-r--r--   0        0        0      534 2021-06-18 10:06:28.455939 flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/__init__.py
--rw-r--r--   0        0        0     3015 2023-02-15 07:35:43.069201 flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/assertion.py
--rw-r--r--   0        0        0      954 2021-06-18 10:06:28.456316 flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/fail.py
--rw-r--r--   0        0        0     6672 2021-06-18 10:06:28.456482 flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/fixtures.py
--rw-r--r--   0        0        0      914 2021-06-18 10:06:28.456619 flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/imports.py
--rw-r--r--   0        0        0     2326 2021-06-18 10:06:28.456769 flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/marks.py
--rw-r--r--   0        0        0     4771 2021-06-18 10:06:28.456947 flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/parametrize.py
--rw-r--r--   0        0        0     1781 2021-06-18 10:06:28.457089 flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/patch.py
--rw-r--r--   0        0        0     3127 2022-07-11 16:32:23.780419 flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/raises.py
--rw-r--r--   0        0        0     1370 2023-02-15 07:38:51.420559 flake8_pytest_style-1.7.2/pyproject.toml
--rw-r--r--   0        0        0    11074 1970-01-01 00:00:00.000000 flake8_pytest_style-1.7.2/setup.py
--rw-r--r--   0        0        0    11177 1970-01-01 00:00:00.000000 flake8_pytest_style-1.7.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1074 2019-05-18 21:00:28.085109 flake8_pytest_style-2.0.0/LICENSE
+-rwxr-xr-x   0        0        0    10272 2024-04-01 17:15:06.028266 flake8_pytest_style-2.0.0/README-pypi.md
+-rwxr-xr-x   0        0        0        0 2019-05-21 21:51:56.432747 flake8_pytest_style-2.0.0/flake8_pytest_style/__init__.py
+-rwxr-xr-x   0        0        0     1150 2024-04-01 15:53:22.808188 flake8_pytest_style-2.0.0/flake8_pytest_style/config.py
+-rwxr-xr-x   0        0        0     3884 2024-04-01 13:46:04.569539 flake8_pytest_style-2.0.0/flake8_pytest_style/errors.py
+-rwxr-xr-x   0        0        0     4027 2024-04-01 17:09:20.832634 flake8_pytest_style-2.0.0/flake8_pytest_style/plugin.py
+-rwxr-xr-x   0        0        0        0 2021-12-22 21:16:40.698762 flake8_pytest_style-2.0.0/flake8_pytest_style/py.typed
+-rwxr-xr-x   0        0        0     9328 2021-04-01 20:09:10.777207 flake8_pytest_style-2.0.0/flake8_pytest_style/utils.py
+-rwxr-xr-x   0        0        0      534 2021-03-13 11:11:11.309768 flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/__init__.py
+-rwxr-xr-x   0        0        0     3015 2024-04-01 13:46:04.594981 flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/assertion.py
+-rwxr-xr-x   0        0        0      954 2021-04-01 20:09:10.815206 flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/fail.py
+-rwxr-xr-x   0        0        0     6708 2024-04-01 13:46:04.607727 flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/fixtures.py
+-rwxr-xr-x   0        0        0      914 2021-04-01 20:09:10.847211 flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/imports.py
+-rwxr-xr-x   0        0        0     2326 2021-06-18 08:20:59.333458 flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/marks.py
+-rwxr-xr-x   0        0        0     4771 2021-04-01 20:09:10.881217 flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/parametrize.py
+-rwxr-xr-x   0        0        0     1781 2021-04-01 20:09:10.897212 flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/patch.py
+-rwxr-xr-x   0        0        0     3127 2021-11-05 11:09:42.981132 flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/raises.py
+-rwxr-xr-x   0        0        0     1371 2024-04-01 17:15:06.033266 flake8_pytest_style-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11546 1970-01-01 00:00:00.000000 flake8_pytest_style-2.0.0/PKG-INFO
```

### Comparing `flake8_pytest_style-1.7.2/LICENSE` & `flake8_pytest_style-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_pytest_style-1.7.2/README-pypi.md` & `flake8_pytest_style-2.0.0/README-pypi.md`

 * *Files 8% similar despite different names*

```diff
@@ -81,14 +81,23 @@
 
 ## Change Log
 
 **Unreleased**
 
 ...
 
+**2.0.0 - 2024-04-01**
+
+* **BREAKING:** invert default values for `pytest-fixture-no-parentheses` and `pytest-mark-no-parentheses`
+  to conform with `pytest` official style
+  * If you get a lot of [PT001] or [PT023] violations after upgrading, consider setting explicit values
+    for these configuration options
+* require at least Python 3.8.1
+* support Python 3.12
+
 **1.7.2 - 2023-02-15**
 
 * fix false positive for [PT009] on `pytest.fail`
 
 **1.7.1 - 2023-02-15**
 
 * update list of unittest-style assert methods for [PT009]/[PT027]
@@ -214,34 +223,34 @@
 
 * update PyPI description
 
 **0.1.0 - 2019-05-23**
 
 * initial
 
-[PT001]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT001.md
-[PT002]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT002.md
-[PT003]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT003.md
-[PT004]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT004.md
-[PT005]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT005.md
-[PT006]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT006.md
-[PT007]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT007.md
-[PT008]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT008.md
-[PT009]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT009.md
-[PT010]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT010.md
-[PT011]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT011.md
-[PT012]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT012.md
-[PT013]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT013.md
-[PT014]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT014.md
-[PT015]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT015.md
-[PT016]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT016.md
-[PT017]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT017.md
-[PT018]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT018.md
-[PT019]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT019.md
-[PT020]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT020.md
-[PT021]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT021.md
-[PT022]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT022.md
-[PT023]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT023.md
-[PT024]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT024.md
-[PT025]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT025.md
-[PT026]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT026.md
-[PT027]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT027.md
+[PT001]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT001.md
+[PT002]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT002.md
+[PT003]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT003.md
+[PT004]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT004.md
+[PT005]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT005.md
+[PT006]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT006.md
+[PT007]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT007.md
+[PT008]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT008.md
+[PT009]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT009.md
+[PT010]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT010.md
+[PT011]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT011.md
+[PT012]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT012.md
+[PT013]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT013.md
+[PT014]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT014.md
+[PT015]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT015.md
+[PT016]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT016.md
+[PT017]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT017.md
+[PT018]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT018.md
+[PT019]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT019.md
+[PT020]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT020.md
+[PT021]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT021.md
+[PT022]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT022.md
+[PT023]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT023.md
+[PT024]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT024.md
+[PT025]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT025.md
+[PT026]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT026.md
+[PT027]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT027.md
```

### Comparing `flake8_pytest_style-1.7.2/flake8_pytest_style/config.py` & `flake8_pytest_style-2.0.0/flake8_pytest_style/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,22 +28,22 @@
     parametrize_names_type: ParametrizeNamesType
     parametrize_values_type: ParametrizeValuesType
     parametrize_values_row_type: ParametrizeValuesRowType
     mark_parentheses: bool
 
 
 DEFAULT_CONFIG = Config(
-    fixture_parentheses=True,
+    fixture_parentheses=False,
     raises_require_match_for=[
         'BaseException',
         'Exception',
         'ValueError',
         'IOError',
         'OSError',
         'EnvironmentError',
         'socket.error',
     ],
     parametrize_names_type=ParametrizeNamesType.TUPLE,
     parametrize_values_type=ParametrizeValuesType.LIST,
     parametrize_values_row_type=ParametrizeValuesRowType.TUPLE,
-    mark_parentheses=True,
+    mark_parentheses=False,
 )
```

### Comparing `flake8_pytest_style-1.7.2/flake8_pytest_style/errors.py` & `flake8_pytest_style-2.0.0/flake8_pytest_style/errors.py`

 * *Files identical despite different names*

### Comparing `flake8_pytest_style-1.7.2/flake8_pytest_style/plugin.py` & `flake8_pytest_style-2.0.0/flake8_pytest_style/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     MarksVisitor,
     ParametrizeVisitor,
     PatchVisitor,
     RaisesVisitor,
     UnittestAssertionVisitor,
 )
 
-__version__ = '1.7.2'
+__version__ = '2.0.0'
 
 
 class PytestStylePlugin(Plugin[Config]):
     name = 'flake8-pytest-style'
     version = __version__
     visitors = [
         AssertionVisitor,
```

### Comparing `flake8_pytest_style-1.7.2/flake8_pytest_style/utils.py` & `flake8_pytest_style-2.0.0/flake8_pytest_style/utils.py`

 * *Files identical despite different names*

### Comparing `flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/__init__.py` & `flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/__init__.py`

 * *Files identical despite different names*

### Comparing `flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/assertion.py` & `flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/assertion.py`

 * *Files identical despite different names*

### Comparing `flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/fail.py` & `flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/fail.py`

 * *Files identical despite different names*

### Comparing `flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/fixtures.py` & `flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ast
-from typing import Union
+from typing import Set, Type, Union
 
-from flake8_plugin_utils import Visitor
+from flake8_plugin_utils import Error, Visitor
 
 from flake8_pytest_style.config import Config
 from flake8_pytest_style.errors import (
     DeprecatedYieldFixture,
     ErroneousUseFixturesOnFixture,
     ExtraneousScopeFunction,
     FixtureFinalizerCallback,
@@ -131,15 +131,15 @@
                 and get_qualname(child.func) == 'request.addfinalizer'
             ):
                 self.error_from_node(FixtureFinalizerCallback, child)
                 return
 
     def _check_fixture_marks(self, node: AnyFunctionDef) -> None:
         """Checks for PT024, PT025."""
-        reported_errors = set()
+        reported_errors: Set[Type[Error]] = set()
         marks = get_mark_decorators(node)
         for mark in marks:
             mark_name = get_mark_name(mark)
             if (
                 mark_name == 'asyncio'
                 and UnnecessaryAsyncioMarkOnFixture not in reported_errors
             ):
```

### Comparing `flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/imports.py` & `flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/imports.py`

 * *Files identical despite different names*

### Comparing `flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/marks.py` & `flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/marks.py`

 * *Files identical despite different names*

### Comparing `flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/parametrize.py` & `flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/parametrize.py`

 * *Files identical despite different names*

### Comparing `flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/patch.py` & `flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/patch.py`

 * *Files identical despite different names*

### Comparing `flake8_pytest_style-1.7.2/flake8_pytest_style/visitors/raises.py` & `flake8_pytest_style-2.0.0/flake8_pytest_style/visitors/raises.py`

 * *Files identical despite different names*

### Comparing `flake8_pytest_style-1.7.2/pyproject.toml` & `flake8_pytest_style-2.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flake8-pytest-style"
-version = "1.7.2"
+version = "2.0.0"
 description = "A flake8 plugin checking common style issues or inconsistencies with pytest-based tests."
 authors = ["Mikhail Burshteyn <mdburshteyn@gmail.com>"]
 license = "MIT"
 readme = "README-pypi.md"
 repository = "https://github.com/m-burst/flake8-pytest-style"
 homepage = "https://pypi.org/project/flake8-pytest-style"
 keywords = ["flake8", "pytest"]
@@ -21,27 +21,27 @@
   "Topic :: Software Development :: Testing :: Unit",
 ]
 
 [tool.poetry.plugins."flake8.extension"]
 PT = 'flake8_pytest_style.plugin:PytestStylePlugin'
 
 [tool.poetry.dependencies]
-python = "^3.7.2"
+python = "^3.8.1"
 flake8-plugin-utils = "^1.3.2"
 
-[tool.poetry.dev-dependencies]
-black = {version = "^23.1"}
+[tool.poetry.group.dev.dependencies]
+black = "^24.3.0"
 bump2version = "^1.0.1"
 flake8-awesome = ">=0.2.0"
-mypy = "^1.0"
-pylint = "^2.16"
-pytest = "^7.2"
-pytest-cov = "^4.0"
+mypy = "^1.4"
+pylint = "^3.1.0"
+pytest = "^8.1.1"
+pytest-cov = "5.0.0"
 pytest-deadfixtures = "^2.1"
-flake8 = "^4.0.1"
-pytest-mock = "^3.6.0"
+flake8 = "^7.0.0"
+pytest-mock = "^3.11.1"
 unify = "^0.5.0"
-tomlkit = "^0.11.4"
+tomlkit = "^0.12.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `flake8_pytest_style-1.7.2/setup.py` & `flake8_pytest_style-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,287 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: flake8-pytest-style
+Version: 2.0.0
+Summary: A flake8 plugin checking common style issues or inconsistencies with pytest-based tests.
+Home-page: https://pypi.org/project/flake8-pytest-style
+License: MIT
+Keywords: flake8,pytest
+Author: Mikhail Burshteyn
+Author-email: mdburshteyn@gmail.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Plugins
+Classifier: Framework :: Flake8
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Unit
+Requires-Dist: flake8-plugin-utils (>=1.3.2,<2.0.0)
+Project-URL: Repository, https://github.com/m-burst/flake8-pytest-style
+Description-Content-Type: text/markdown
 
-packages = \
-['flake8_pytest_style', 'flake8_pytest_style.visitors']
+# flake8-pytest-style
 
-package_data = \
-{'': ['*']}
+[![pypi](https://badge.fury.io/py/flake8-pytest-style.svg)](https://pypi.org/project/flake8-pytest-style)
+[![Python: 3.7+](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://pypi.org/project/flake8-pytest-style)
+[![Downloads](https://img.shields.io/pypi/dm/flake8-pytest-style.svg)](https://pypistats.org/packages/flake8-pytest-style)
+[![Build Status](https://github.com/m-burst/flake8-pytest-style/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/m-burst/flake8-pytest-style/actions/workflows/ci.yml)
+[![Code coverage](https://codecov.io/gh/m-burst/flake8-pytest-style/branch/master/graph/badge.svg)](https://codecov.io/gh/m-burst/flake8-pytest-style)
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://en.wikipedia.org/wiki/MIT_License)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
-install_requires = \
-['flake8-plugin-utils>=1.3.2,<2.0.0']
-
-entry_points = \
-{'flake8.extension': ['PT = flake8_pytest_style.plugin:PytestStylePlugin']}
-
-setup_kwargs = {
-    'name': 'flake8-pytest-style',
-    'version': '1.7.2',
-    'description': 'A flake8 plugin checking common style issues or inconsistencies with pytest-based tests.',
-    'long_description': "# flake8-pytest-style\n\n[![pypi](https://badge.fury.io/py/flake8-pytest-style.svg)](https://pypi.org/project/flake8-pytest-style)\n[![Python: 3.7+](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://pypi.org/project/flake8-pytest-style)\n[![Downloads](https://img.shields.io/pypi/dm/flake8-pytest-style.svg)](https://pypistats.org/packages/flake8-pytest-style)\n[![Build Status](https://github.com/m-burst/flake8-pytest-style/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/m-burst/flake8-pytest-style/actions/workflows/ci.yml)\n[![Code coverage](https://codecov.io/gh/m-burst/flake8-pytest-style/branch/master/graph/badge.svg)](https://codecov.io/gh/m-burst/flake8-pytest-style)\n[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://en.wikipedia.org/wiki/MIT_License)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n\n## Description\n\nA `flake8` plugin checking common style issues or inconsistencies with `pytest`-based tests.\n\nCurrently the following errors are reported:\n\n| Code    | Description |\n| ------- | ----------- |\n| [PT001] | use @pytest.fixture() over @pytest.fixture <br> (configurable by `pytest-fixture-no-parentheses`) |\n| [PT002] | configuration for fixture '{name}' specified via positional args, use kwargs |\n| [PT003] | scope='function' is implied in @pytest.fixture() |\n| [PT004] | fixture '{name}' does not return anything, add leading underscore |\n| [PT005] | fixture '{name}' returns a value, remove leading underscore |\n| [PT006] | wrong name(s) type in @pytest.mark.parametrize, expected {expected_type} <br> (configurable by `pytest-parametrize-names-type`) |\n| [PT007] | wrong values type in @pytest.mark.parametrize, expected {expected_type} <br> (configurable by `pytest-parametrize-values-type` and `pytest-parametrize-values-row-type`) |\n| [PT008] | use return_value= instead of patching with lambda |\n| [PT009] | use a regular assert instead of unittest-style '{assertion}' |\n| [PT010] | set the expected exception in pytest.raises() |\n| [PT011] | pytest.raises({exception}) is too broad, set the match parameter or use a more specific exception <br> (configurable by `pytest-raises-require-match-for`) |\n| [PT012] | pytest.raises() block should contain a single simple statement |\n| [PT013] | found incorrect import of pytest, use simple 'import pytest' instead |\n| [PT014] | found duplicate test cases {indexes} in @pytest.mark.parametrize |\n| [PT015] | assertion always fails, replace with pytest.fail() |\n| [PT016] | no message passed to pytest.fail() |\n| [PT017] | found assertion on exception {name} in except block, use pytest.raises() instead |\n| [PT018] | assertion should be broken down into multiple parts |\n| [PT019] | fixture {name} without value is injected as parameter, use @pytest.mark.usefixtures instead |\n| [PT020] | @pytest.yield_fixture is deprecated, use @pytest.fixture |\n| [PT021] | use yield instead of request.addfinalizer |\n| [PT022] | no teardown in fixture {name}, use return instead of yield |\n| [PT023] | use @pytest.mark.foo() over @pytest.mark.foo <br> (configurable by `pytest-mark-no-parentheses`) |\n| [PT024] | pytest.mark.asyncio is unnecessary for fixtures |\n| [PT025] | pytest.mark.usefixtures has no effect on fixtures |\n| [PT026] | useless pytest.mark.usefixtures without parameters | \n| [PT027] | use pytest.raises() instead of unittest-style '{assertion}' |\n\n## Installation\n\n    pip install flake8-pytest-style\n\n## Configuration\n\nThe plugin has the following configuration options:\n\n* `pytest-fixture-no-parentheses` &mdash; see [PT001]\n* `pytest-parametrize-names-type` &mdash; see [PT006]\n* `pytest-parametrize-values-type` &mdash; see [PT007]\n* `pytest-parametrize-values-row-type` &mdash; see [PT007]\n* `pytest-raises-require-match-for` &mdash; see [PT011]\n* `pytest-mark-no-parentheses` &mdash; see [PT023]\n\n## For developers\n\n### Install deps and setup pre-commit hook\n\n    make init\n\n### Run linters, autoformat, tests etc.\n\n    make format lint test\n\n### Bump new version\n\n    make bump_major\n    make bump_minor\n    make bump_patch\n\n## License\n\nMIT\n\n## Change Log\n\n**Unreleased**\n\n...\n\n**1.7.2 - 2023-02-15**\n\n* fix false positive for [PT009] on `pytest.fail`\n\n**1.7.1 - 2023-02-15**\n\n* update list of unittest-style assert methods for [PT009]/[PT027]\n\n**1.7.0 - 2023-02-09**\n\n* require at least Python 3.7.2\n* support Python 3.11\n* add [PT027] (checks for unittest-style `assertRaises`)\n\n**1.6.0 - 2021-12-23**\n\n* require at least Python 3.6.2\n* expose `py.typed` file\n\n**1.5.1 - 2021-11-05**\n\n* better wording for [PT011]\n* support Python 3.10\n\n**1.5.0 - 2021-06-18**\n\n* add [PT025] (checks for erroneous `pytest.mark.usefixtures` on fixtures)\n* add [PT026] (checks for `pytest.mark.usefixtures` without parameters)\n\n**1.4.4 - 2021-06-17**\n\n* fix [PT023] not checking marks in classes\n* fix [PT004] incorrectly firing on fixtures with `yield from`\n\n**1.4.2 - 2021-05-24**\n\n* update `flake8-plugin-utils` version to improve stability\n\n**1.4.1 - 2021-04-01**\n\n* fix argparse-related warnings\n\n**1.4.0 - 2021-03-14**\n\n* add [PT023] (checks for parentheses consistency in `pytest.mark` usage)\n* add [PT024] (checks for unnecessary `pytest.mark.asyncio` on fixtures)\n* fix [PT004], [PT005] firing on abstract fixtures\n* fix [PT012] firing on `with` statements containing a single `pass`\n\n**1.3.0 - 2020-08-30**\n\n* add [PT022] (checks for `yield` fixtures without teardown)\n\n**1.2.3 - 2020-08-06**\n\n* update `flake8-plugin-utils` dependency to fix encoding problems on Windows\n\n**1.2.2 - 2020-07-23**\n\n* fix [PT004]/[PT005] inspecting returns of nested functions\n\n**1.2.1 - 2020-06-15**\n\n* fix [PT021] for factory fixtures (#46)\n\n**1.2.0 - 2020-06-12**\n\n* support scoped `mocker` fixtures from `pytest-mock` for [PT008]\n* check for positional-only lambda arguments in [PT008]\n* add [PT020] (checks for `pytest.yield_fixture`)\n* add [PT021] (checks for `request.addfinalizer`)\n* add documentation pages for all rules\n\n**1.1.1 - 2020-04-17**\n\n* fix [PT011] not reporting `match=''` as a violation\n\n**1.1.0 - 2020-04-14**\n\n* add [PT015] (checks for `assert False`)\n* add [PT016] (checks for `pytest.fail()` without message)\n* add [PT017] (checks for assertions on exceptions in `except` blocks)\n* add [PT018] (checks for composite assertions)\n* add [PT019] (checks for fixtures without value injected as parameters)\n\n**1.0.0 - 2020-03-26**\n\n* add [PT014] (checks for duplicate test cases in `@pytest.mark.parametrize`)\n\n**0.6.0 - 2020-03-21**\n\n* add configuration option `pytest-parametrize-names-type` for [PT006]\n* add configuration options `pytest-parametrize-values-type` and\n`pytest-parametrize-values-row-type` for [PT007]\n\n**0.5.0 - 2020-03-09**\n\n* add configuration option `pytest-fixture-no-parentheses` for [PT001]\n* add [PT013] (checks for `from`-imports from `pytest`)\n\n**0.4.0 - 2020-03-09**\n\n* add [PT012] (checks for multiple statements in `with pytest.raises()`)\n\n**0.3.1 - 2020-03-09**\n\n* fix default value of `pytest-raises-require-match-for` config option\n\n**0.3.0 - 2020-03-09**\n\n* add [PT010] and [PT011] (checks for `pytest.raises` parameters)\n\n**0.2.0 - 2020-03-01**\n\n* add [PT009] (ported from [flake8-pytest](https://github.com/vikingco/flake8-pytest))\n\n**0.1.3 - 2019-05-24**\n\n* add `yield` fixtures support\n* fix changelog entry for 0.1.2\n\n**0.1.2 - 2019-05-23**\n\n* fix parametrize checkers not working in decorators\n\n**0.1.1 - 2019-05-23**\n\n* update PyPI description\n\n**0.1.0 - 2019-05-23**\n\n* initial\n\n[PT001]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT001.md\n[PT002]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT002.md\n[PT003]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT003.md\n[PT004]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT004.md\n[PT005]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT005.md\n[PT006]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT006.md\n[PT007]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT007.md\n[PT008]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT008.md\n[PT009]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT009.md\n[PT010]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT010.md\n[PT011]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT011.md\n[PT012]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT012.md\n[PT013]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT013.md\n[PT014]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT014.md\n[PT015]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT015.md\n[PT016]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT016.md\n[PT017]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT017.md\n[PT018]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT018.md\n[PT019]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT019.md\n[PT020]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT020.md\n[PT021]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT021.md\n[PT022]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT022.md\n[PT023]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT023.md\n[PT024]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT024.md\n[PT025]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT025.md\n[PT026]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT026.md\n[PT027]: https://github.com/m-burst/flake8-pytest-style/blob/v1.7.2/docs/rules/PT027.md\n",
-    'author': 'Mikhail Burshteyn',
-    'author_email': 'mdburshteyn@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://pypi.org/project/flake8-pytest-style',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.2,<4.0.0',
-}
+## Description
 
+A `flake8` plugin checking common style issues or inconsistencies with `pytest`-based tests.
+
+Currently the following errors are reported:
+
+| Code    | Description |
+| ------- | ----------- |
+| [PT001] | use @pytest.fixture() over @pytest.fixture <br> (configurable by `pytest-fixture-no-parentheses`) |
+| [PT002] | configuration for fixture '{name}' specified via positional args, use kwargs |
+| [PT003] | scope='function' is implied in @pytest.fixture() |
+| [PT004] | fixture '{name}' does not return anything, add leading underscore |
+| [PT005] | fixture '{name}' returns a value, remove leading underscore |
+| [PT006] | wrong name(s) type in @pytest.mark.parametrize, expected {expected_type} <br> (configurable by `pytest-parametrize-names-type`) |
+| [PT007] | wrong values type in @pytest.mark.parametrize, expected {expected_type} <br> (configurable by `pytest-parametrize-values-type` and `pytest-parametrize-values-row-type`) |
+| [PT008] | use return_value= instead of patching with lambda |
+| [PT009] | use a regular assert instead of unittest-style '{assertion}' |
+| [PT010] | set the expected exception in pytest.raises() |
+| [PT011] | pytest.raises({exception}) is too broad, set the match parameter or use a more specific exception <br> (configurable by `pytest-raises-require-match-for`) |
+| [PT012] | pytest.raises() block should contain a single simple statement |
+| [PT013] | found incorrect import of pytest, use simple 'import pytest' instead |
+| [PT014] | found duplicate test cases {indexes} in @pytest.mark.parametrize |
+| [PT015] | assertion always fails, replace with pytest.fail() |
+| [PT016] | no message passed to pytest.fail() |
+| [PT017] | found assertion on exception {name} in except block, use pytest.raises() instead |
+| [PT018] | assertion should be broken down into multiple parts |
+| [PT019] | fixture {name} without value is injected as parameter, use @pytest.mark.usefixtures instead |
+| [PT020] | @pytest.yield_fixture is deprecated, use @pytest.fixture |
+| [PT021] | use yield instead of request.addfinalizer |
+| [PT022] | no teardown in fixture {name}, use return instead of yield |
+| [PT023] | use @pytest.mark.foo() over @pytest.mark.foo <br> (configurable by `pytest-mark-no-parentheses`) |
+| [PT024] | pytest.mark.asyncio is unnecessary for fixtures |
+| [PT025] | pytest.mark.usefixtures has no effect on fixtures |
+| [PT026] | useless pytest.mark.usefixtures without parameters | 
+| [PT027] | use pytest.raises() instead of unittest-style '{assertion}' |
+
+## Installation
+
+    pip install flake8-pytest-style
+
+## Configuration
+
+The plugin has the following configuration options:
+
+* `pytest-fixture-no-parentheses` &mdash; see [PT001]
+* `pytest-parametrize-names-type` &mdash; see [PT006]
+* `pytest-parametrize-values-type` &mdash; see [PT007]
+* `pytest-parametrize-values-row-type` &mdash; see [PT007]
+* `pytest-raises-require-match-for` &mdash; see [PT011]
+* `pytest-mark-no-parentheses` &mdash; see [PT023]
+
+## For developers
+
+### Install deps and setup pre-commit hook
+
+    make init
+
+### Run linters, autoformat, tests etc.
+
+    make format lint test
+
+### Bump new version
+
+    make bump_major
+    make bump_minor
+    make bump_patch
+
+## License
+
+MIT
+
+## Change Log
+
+**Unreleased**
+
+...
+
+**2.0.0 - 2024-04-01**
+
+* **BREAKING:** invert default values for `pytest-fixture-no-parentheses` and `pytest-mark-no-parentheses`
+  to conform with `pytest` official style
+  * If you get a lot of [PT001] or [PT023] violations after upgrading, consider setting explicit values
+    for these configuration options
+* require at least Python 3.8.1
+* support Python 3.12
+
+**1.7.2 - 2023-02-15**
+
+* fix false positive for [PT009] on `pytest.fail`
+
+**1.7.1 - 2023-02-15**
+
+* update list of unittest-style assert methods for [PT009]/[PT027]
+
+**1.7.0 - 2023-02-09**
+
+* require at least Python 3.7.2
+* support Python 3.11
+* add [PT027] (checks for unittest-style `assertRaises`)
+
+**1.6.0 - 2021-12-23**
+
+* require at least Python 3.6.2
+* expose `py.typed` file
+
+**1.5.1 - 2021-11-05**
+
+* better wording for [PT011]
+* support Python 3.10
+
+**1.5.0 - 2021-06-18**
+
+* add [PT025] (checks for erroneous `pytest.mark.usefixtures` on fixtures)
+* add [PT026] (checks for `pytest.mark.usefixtures` without parameters)
+
+**1.4.4 - 2021-06-17**
+
+* fix [PT023] not checking marks in classes
+* fix [PT004] incorrectly firing on fixtures with `yield from`
+
+**1.4.2 - 2021-05-24**
+
+* update `flake8-plugin-utils` version to improve stability
+
+**1.4.1 - 2021-04-01**
+
+* fix argparse-related warnings
+
+**1.4.0 - 2021-03-14**
+
+* add [PT023] (checks for parentheses consistency in `pytest.mark` usage)
+* add [PT024] (checks for unnecessary `pytest.mark.asyncio` on fixtures)
+* fix [PT004], [PT005] firing on abstract fixtures
+* fix [PT012] firing on `with` statements containing a single `pass`
+
+**1.3.0 - 2020-08-30**
+
+* add [PT022] (checks for `yield` fixtures without teardown)
+
+**1.2.3 - 2020-08-06**
+
+* update `flake8-plugin-utils` dependency to fix encoding problems on Windows
+
+**1.2.2 - 2020-07-23**
+
+* fix [PT004]/[PT005] inspecting returns of nested functions
+
+**1.2.1 - 2020-06-15**
+
+* fix [PT021] for factory fixtures (#46)
+
+**1.2.0 - 2020-06-12**
+
+* support scoped `mocker` fixtures from `pytest-mock` for [PT008]
+* check for positional-only lambda arguments in [PT008]
+* add [PT020] (checks for `pytest.yield_fixture`)
+* add [PT021] (checks for `request.addfinalizer`)
+* add documentation pages for all rules
+
+**1.1.1 - 2020-04-17**
+
+* fix [PT011] not reporting `match=''` as a violation
+
+**1.1.0 - 2020-04-14**
+
+* add [PT015] (checks for `assert False`)
+* add [PT016] (checks for `pytest.fail()` without message)
+* add [PT017] (checks for assertions on exceptions in `except` blocks)
+* add [PT018] (checks for composite assertions)
+* add [PT019] (checks for fixtures without value injected as parameters)
+
+**1.0.0 - 2020-03-26**
+
+* add [PT014] (checks for duplicate test cases in `@pytest.mark.parametrize`)
+
+**0.6.0 - 2020-03-21**
+
+* add configuration option `pytest-parametrize-names-type` for [PT006]
+* add configuration options `pytest-parametrize-values-type` and
+`pytest-parametrize-values-row-type` for [PT007]
+
+**0.5.0 - 2020-03-09**
+
+* add configuration option `pytest-fixture-no-parentheses` for [PT001]
+* add [PT013] (checks for `from`-imports from `pytest`)
+
+**0.4.0 - 2020-03-09**
+
+* add [PT012] (checks for multiple statements in `with pytest.raises()`)
+
+**0.3.1 - 2020-03-09**
+
+* fix default value of `pytest-raises-require-match-for` config option
+
+**0.3.0 - 2020-03-09**
+
+* add [PT010] and [PT011] (checks for `pytest.raises` parameters)
+
+**0.2.0 - 2020-03-01**
+
+* add [PT009] (ported from [flake8-pytest](https://github.com/vikingco/flake8-pytest))
+
+**0.1.3 - 2019-05-24**
+
+* add `yield` fixtures support
+* fix changelog entry for 0.1.2
+
+**0.1.2 - 2019-05-23**
+
+* fix parametrize checkers not working in decorators
+
+**0.1.1 - 2019-05-23**
+
+* update PyPI description
+
+**0.1.0 - 2019-05-23**
+
+* initial
+
+[PT001]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT001.md
+[PT002]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT002.md
+[PT003]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT003.md
+[PT004]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT004.md
+[PT005]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT005.md
+[PT006]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT006.md
+[PT007]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT007.md
+[PT008]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT008.md
+[PT009]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT009.md
+[PT010]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT010.md
+[PT011]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT011.md
+[PT012]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT012.md
+[PT013]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT013.md
+[PT014]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT014.md
+[PT015]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT015.md
+[PT016]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT016.md
+[PT017]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT017.md
+[PT018]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT018.md
+[PT019]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT019.md
+[PT020]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT020.md
+[PT021]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT021.md
+[PT022]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT022.md
+[PT023]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT023.md
+[PT024]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT024.md
+[PT025]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT025.md
+[PT026]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT026.md
+[PT027]: https://github.com/m-burst/flake8-pytest-style/blob/v2.0.0/docs/rules/PT027.md
 
-setup(**setup_kwargs)
```

