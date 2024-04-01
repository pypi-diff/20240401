# Comparing `tmp/litestar_granian-0.2.5.tar.gz` & `tmp/litestar_granian-0.2.6.tar.gz`

## Comparing `litestar_granian-0.2.5.tar` & `litestar_granian-0.2.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/CONTRIBUTING.rst
--rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/Makefile
--rw-r--r--   0        0        0   143265 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/pdm.lock
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/.github/CODEOWNERS
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/.github/workflows/cd.yaml
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/.github/workflows/docs-preview.yaml
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/.github/workflows/docs.yaml
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/.github/workflows/pr-title.yaml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/docs/Makefile
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/docs/conf.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/docs/contribution-guide.rst
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/docs/fix_missing_references.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/docs/index.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/docs/reference/config.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/docs/reference/plugin.rst
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/docs/usage/index.rst
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/docs/usage/placeholder.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/examples/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/examples/basic.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/examples/index.html
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/examples/structlog.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/litestar_granian/__init__.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/litestar_granian/__metadata__.py
--rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/litestar_granian/cli.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/litestar_granian/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/litestar_granian/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/tests/docker-compose.yml
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/tests/test_cli.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/tests/test_plugin.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/LICENSE
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/README.md
--rw-r--r--   0        0        0     8132 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 litestar_granian-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/Makefile
+-rw-r--r--   0        0        0   143265 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/pdm.lock
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.github/CODEOWNERS
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.github/workflows/cd.yaml
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.github/workflows/docs-preview.yaml
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.github/workflows/docs.yaml
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.github/workflows/pr-title.yaml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/Makefile
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/conf.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/contribution-guide.rst
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/fix_missing_references.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/index.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/reference/config.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/reference/plugin.rst
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/usage/index.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/usage/placeholder.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/examples/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/examples/basic.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/examples/index.html
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/examples/structlog.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/litestar_granian/__init__.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/litestar_granian/__metadata__.py
+-rw-r--r--   0        0        0    13512 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/litestar_granian/cli.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/litestar_granian/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/litestar_granian/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/tests/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/tests/docker-compose.yml
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/tests/test_cli.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/tests/test_plugin.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/LICENSE
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/README.md
+-rw-r--r--   0        0        0     8132 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/PKG-INFO
```

### Comparing `litestar_granian-0.2.5/.pre-commit-config.yaml` & `litestar_granian-0.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/CONTRIBUTING.rst` & `litestar_granian-0.2.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/Makefile` & `litestar_granian-0.2.6/Makefile`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/pdm.lock` & `litestar_granian-0.2.6/pdm.lock`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/.github/workflows/cd.yaml` & `litestar_granian-0.2.6/.github/workflows/cd.yaml`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/.github/workflows/ci.yaml` & `litestar_granian-0.2.6/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/.github/workflows/docs-preview.yaml` & `litestar_granian-0.2.6/.github/workflows/docs-preview.yaml`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/.github/workflows/docs.yaml` & `litestar_granian-0.2.6/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/.github/workflows/publish.yaml` & `litestar_granian-0.2.6/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/docs/Makefile` & `litestar_granian-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/docs/conf.py` & `litestar_granian-0.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/docs/fix_missing_references.py` & `litestar_granian-0.2.6/docs/fix_missing_references.py`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/docs/index.rst` & `litestar_granian-0.2.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/examples/basic.py` & `litestar_granian-0.2.6/examples/basic.py`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/examples/structlog.py` & `litestar_granian-0.2.6/examples/structlog.py`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/litestar_granian/cli.py` & `litestar_granian-0.2.6/litestar_granian/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,15 @@
 
     from granian._loops import loops
     from granian.constants import ThreadModes
     from litestar.cli._utils import console, create_ssl_files, show_app_info
     from litestar.cli.commands.core import _server_lifespan
 
     loops.get("auto")
-    if debug is not None:
+    if debug:
         app.debug = True
         os.environ["LITESTAR_DEBUG"] = "1"
     if pdb:
         os.environ["LITESTAR_PDB"] = "1"
     quiet_console = os.getenv("LITESTAR_QUIET_CONSOLE") or False
     if callable(ctx.obj):
         ctx.obj = ctx.obj()
```

### Comparing `litestar_granian-0.2.5/litestar_granian/plugin.py` & `litestar_granian-0.2.6/litestar_granian/plugin.py`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/tests/test_cli.py` & `litestar_granian-0.2.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/tests/test_plugin.py` & `litestar_granian-0.2.6/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/.gitignore` & `litestar_granian-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/LICENSE` & `litestar_granian-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/README.md` & `litestar_granian-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.5/pyproject.toml` & `litestar_granian-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 dependencies = ["litestar>=2.0.1", "granian>=1.0.0"]
 description = "Granian plugin for Litestar"
 keywords = ["litestar", "granian", "asgi"]
 license = { text = "MIT" }
 name = "litestar-granian"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.2.5"
+version = "0.2.6"
 
 [project.urls]
 Changelog = "https://cofin.github.io/litesatr-granian/latest/changelog"
 Discord = "https://discord.gg/X3FJqy8d2j"
 Documentation = "https://cofin.github.io/litesatr-granian/latest/"
 Homepage = "https://cofin.github.io/litesatr-granian/latest/"
 Issue = "https://github.com/cofin/litestar-granian/issues/"
```

### Comparing `litestar_granian-0.2.5/PKG-INFO` & `litestar_granian-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: litestar-granian
-Version: 0.2.5
+Version: 0.2.6
 Summary: Granian plugin for Litestar
 Project-URL: Changelog, https://cofin.github.io/litesatr-granian/latest/changelog
 Project-URL: Discord, https://discord.gg/X3FJqy8d2j
 Project-URL: Documentation, https://cofin.github.io/litesatr-granian/latest/
 Project-URL: Homepage, https://cofin.github.io/litesatr-granian/latest/
 Project-URL: Issue, https://github.com/cofin/litestar-granian/issues/
 Project-URL: Source, https://github.com/cofin/litestar-granian
```

