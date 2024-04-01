# Comparing `tmp/vupitap-0.0.1.tar.gz` & `tmp/vupitap-0.0.2.tar.gz`

## Comparing `vupitap-0.0.1.tar` & `vupitap-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,6 @@
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 vupitap-0.0.1/.flake8
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 vupitap-0.0.1/Makefile
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 vupitap-0.0.1/requirements-dev.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vupitap-0.0.1/requirements.txt
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 vupitap-0.0.1/vupitap/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vupitap-0.0.1/vupitap/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vupitap-0.0.1/vupitap/notes
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 vupitap-0.0.1/vupitap/vupitap.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 vupitap-0.0.1/vupitap/tests/test_vupitap.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 vupitap-0.0.1/.gitignore
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 vupitap-0.0.1/README.md
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 vupitap-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 vupitap-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 vupitap-0.0.2/vupitap/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 vupitap-0.0.2/vupitap/cli.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 vupitap-0.0.2/.gitignore
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vupitap-0.0.2/README.md
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 vupitap-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 vupitap-0.0.2/PKG-INFO
```

### Comparing `vupitap-0.0.1/.gitignore` & `vupitap-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `vupitap-0.0.1/pyproject.toml` & `vupitap-0.0.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,81 @@
 [project]
 name = "vupitap"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name = "Albertas Gimbutas", email = "albertasgim@gmail.com"},
 ]
-description = "Dict experiment"
+description = "Backward chaining algorithm for common configuration and commandline tasks"
 readme = "README.md"
-requires-python = ">= 3.9"
+requires-python = ">= 3.11"
 classifiers = [
     "Development Status :: 3 - Alpha",
-    "License :: OSI Approved :: GNU Affero General Public License v3",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
 ]
 
+[project.scripts]
+vupitap = "vupitap.vupitap:main"
+
+
+[project.urls]
+homepage = "https://github.com/albertas/vupitap"
+
+[project.optional-dependencies]
+test = [
+    "hatch",
+    "ruff",
+    "mypy",
+    "pip-audit",
+    "deadcode",
+    "pytest",
+    "pytest-cov",
+]
+
+
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
-[tool.hatch.publish.index]
-disable = true
+[tool.hatch.build]
+include = ["**/*.py"]
+exclude = ["tests/**"]
+
+
+[tool.ruff]  # https://docs.astral.sh/ruff/settings/
+line-length = 88
+
+[tool.ruff.lint.flake8-quotes]
+inline-quotes = "single"
+
+[tool.ruff.format]
+quote-style = "single"
+docstring-code-format = true
+
+[tool.ruff.lint]
+select = ["ALL"]
+ignore = [
+    "D203",  # one-blank-line-before-class
+    "D213",  # multi-line-summary-second-line
+    "COM812",  # missing-trailing-comma
+    "ISC001",  # single-line-implicit-string-concatenation
+]
 
 [tool.mypy]
-exclude = ["build", "dist", "venv"]
-python_version = "3.8"
+exclude = ["build", "dist", ".venv", "tests"]
+python_version = "3.11"
+strict = true
 pretty = true
 color_output = true
 show_error_codes = true
 warn_return_any = true
 warn_unused_configs = true
 
-[tool.isort]
-profile = "black"
-multi_line_output = 3
-
-[tool.ruff]  # https://beta.ruff.rs/docs/settings/
-line-length = 120
+[tool.deadcode]
+ignore_names = [
+    "main",
+]
+exclude = ["tests"]
```

