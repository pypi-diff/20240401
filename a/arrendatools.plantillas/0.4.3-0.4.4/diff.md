# Comparing `tmp/arrendatools.plantillas-0.4.3.tar.gz` & `tmp/arrendatools.plantillas-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrendatools.plantillas-0.4.3.tar", last modified: Mon Mar 25 11:01:58 2024, max compression
+gzip compressed data, was "arrendatools.plantillas-0.4.4.tar", last modified: Mon Apr  1 09:42:09 2024, max compression
```

## Comparing `arrendatools.plantillas-0.4.3.tar` & `arrendatools.plantillas-0.4.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 11:01:58.375161 arrendatools.plantillas-0.4.3/
--rw-r--r--   0 root         (0) root         (0)       66 2024-03-25 11:01:51.000000 arrendatools.plantillas-0.4.3/.gitattributes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 11:01:58.371161 arrendatools.plantillas-0.4.3/.github/
--rw-r--r--   0 root         (0) root         (0)      397 2024-03-25 11:01:51.000000 arrendatools.plantillas-0.4.3/.github/dependabot.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 11:01:58.371161 arrendatools.plantillas-0.4.3/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1951 2024-03-25 11:01:51.000000 arrendatools.plantillas-0.4.3/.github/workflows/main.yml
--rw-r--r--   0 root         (0) root         (0)      867 2024-03-25 11:01:51.000000 arrendatools.plantillas-0.4.3/.github/workflows/test.yml
--rw-r--r--   0 root         (0) root         (0)     2788 2024-03-25 11:01:51.000000 arrendatools.plantillas-0.4.3/.gitignore
--rw-r--r--   0 root         (0) root         (0)    26908 2024-03-25 11:01:52.000000 arrendatools.plantillas-0.4.3/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1062 2024-03-25 11:01:51.000000 arrendatools.plantillas-0.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2092 2024-03-25 11:01:58.375161 arrendatools.plantillas-0.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1200 2024-03-25 11:01:51.000000 arrendatools.plantillas-0.4.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 11:01:58.371161 arrendatools.plantillas-0.4.3/arrendatools/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-25 11:01:52.000000 arrendatools.plantillas-0.4.3/arrendatools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 11:01:58.371161 arrendatools.plantillas-0.4.3/arrendatools/plantillas/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 11:01:51.000000 arrendatools.plantillas-0.4.3/arrendatools/plantillas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 11:01:58.371161 arrendatools.plantillas-0.4.3/arrendatools/plantillas/filters/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 11:01:51.000000 arrendatools.plantillas-0.4.3/arrendatools/plantillas/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4769 2024-03-25 11:01:51.000000 arrendatools.plantillas-0.4.3/arrendatools/plantillas/filters/fechas.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-03-25 11:01:51.000000 arrendatools.plantillas-0.4.3/arrendatools/plantillas/filters/numeros.py
--rw-r--r--   0 root         (0) root         (0)     1381 2024-03-25 11:01:51.000000 arrendatools.plantillas-0.4.3/arrendatools/plantillas/plantilla.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 11:01:58.375161 arrendatools.plantillas-0.4.3/arrendatools.plantillas.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2092 2024-03-25 11:01:58.000000 arrendatools.plantillas-0.4.3/arrendatools.plantillas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      676 2024-03-25 11:01:58.000000 arrendatools.plantillas-0.4.3/arrendatools.plantillas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 11:01:58.000000 arrendatools.plantillas-0.4.3/arrendatools.plantillas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2024-03-25 11:01:58.000000 arrendatools.plantillas-0.4.3/arrendatools.plantillas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-03-25 11:01:58.000000 arrendatools.plantillas-0.4.3/arrendatools.plantillas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1533 2024-03-25 11:01:52.000000 arrendatools.plantillas-0.4.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       61 2024-03-25 11:01:51.000000 arrendatools.plantillas-0.4.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-25 11:01:58.375161 arrendatools.plantillas-0.4.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 11:01:58.371161 arrendatools.plantillas-0.4.3/test/
--rw-r--r--   0 root         (0) root         (0)     2491 2024-03-25 11:01:51.000000 arrendatools.plantillas-0.4.3/test/test_fechas.py
--rw-r--r--   0 root         (0) root         (0)     1149 2024-03-25 11:01:51.000000 arrendatools.plantillas-0.4.3/test/test_numeros.py
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-25 11:01:51.000000 arrendatools.plantillas-0.4.3/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:42:09.739726 arrendatools.plantillas-0.4.4/
+-rw-r--r--   0 root         (0) root         (0)       66 2024-04-01 09:42:02.000000 arrendatools.plantillas-0.4.4/.gitattributes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:42:09.735726 arrendatools.plantillas-0.4.4/.github/
+-rw-r--r--   0 root         (0) root         (0)      397 2024-04-01 09:42:02.000000 arrendatools.plantillas-0.4.4/.github/dependabot.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:42:09.735726 arrendatools.plantillas-0.4.4/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-04-01 09:42:02.000000 arrendatools.plantillas-0.4.4/.github/workflows/main.yml
+-rw-r--r--   0 root         (0) root         (0)      867 2024-04-01 09:42:02.000000 arrendatools.plantillas-0.4.4/.github/workflows/test.yml
+-rw-r--r--   0 root         (0) root         (0)     2788 2024-04-01 09:42:02.000000 arrendatools.plantillas-0.4.4/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    28505 2024-04-01 09:42:03.000000 arrendatools.plantillas-0.4.4/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-04-01 09:42:02.000000 arrendatools.plantillas-0.4.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2092 2024-04-01 09:42:09.739726 arrendatools.plantillas-0.4.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-04-01 09:42:02.000000 arrendatools.plantillas-0.4.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:42:09.735726 arrendatools.plantillas-0.4.4/arrendatools/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-01 09:42:03.000000 arrendatools.plantillas-0.4.4/arrendatools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:42:09.739726 arrendatools.plantillas-0.4.4/arrendatools/plantillas/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 09:42:02.000000 arrendatools.plantillas-0.4.4/arrendatools/plantillas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:42:09.739726 arrendatools.plantillas-0.4.4/arrendatools/plantillas/filters/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 09:42:02.000000 arrendatools.plantillas-0.4.4/arrendatools/plantillas/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2024-04-01 09:42:02.000000 arrendatools.plantillas-0.4.4/arrendatools/plantillas/filters/fechas.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2024-04-01 09:42:02.000000 arrendatools.plantillas-0.4.4/arrendatools/plantillas/filters/numeros.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2024-04-01 09:42:02.000000 arrendatools.plantillas-0.4.4/arrendatools/plantillas/plantilla.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:42:09.739726 arrendatools.plantillas-0.4.4/arrendatools.plantillas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2092 2024-04-01 09:42:09.000000 arrendatools.plantillas-0.4.4/arrendatools.plantillas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      676 2024-04-01 09:42:09.000000 arrendatools.plantillas-0.4.4/arrendatools.plantillas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 09:42:09.000000 arrendatools.plantillas-0.4.4/arrendatools.plantillas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2024-04-01 09:42:09.000000 arrendatools.plantillas-0.4.4/arrendatools.plantillas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-01 09:42:09.000000 arrendatools.plantillas-0.4.4/arrendatools.plantillas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1533 2024-04-01 09:42:03.000000 arrendatools.plantillas-0.4.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-01 09:42:02.000000 arrendatools.plantillas-0.4.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-01 09:42:09.739726 arrendatools.plantillas-0.4.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:42:09.739726 arrendatools.plantillas-0.4.4/test/
+-rw-r--r--   0 root         (0) root         (0)     2491 2024-04-01 09:42:02.000000 arrendatools.plantillas-0.4.4/test/test_fechas.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-01 09:42:02.000000 arrendatools.plantillas-0.4.4/test/test_numeros.py
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-01 09:42:02.000000 arrendatools.plantillas-0.4.4/tox.ini
```

### Comparing `arrendatools.plantillas-0.4.3/.github/workflows/main.yml` & `arrendatools.plantillas-0.4.4/.github/workflows/main.yml`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
       id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing in PyPi
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - name: Python Semantic Release
       id: release
-      uses: python-semantic-release/python-semantic-release@v9.3.1
+      uses: python-semantic-release/python-semantic-release@v9.4.0
       with:
         github_token: ${{ secrets.GITHUB_TOKEN }}
     - name: Publish package distributions to PyPI
       id: pypi-publish
       uses: pypa/gh-action-pypi-publish@release/v1
       # NOTE: DO NOT wrap the conditional in ${{ }} as it will always evaluate to true.
       # See https://github.com/actions/runner/issues/1173
```

