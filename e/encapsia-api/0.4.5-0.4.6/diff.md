# Comparing `tmp/encapsia_api-0.4.5.tar.gz` & `tmp/encapsia_api-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encapsia_api-0.4.5.tar", max compression
+gzip compressed data, was "encapsia_api-0.4.6.tar", max compression
```

## Comparing `encapsia_api-0.4.5.tar` & `encapsia_api-0.4.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1078 2022-01-07 06:44:29.651749 encapsia_api-0.4.5/LICENSE
--rw-r--r--   0        0        0     2863 2023-05-05 07:11:44.945138 encapsia_api-0.4.5/README.md
--rw-r--r--   0        0        0      595 2024-01-08 11:20:15.918225 encapsia_api-0.4.5/encapsia_api/__init__.py
--rw-r--r--   0        0        0     1877 2023-05-05 07:11:44.949138 encapsia_api-0.4.5/encapsia_api/analytics.py
--rw-r--r--   0        0        0     2858 2024-01-08 11:20:15.922225 encapsia_api-0.4.5/encapsia_api/credentials.py
--rw-r--r--   0        0        0     3007 2023-05-05 07:11:44.949138 encapsia_api-0.4.5/encapsia_api/lib.py
--rw-r--r--   0        0        0     6255 2024-01-08 11:20:15.922225 encapsia_api-0.4.5/encapsia_api/package.py
--rw-r--r--   0        0        0     3407 2024-01-08 11:20:15.922225 encapsia_api-0.4.5/encapsia_api/plugin.py
--rw-r--r--   0        0        0        0 2023-10-13 07:21:41.780961 encapsia_api-0.4.5/encapsia_api/py.typed
--rw-r--r--   0        0        0     3987 2023-05-05 07:11:44.949138 encapsia_api-0.4.5/encapsia_api/resilient_request.py
--rw-r--r--   0        0        0    32926 2024-01-08 11:20:15.922225 encapsia_api-0.4.5/encapsia_api/rest.py
--rw-r--r--   0        0        0        0 2023-10-13 07:21:41.780961 encapsia_api-0.4.5/encapsia_api/tests/__init__.py
--rw-r--r--   0        0        0     3516 2023-05-05 07:11:44.949138 encapsia_api-0.4.5/encapsia_api/tests/test_credentials.py
--rw-r--r--   0        0        0     6371 2023-05-05 07:11:44.949138 encapsia_api-0.4.5/encapsia_api/tests/test_package.py
--rw-r--r--   0        0        0      536 2023-05-05 07:11:44.949138 encapsia_api-0.4.5/encapsia_api/tests/test_plugin.py
--rw-r--r--   0        0        0     9154 2023-05-05 07:11:44.949138 encapsia_api-0.4.5/encapsia_api/tests/test_resilient_request.py
--rw-r--r--   0        0        0     7006 2023-05-02 17:09:35.347096 encapsia_api-0.4.5/encapsia_api/tests/test_rest.py
--rw-r--r--   0        0        0      566 2023-05-05 07:11:44.949138 encapsia_api-0.4.5/encapsia_api/util.py
--rw-r--r--   0        0        0     3472 2024-01-08 11:20:15.922225 encapsia_api-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 encapsia_api-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-01-07 06:44:29.651749 encapsia_api-0.4.6/LICENSE
+-rw-r--r--   0        0        0     2863 2023-05-05 07:11:44.945138 encapsia_api-0.4.6/README.md
+-rw-r--r--   0        0        0      595 2024-04-01 09:06:52.985905 encapsia_api-0.4.6/encapsia_api/__init__.py
+-rw-r--r--   0        0        0     1877 2024-04-01 09:01:54.171375 encapsia_api-0.4.6/encapsia_api/analytics.py
+-rw-r--r--   0        0        0     2858 2024-04-01 09:01:54.171375 encapsia_api-0.4.6/encapsia_api/credentials.py
+-rw-r--r--   0        0        0     3035 2024-04-01 09:16:18.078304 encapsia_api-0.4.6/encapsia_api/lib.py
+-rw-r--r--   0        0        0     6254 2024-04-01 09:05:22.241159 encapsia_api-0.4.6/encapsia_api/package.py
+-rw-r--r--   0        0        0     3406 2024-04-01 09:05:22.185158 encapsia_api-0.4.6/encapsia_api/plugin.py
+-rw-r--r--   0        0        0        0 2023-10-13 07:21:41.780961 encapsia_api-0.4.6/encapsia_api/py.typed
+-rw-r--r--   0        0        0     3987 2024-04-01 09:01:54.171375 encapsia_api-0.4.6/encapsia_api/resilient_request.py
+-rw-r--r--   0        0        0    33035 2024-04-01 09:28:35.087754 encapsia_api-0.4.6/encapsia_api/rest.py
+-rw-r--r--   0        0        0        0 2023-10-13 07:21:41.780961 encapsia_api-0.4.6/encapsia_api/tests/__init__.py
+-rw-r--r--   0        0        0     3516 2023-05-05 07:11:44.949138 encapsia_api-0.4.6/encapsia_api/tests/test_credentials.py
+-rw-r--r--   0        0        0     6432 2024-04-01 09:32:49.605609 encapsia_api-0.4.6/encapsia_api/tests/test_package.py
+-rw-r--r--   0        0        0      536 2023-05-05 07:11:44.949138 encapsia_api-0.4.6/encapsia_api/tests/test_plugin.py
+-rw-r--r--   0        0        0     9154 2024-04-01 09:01:54.171375 encapsia_api-0.4.6/encapsia_api/tests/test_resilient_request.py
+-rw-r--r--   0        0        0     7067 2024-04-01 09:34:17.498249 encapsia_api-0.4.6/encapsia_api/tests/test_rest.py
+-rw-r--r--   0        0        0      566 2024-04-01 09:01:54.171375 encapsia_api-0.4.6/encapsia_api/util.py
+-rw-r--r--   0        0        0     3509 2024-04-01 09:18:05.279109 encapsia_api-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 encapsia_api-0.4.6/PKG-INFO
```

### Comparing `encapsia_api-0.4.5/LICENSE` & `encapsia_api-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.5/README.md` & `encapsia_api-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.5/encapsia_api/__init__.py` & `encapsia_api-0.4.6/encapsia_api/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #: Keep in sync with git tag and package version in pyproject.toml.
-__version__ = "0.4.5"
+__version__ = "0.4.6"
 
 
 class EncapsiaApiError(RuntimeError):
     def __init__(self, message, payload=None):
         super().__init__(message)
         self.message = message
         self.payload = payload
