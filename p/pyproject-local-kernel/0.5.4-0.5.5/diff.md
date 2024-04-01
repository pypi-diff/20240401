# Comparing `tmp/pyproject_local_kernel-0.5.4.tar.gz` & `tmp/pyproject_local_kernel-0.5.5.tar.gz`

## Comparing `pyproject_local_kernel-0.5.4.tar` & `pyproject_local_kernel-0.5.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/.python-version
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/CHANGELOG.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/FAQ.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/data/kernel.json
--rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/src/pyproject_local_kernel/__init__.py
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/src/pyproject_local_kernel/__main__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/tests/test_identify.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/tests/identify/broken/pyproject.toml
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/tests/identify/custom/pyproject.toml
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/tests/identify/custom_broken/pyproject.toml
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/tests/identify/hatch/pyproject.toml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/tests/identify/pdm/pyproject.toml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/tests/identify/poetry/pyproject.toml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/tests/identify/rye/pyproject.toml
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/tests/identify/unknown/pyproject.toml
--rwxr-xr-x   0        0        0      391 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/tests/server-client/setup_run.sh
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/tests/server-client/client/notebook.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/tests/server-client/client/pyproject.toml
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/tests/server-client/client/requirements-dev.lock
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/tests/server-client/client/requirements.lock
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/tests/server-client/server/pyproject.toml
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/tests/server-client/server/requirements-dev.lock
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/tests/server-client/server/requirements.lock
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/LICENSE.md
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/README.md
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/.python-version
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/CHANGELOG.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/FAQ.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/data/kernel.json
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/src/pyproject_local_kernel/__init__.py
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/src/pyproject_local_kernel/__main__.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/tests/test_identify.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/tests/identify/broken/pyproject.toml
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/tests/identify/custom/pyproject.toml
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/tests/identify/custom_broken/pyproject.toml
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/tests/identify/hatch/pyproject.toml
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/tests/identify/pdm/pyproject.toml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/tests/identify/poetry/pyproject.toml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/tests/identify/rye/pyproject.toml
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/tests/identify/unknown/pyproject.toml
+-rwxr-xr-x   0        0        0      391 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/tests/server-client/setup_run.sh
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/tests/server-client/client/notebook.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/tests/server-client/client/pyproject.toml
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/tests/server-client/client/requirements-dev.lock
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/tests/server-client/client/requirements.lock
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/tests/server-client/server/pyproject.toml
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/tests/server-client/server/requirements-dev.lock
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/tests/server-client/server/requirements.lock
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/LICENSE.md
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/README.md
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 pyproject_local_kernel-0.5.5/PKG-INFO
```

### Comparing `pyproject_local_kernel-0.5.4/CHANGELOG.md` & `pyproject_local_kernel-0.5.5/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 0.5.5
+
+- Fix ProjectDetection.path which should hold the path to the pyproject file
+- Added trusted publishing (for PyPI) workflow on github
+
 ## 0.5.4
 
 - Enable debugging for the Pyproject Local kernel (just like the regular
 ipykernel)
 - More extensive tests, on linux and windows, including notebook execution
 
 ## 0.5.3
```

### Comparing `pyproject_local_kernel-0.5.4/FAQ.md` & `pyproject_local_kernel-0.5.5/FAQ.md`

 * *Files identical despite different names*

### Comparing `pyproject_local_kernel-0.5.4/src/pyproject_local_kernel/__init__.py` & `pyproject_local_kernel-0.5.5/src/pyproject_local_kernel/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 from dataclasses import dataclass
 import enum
 import logging
 import sys
 from pathlib import Path
-import typing
+import typing as t
 
 try:
     import tomllib as tomli
 except ImportError:
     import tomli as tomli
 
 
@@ -61,17 +61,18 @@
         if self == ProjectKind.Hatch:
             return ['hatch', 'run', 'python']
         return None
 
 
 @dataclass
 class ProjectDetection:
-    path: Path
+    # pyproject.toml file path
+    path: t.Optional[Path]
     kind: ProjectKind
-    python_cmd: typing.Optional[typing.List[str]] = None
+    python_cmd: t.Optional[t.List[str]] = None
 
     def get_python_cmd(self):
         if self.python_cmd is not None:
             return self.python_cmd
         return self.kind.python_cmd() or DEFAULT_RYE_RUN_CMD
 
 