### Comparing `arrendatools.plantillas-0.4.3/.github/workflows/test.yml` & `arrendatools.plantillas-0.4.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.4.3/.gitignore` & `arrendatools.plantillas-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.4.3/CHANGELOG.md` & `arrendatools.plantillas-0.4.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,46 @@
 # CHANGELOG
 
 
 
+## v0.4.4 (2024-04-01)
+
+### Build
+
+* build(deps): bump python-semantic-release/python-semantic-release
+
+Bumps [python-semantic-release/python-semantic-release](https://github.com/python-semantic-release/python-semantic-release) from 9.3.1 to 9.4.0.
+- [Release notes](https://github.com/python-semantic-release/python-semantic-release/releases)
+- [Changelog](https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md)
+- [Commits](https://github.com/python-semantic-release/python-semantic-release/compare/v9.3.1...v9.4.0)
+
+---
+updated-dependencies:
+- dependency-name: python-semantic-release/python-semantic-release
+  dependency-type: direct:production
+  update-type: version-update:semver-minor
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`7e11916`](https://github.com/hokus15/ArrendaToolsPlantillas/commit/7e119164e6752d115793f9c2a96607d025a87406))
+
+### Fix
+
+* fix(autoescape): undo XSS mitigation ([`11c1add`](https://github.com/hokus15/ArrendaToolsPlantillas/commit/11c1addb51271880d341dedc9402dda899d1ab79))
+
+### Unknown
+
+* Merge pull request #37 from hokus15/devel
+
+fix(autoescape): undo XSS mitigation ([`7b17b04`](https://github.com/hokus15/ArrendaToolsPlantillas/commit/7b17b043768ebbdba18e2325de13d39f752c14a9))
+
+* Merge pull request #36 from hokus15/dependabot/github_actions/python-semantic-release/python-semantic-release-9.4.0
+
+build(deps): bump python-semantic-release/python-semantic-release from 9.3.1 to 9.4.0 ([`359c846`](https://github.com/hokus15/ArrendaToolsPlantillas/commit/359c846173a165f1a9667e901622a2fc14899556))
+
+
 ## v0.4.3 (2024-03-25)
 
 ### Build
 
 * build(deps): bump python-semantic-release/python-semantic-release
 
 Bumps [python-semantic-release/python-semantic-release](https://github.com/python-semantic-release/python-semantic-release) from 9.3.0 to 9.3.1.
```

### Comparing `arrendatools.plantillas-0.4.3/LICENSE` & `arrendatools.plantillas-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.4.3/PKG-INFO` & `arrendatools.plantillas-0.4.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrendatools.plantillas
-Version: 0.4.3
+Version: 0.4.4
 Summary: Módulo de Python que aplica plantillas jinja. Además inlcuye filtros que pueden ser útiles para la generación de recibos de alquiler, facturas, informes,...
 Author-email: Jordi Morell <hokus@hotmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `arrendatools.plantillas-0.4.3/README.md` & `arrendatools.plantillas-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.4.3/arrendatools/plantillas/filters/fechas.py` & `arrendatools.plantillas-0.4.4/arrendatools/plantillas/filters/fechas.py`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.4.3/arrendatools/plantillas/filters/numeros.py` & `arrendatools.plantillas-0.4.4/arrendatools/plantillas/filters/numeros.py`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.4.3/arrendatools/plantillas/plantilla.py` & `arrendatools.plantillas-0.4.4/arrendatools/plantillas/plantilla.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,23 @@
     "dias_entre": dias_entre
 }
 
 custom_filters = {**custom_functions}
 
 
 def aplicar_plantilla(directorio_plantillas, plantilla, datos):
-    environment = Environment(loader=FileSystemLoader(directorio_plantillas), autoescape=True)
+    environment = Environment(loader=FileSystemLoader(directorio_plantillas), autoescape=False)
     environment.filters.update(custom_filters)
     environment.globals.update(custom_functions)
     template = environment.get_template(plantilla)
     return template.render(datos)
 
 
 def aplicar_plantilla_texto(texto_plantilla, datos):
     try:
-        environment = Environment(loader=BaseLoader, autoescape=True)
+        environment = Environment(loader=BaseLoader, autoescape=False)
         environment.filters.update(custom_filters)
         environment.globals.update(custom_functions)
         template = environment.from_string(texto_plantilla)
         return template.render(datos)
     except Exception as e:
         return str(e)
```

### Comparing `arrendatools.plantillas-0.4.3/arrendatools.plantillas.egg-info/PKG-INFO` & `arrendatools.plantillas-0.4.4/arrendatools.plantillas.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrendatools.plantillas
-Version: 0.4.3
+Version: 0.4.4
 Summary: Módulo de Python que aplica plantillas jinja. Además inlcuye filtros que pueden ser útiles para la generación de recibos de alquiler, facturas, informes,...
 Author-email: Jordi Morell <hokus@hotmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `arrendatools.plantillas-0.4.3/arrendatools.plantillas.egg-info/SOURCES.txt` & `arrendatools.plantillas-0.4.4/arrendatools.plantillas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.4.3/pyproject.toml` & `arrendatools.plantillas-0.4.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arrendatools.plantillas"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
     {name = "Jordi Morell", email = "hokus@hotmail.com"},
 ]
 description = "Módulo de Python que aplica plantillas jinja. Además inlcuye filtros que pueden ser útiles para la generación de recibos de alquiler, facturas, informes,..."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT"}
```

### Comparing `arrendatools.plantillas-0.4.3/test/test_fechas.py` & `arrendatools.plantillas-0.4.4/test/test_fechas.py`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.4.3/test/test_numeros.py` & `arrendatools.plantillas-0.4.4/test/test_numeros.py`

 * *Files identical despite different names*