```

### Comparing `encapsia_api-0.4.5/encapsia_api/analytics.py` & `encapsia_api-0.4.6/encapsia_api/analytics.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.5/encapsia_api/credentials.py` & `encapsia_api-0.4.6/encapsia_api/credentials.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.5/encapsia_api/lib.py` & `encapsia_api-0.4.6/encapsia_api/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,19 +87,19 @@
 
     If target_dir is None then a temporary directory is created.
 
     """
     if target_dir:
         try:
             tar = tarfile.open(filename)
-            tar.extractall(target_dir)
+            tar.extractall(target_dir)  # noqa: S202
             tar.close()
             yield target_dir
         finally:
             if cleanup:
                 shutil.rmtree(target_dir)
     else:
         with make_temp_dir_path(cleanup=cleanup) as directory:
             tar = tarfile.open(filename)
-            tar.extractall(directory)
+            tar.extractall(directory)  # noqa: S202
             tar.close()
             yield directory
```

### Comparing `encapsia_api-0.4.5/encapsia_api/package.py` & `encapsia_api-0.4.6/encapsia_api/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         manifest = tar.extractfile(manifest_name)
         if manifest is None:
             raise ValueError(f"Missing manifest file: {manifest_name}")
         return toml.loads(manifest.read().decode())
 
 
 class PackageMaker:
-
     """Generic maker of packages, intended to be used as a context manager."""
 
     def __init__(self, package_format: str, manifest_fields: dict, temp_dir=None):
         self.manifest = self._seed_manifest(package_format, manifest_fields)
         self.temp_dir = temp_dir
         self.directory = pathlib.Path(tempfile.mkdtemp(dir=temp_dir))
```

### Comparing `encapsia_api-0.4.5/encapsia_api/plugin.py` & `encapsia_api-0.4.6/encapsia_api/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     data = io.BytesIO()
     with tarfile.open(mode="w:gz", fileobj=data) as tar:
         tar.add(directory, arcname=directory.name)
     return data.getvalue()
 
 
 class PluginMaker:
-
     """Generic maker of plugins, intended to be used as a context manager."""
 
     def __init__(self, name, directory=None, **kwargs):
         self.directory = pathlib.Path(directory or tempfile.mkdtemp())
         self._add_manifest(name=name, **kwargs)
 
     def __enter__(self):
```

### Comparing `encapsia_api-0.4.5/encapsia_api/resilient_request.py` & `encapsia_api-0.4.6/encapsia_api/resilient_request.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.5/encapsia_api/rest.py` & `encapsia_api-0.4.6/encapsia_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,24 +343,26 @@
 
     def __init__(self, filename, mime_type):
         self.filename = filename
         self.mime_type = mime_type
 
 
 class Boolean:
-    BOOLEAN_LOOKUP = {
-        "yes": True,
-        "y": True,
-        "t": True,
-        "true": True,
-        "no": False,
-        "n": False,
-        "f": False,
-        "false": False,
-    }
+    BOOLEAN_LOOKUP = frozenset(
+        {
+            "yes": True,
+            "y": True,
+            "t": True,
+            "true": True,
+            "no": False,
+            "n": False,
+            "f": False,
+            "false": False,
+        }
+    )
 
     @classmethod
     def from_str(cls, value):
         try:
             return cls.BOOLEAN_LOOKUP[value.lower()]
         except KeyError as e:
             raise ValueError(f"Cannot convert {value} to boolean.") from e
@@ -377,21 +379,23 @@
             return None
         return "yes" if bool(value) else "no"
 
 
 class CsvResponse:
     """Iterable returned from a task or view when responding with non-downloaded CSV."""
 
-    TYPE_CASTERS = {
-        "json": json.loads,
-        "integer": int,
-        "float": float,
-        "datetime": lambda x: arrow.get(x).datetime,
-        "boolean": Boolean().from_str,
-    }
+    TYPE_CASTERS = frozenset(
+        {
+            "json": json.loads,
+            "integer": int,
+            "float": float,
+            "datetime": lambda x: arrow.get(x).datetime,
+            "boolean": Boolean().from_str,
+        }
+    )
 
     def __init__(self, line_iterable):
         self.reader = csv.reader(line_iterable)
         self.headers, self.type_casters = self._parse_headers()
 
     def _parse_headers(self):
         raw_headers = next(self.reader)
@@ -961,9 +965,8 @@
     DbCtlMixin,
     MiscMixin,
     ConfigMixin,
     UserMixin,
     SystemUserMixin,
     SuperUserMixin,
 ):
-
     """REST API access to an Encapsia server."""
```

### Comparing `encapsia_api-0.4.5/encapsia_api/tests/test_credentials.py` & `encapsia_api-0.4.6/encapsia_api/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.5/encapsia_api/tests/test_package.py` & `encapsia_api-0.4.6/encapsia_api/tests/test_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import tarfile
+import typing
 
 import pytest
 
 from encapsia_api import package
 
 
 class TestMakeValidName:
@@ -29,15 +30,15 @@
     def test_newlines(self):
         assert package._make_valid_name("abc\ndef") == "abcdef"
         assert package._make_valid_name("\n\nabc\ndef") == "abcdef"
         assert package._make_valid_name("\n\nabc\ndef\n") == "abcdef"
 
 
 class TestPackageMaker:
-    MANIFEST_FIELDS = {
+    MANIFEST_FIELDS: typing.ClassVar[typing.Dict[str, typing.Any]] = {
         "type": {"name": "test-type", "format": "1.0", "description": "whatever"},
         "instance": {
             "name": "test instance",
             "description": "",
             "version": "1.2.3",
             "created_by": "fred",
         },
```

### Comparing `encapsia_api-0.4.5/encapsia_api/tests/test_plugin.py` & `encapsia_api-0.4.6/encapsia_api/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.5/encapsia_api/tests/test_resilient_request.py` & `encapsia_api-0.4.6/encapsia_api/tests/test_resilient_request.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.5/encapsia_api/tests/test_rest.py` & `encapsia_api-0.4.6/encapsia_api/tests/test_rest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import collections
+import typing
 import unittest
 import unittest.mock
 
 import requests_mock
 
 from encapsia_api import resilient_request, rest
 
@@ -122,15 +123,15 @@
         api = rest.EncapsiaApi("https://snorri.icethree.com", "token")
         self.assertEqual(api.host, "snorri.icethree.com")
 
 
 class TestResilientRestAPI(unittest.TestCase):
     API_URL = "https://localhost.icethree.com"
     TEST_URL = "https://localhost.icethree.com/v1/whoami"
-    RESPONSE = {
+    RESPONSE: typing.ClassVar[typing.Dict[str, typing.Any]] = {
         "status": "ok",
         "result": {
             "id": 1,
             "name": "Root Superuser",
             "email": "system@root.encapsia.com",
             "capabilities": ["superuser"],
             "expires_at": "2021-09-28T13:24:21.745065+00:00",
```

### Comparing `encapsia_api-0.4.5/encapsia_api/util.py` & `encapsia_api-0.4.6/encapsia_api/util.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.5/pyproject.toml` & `encapsia_api-0.4.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encapsia-api"
-version = "0.4.5"
+version = "0.4.6"
 description = "Client API for talking to an Encapsia system."
 readme = "README.md"
 authors = ["Timothy Corbett-Clark <timothy.corbettclark@gmail.com>"]
 maintainers = ["Petre Mierluțiu <petre.mierlutiu@aixial.com>"]
 license = "MIT"
 keywords = ["encapsia", "eSource", "EDC", "Clinical Trials"]
 homepage = "https://github.com/Encapsia/encapsia-api"
@@ -14,19 +14,19 @@
 requests = {version = ">=2.24",extras = ["security"]}
 toml = ">=0.10"
 arrow = ">=1.2.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.1"
-mypy = "^1.3.0"
+mypy = "^1.9.0"
 requests-mock = "^1.10.0"
-ruff = "^0.0.270"
+ruff = "^0.3.4"
 types-toml = "^0.10.8.6"
-types-requests = "^2.31.0.0"
+types-requests = "^2.31.0.20240311"
 
 
 [build-system]
 requires = ["poetry>=1.0.5"]
 build-backend = "poetry.masonry.api"
 
 [tool.pytest.ini_options]
@@ -40,14 +40,47 @@
 ]
 
 [tool.black]
 line-length = 88
 target_version = ['py38']
 
 [tool.ruff]
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".pytype",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pycache__",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
+]
+
+# Same as Black.
+line-length = 88
+
+# Assume Python 3.8.
+target-version = "py38"
+
+
+[tool.ruff.lint]
 select = [
     "E", "F", "I", "W", "RET", "SIM", "UP", "S", "B", "A", "COM",
     "C90", "C4", "G", "ERA", "PLC",
     # pylint (PL)
     "PLE", "PLR", "PLW",
     # ruff specific rules
     "RUF",
@@ -77,57 +110,26 @@
     "A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W",
     "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "EXE", "FBT",
     "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI",
     "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"
 ]
 unfixable = []
 
-# Exclude a variety of commonly ignored directories.
-exclude = [
-    ".bzr",
-    ".direnv",
-    ".eggs",
-    ".git",
-    ".hg",
-    ".mypy_cache",
-    ".nox",
-    ".pants.d",
-    ".pytype",
-    ".ruff_cache",
-    ".svn",
-    ".tox",
-    ".venv",
-    "__pycache__",
-    "__pypackages__",
-    "_build",
-    "buck-out",
-    "build",
-    "dist",
-    "node_modules",
-    "venv",
-]
-
-# Same as Black.
-line-length = 88
-
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-# Assume Python 3.10.
-target-version = "py38"
-
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # many pylint suggestions are improper for tests
 "encapsia_api/tests/*" = ["PLR", "PLW", "PLC1901"]
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 lines-after-imports = 2
 
 [tool.mypy]
 python_version = "3.8"
 warn_return_any = true
 warn_unused_configs = true
 warn_redundant_casts = true
```

### Comparing `encapsia_api-0.4.5/PKG-INFO` & `encapsia_api-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsia-api
-Version: 0.4.5
+Version: 0.4.6
 Summary: Client API for talking to an Encapsia system.
 Home-page: https://github.com/Encapsia/encapsia-api
 License: MIT
 Keywords: encapsia,eSource,EDC,Clinical Trials
 Author: Timothy Corbett-Clark
 Author-email: timothy.corbettclark@gmail.com
 Maintainer: Petre Mierluțiu
```