@@ -152,11 +153,11 @@
         try:
             with open(pyproj, "rb") as tf:
                 toml_structure = tomli.load(tf)
                 identity, extra_vars = _identify_toml(toml_structure)
         except (IOError, tomli.TOMLDecodeError) as exc:
             print("Error: ", exc, file=sys.stderr)
             kind = ProjectKind.InvalidData
-            return ProjectDetection(file, kind)
+            return ProjectDetection(pyproj, kind)
 
-    return ProjectDetection(file, identity, **extra_vars)
+    return ProjectDetection(pyproj, identity, **extra_vars)
```

### Comparing `pyproject_local_kernel-0.5.4/src/pyproject_local_kernel/__main__.py` & `pyproject_local_kernel-0.5.5/src/pyproject_local_kernel/__main__.py`

 * *Files identical despite different names*

### Comparing `pyproject_local_kernel-0.5.4/tests/identify/hatch/pyproject.toml` & `pyproject_local_kernel-0.5.5/tests/identify/hatch/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject_local_kernel-0.5.4/tests/server-client/client/requirements-dev.lock` & `pyproject_local_kernel-0.5.5/tests/server-client/client/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `pyproject_local_kernel-0.5.4/tests/server-client/client/requirements.lock` & `pyproject_local_kernel-0.5.5/tests/server-client/client/requirements.lock`

 * *Files identical despite different names*

### Comparing `pyproject_local_kernel-0.5.4/tests/server-client/server/requirements-dev.lock` & `pyproject_local_kernel-0.5.5/tests/server-client/server/requirements-dev.lock`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     # via nbclient
     # via papermill
 packaging==24.0
     # via jupytext
 papermill==2.5.0
 platformdirs==4.2.0
     # via jupyter-core
-pyproject-local-kernel @ file:///${PROJECT_ROOT}/../../../../pyproject-local-kernel
+pyproject-local-kernel @ file:///${PROJECT_ROOT}/../../..
 python-dateutil==2.9.0.post0
     # via jupyter-client
 pyyaml==6.0.1
     # via jupytext
     # via papermill
 pyzmq==25.1.2
     # via jupyter-client
```

### Comparing `pyproject_local_kernel-0.5.4/tests/server-client/server/requirements.lock` & `pyproject_local_kernel-0.5.5/tests/server-client/server/requirements.lock`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     # via nbclient
     # via papermill
 packaging==24.0
     # via jupytext
 papermill==2.5.0
 platformdirs==4.2.0
     # via jupyter-core
-pyproject-local-kernel @ file:///${PROJECT_ROOT}/../../../../pyproject-local-kernel
+pyproject-local-kernel @ file:///${PROJECT_ROOT}/../../..
 python-dateutil==2.9.0.post0
     # via jupyter-client
 pyyaml==6.0.1
     # via jupytext
     # via papermill
 pyzmq==25.1.2
     # via jupyter-client
```

### Comparing `pyproject_local_kernel-0.5.4/LICENSE.md` & `pyproject_local_kernel-0.5.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyproject_local_kernel-0.5.4/README.md` & `pyproject_local_kernel-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_local_kernel-0.5.4/pyproject.toml` & `pyproject_local_kernel-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyproject-local-kernel"
-version = "0.5.4"
+version = "0.5.5"
 description = "Python Jupyter kernel using pyproject environment manangers like Rye, PDM, Poetry, Hatch etc."
 authors = [
     { name = "Ulrik Sverdrup", email = "ulrik.sverdrup@gmail.com" }
 ]
 dependencies = [
     "tomli>=2.0.1; python_version < '3.11'",
 ]
```

### Comparing `pyproject_local_kernel-0.5.4/PKG-INFO` & `pyproject_local_kernel-0.5.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyproject-local-kernel
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python Jupyter kernel using pyproject environment manangers like Rye, PDM, Poetry, Hatch etc.
 Project-URL: Repository, https://github.com/bluss/pyproject-local-kernel
 Author-email: Ulrik Sverdrup <ulrik.sverdrup@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.md
 Keywords: Interactive,Interpreter,Jupyter,Pyproject
 Classifier: Framework :: Jupyter
```

