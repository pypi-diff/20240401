# Comparing `tmp/pytest-cython-0.2.2.tar.gz` & `tmp/pytest-cython-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-cython-0.2.2.tar", last modified: Sat Mar 30 06:18:28 2024, max compression
+gzip compressed data, was "pytest-cython-0.3.0.tar", last modified: Mon Apr  1 10:58:02 2024, max compression
```

## Comparing `pytest-cython-0.2.2.tar` & `pytest-cython-0.3.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:18:28.027450 pytest-cython-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-03-30 06:18:28.027450 pytest-cython-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:18:28.023450 pytest-cython-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-30 06:18:28.027450 pytest-cython-0.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1585 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:18:28.023450 pytest-cython-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:18:28.023450 pytest-cython-0.2.2/src/pytest_cython/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/src/pytest_cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/src/pytest_cython/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:18:28.027450 pytest-cython-0.2.2/src/pytest_cython.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-03-30 06:18:28.000000 pytest-cython-0.2.2/src/pytest_cython.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-30 06:18:28.000000 pytest-cython-0.2.2/src/pytest_cython.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 06:18:28.000000 pytest-cython-0.2.2/src/pytest_cython.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-30 06:18:28.000000 pytest-cython-0.2.2/src/pytest_cython.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 06:18:27.000000 pytest-cython-0.2.2/src/pytest_cython.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-30 06:18:28.000000 pytest-cython-0.2.2/src/pytest_cython.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-30 06:18:28.000000 pytest-cython-0.2.2/src/pytest_cython.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:18:28.027450 pytest-cython-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:18:28.027450 pytest-cython-0.2.2/tests/example-project/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/tests/example-project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/tests/example-project/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:18:28.023450 pytest-cython-0.2.2/tests/example-project/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:18:28.027450 pytest-cython-0.2.2/tests/example-project/src/clib/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/tests/example-project/src/clib/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/tests/example-project/src/clib/sqrc.c
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/tests/example-project/src/clib/sqrcpp.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:18:28.027450 pytest-cython-0.2.2/tests/example-project/src/pypackage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/tests/example-project/src/pypackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/tests/example-project/src/pypackage/cython_ext_module.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/tests/example-project/src/pypackage/cython_ext_module.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/tests/example-project/src/pypackage/pure_py_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/tests/example-project/src/pypackage/wrap_c_ext_module.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/tests/example-project/src/pypackage/wrap_cpp_ext_module.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-03-30 06:18:18.000000 pytest-cython-0.2.2/tests/test_pytest_cython.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.660092 pytest-cython-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-01 10:58:02.660092 pytest-cython-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.656092 pytest-cython-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-01 10:58:02.660092 pytest-cython-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1580 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.652092 pytest-cython-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.656092 pytest-cython-0.3.0/src/pytest_cython/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/src/pytest_cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/src/pytest_cython/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.656092 pytest-cython-0.3.0/src/pytest_cython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-01 10:58:02.000000 pytest-cython-0.3.0/src/pytest_cython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-01 10:58:02.000000 pytest-cython-0.3.0/src/pytest_cython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 10:58:02.000000 pytest-cython-0.3.0/src/pytest_cython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 10:58:02.000000 pytest-cython-0.3.0/src/pytest_cython.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 10:58:02.000000 pytest-cython-0.3.0/src/pytest_cython.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 10:58:02.000000 pytest-cython-0.3.0/src/pytest_cython.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 10:58:02.000000 pytest-cython-0.3.0/src/pytest_cython.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.656092 pytest-cython-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.656092 pytest-cython-0.3.0/tests/example-project/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.652092 pytest-cython-0.3.0/tests/example-project/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.656092 pytest-cython-0.3.0/tests/example-project/src/clib/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/clib/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/clib/sqrc.c
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/clib/sqrcpp.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.656092 pytest-cython-0.3.0/tests/example-project/src/pypackage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/pypackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/pypackage/cython_ext_module.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/pypackage/cython_ext_module.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/pypackage/pure_py_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/pypackage/wrap_c_ext_module.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/pypackage/wrap_cpp_ext_module.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/test_pytest_cython.py
```

### Comparing `pytest-cython-0.2.2/CHANGELOG.md` & `pytest-cython-0.3.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pytest-cython-0.2.2/CODE_OF_CONDUCT.md` & `pytest-cython-0.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pytest-cython-0.2.2/CONTRIBUTING.md` & `pytest-cython-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pytest-cython-0.2.2/LICENSE.md` & `pytest-cython-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pytest-cython-0.2.2/PKG-INFO` & `pytest-cython-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-cython
-Version: 0.2.2
+Version: 0.3.0
 Summary: A plugin for testing Cython extension modules
 Home-page: https://github.com/lgpage/pytest-cython
 Author: Logan Page
 Author-email: page.lg@gmail.com
 License: MIT
 Keywords: pytest,py.test,cython,doctest
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: pytest<8,>=4.6
+Requires-Dist: pytest>=8
 
 # Overview
 
 [![PyPI Package latest release](https://img.shields.io/pypi/v/pytest-cython.svg?style=flat)](https://pypi.org/project/pytest-cython)
 [![PyPI Package monthly downloads](https://img.shields.io/pypi/dm/pytest-cython.svg?style=flat)](https://pypi.org/project/pytest-cython)
 [![PyPI Wheel](https://img.shields.io/pypi/wheel/pytest-cython.svg?style=flat)](https://pypi.org/project/pytest-cython)
 [![Supported versions](https://img.shields.io/pypi/pyversions/pytest-cython.svg?style=flat)](https://pypi.org/project/pytest-cython)
@@ -67,14 +67,15 @@
 ## Compatibility
 
 The following table describes the versions of Pytest and Cython the each version of the pytest-cython plugin is
 compatible with.
 
 | Version | Pytest | Cython  |
 | ------- | ------ | ------- |
+| 0.3.x   | 8      | 0.29, 3 |
 | 0.2.x   | 6, 7   | 0.29, 3 |
 
 ## Issues
 
 If you encounter any problems, please [file an issue](https://github.com/lgpage/pytest-cython/issues) along with a
 detailed description.
```

### Comparing `pytest-cython-0.2.2/README.md` & `pytest-cython-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 ## Compatibility
 
 The following table describes the versions of Pytest and Cython the each version of the pytest-cython plugin is
 compatible with.
 
 | Version | Pytest | Cython  |
 | ------- | ------ | ------- |
+| 0.3.x   | 8      | 0.29, 3 |
 | 0.2.x   | 6, 7   | 0.29, 3 |
 
 ## Issues
 
 If you encounter any problems, please [file an issue](https://github.com/lgpage/pytest-cython/issues) along with a
 detailed description.
```

### Comparing `pytest-cython-0.2.2/docs/conf.py` & `pytest-cython-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-cython-0.2.2/noxfile.py` & `pytest-cython-0.3.0/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     session.run("check-manifest")
     session.run("python", "-m", "build")
     session.run("twine", "check", "dist/*.*")
 
 
 @nox.session
 @nox.parametrize('python', ["3.10", "3.11", "3.12"])
-@nox.parametrize('pytest', ["6", "7"])
+@nox.parametrize('pytest', ["8"])
 @nox.parametrize('cython', ["0.29", "3"])
 def test(session, pytest, cython):
     session.install("--upgrade", "setuptools")
 
     session.install(f"pytest=={pytest}.*")
     session.install(f"cython=={cython}.*")
     session.install("-e", ".")
```

### Comparing `pytest-cython-0.2.2/setup.cfg` & `pytest-cython-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-cython-0.2.2/setup.py` & `pytest-cython-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 with open(path.join(this_directory, 'README.md')) as readme_file:
     long_description = readme_file.read()
 
 
 setup(
     name='pytest-cython',
-    version='0.2.2',
+    version='0.3.0',
     description='A plugin for testing Cython extension modules',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Logan Page',
     author_email='page.lg@gmail.com',
     license='MIT',
     url='https://github.com/lgpage/pytest-cython',
@@ -40,15 +40,15 @@
         'Topic :: Software Development :: Testing',
         'Topic :: Utilities',
     ],
     keywords=[
         'pytest', 'py.test', 'cython', 'doctest',
     ],
     install_requires=[
-        'pytest>=4.6,<8',
+        'pytest>=8',
     ],
     entry_points={
         'pytest11': [
             'pytest_cython = pytest_cython.plugin',
         ],
     },
 )
```

### Comparing `pytest-cython-0.2.2/src/pytest_cython.egg-info/PKG-INFO` & `pytest-cython-0.3.0/src/pytest_cython.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-cython
-Version: 0.2.2
+Version: 0.3.0
 Summary: A plugin for testing Cython extension modules
 Home-page: https://github.com/lgpage/pytest-cython
 Author: Logan Page
 Author-email: page.lg@gmail.com
 License: MIT
 Keywords: pytest,py.test,cython,doctest
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: pytest<8,>=4.6
+Requires-Dist: pytest>=8
 
 # Overview
 
 [![PyPI Package latest release](https://img.shields.io/pypi/v/pytest-cython.svg?style=flat)](https://pypi.org/project/pytest-cython)
 [![PyPI Package monthly downloads](https://img.shields.io/pypi/dm/pytest-cython.svg?style=flat)](https://pypi.org/project/pytest-cython)
 [![PyPI Wheel](https://img.shields.io/pypi/wheel/pytest-cython.svg?style=flat)](https://pypi.org/project/pytest-cython)
 [![Supported versions](https://img.shields.io/pypi/pyversions/pytest-cython.svg?style=flat)](https://pypi.org/project/pytest-cython)
@@ -67,14 +67,15 @@
 ## Compatibility
 
 The following table describes the versions of Pytest and Cython the each version of the pytest-cython plugin is
 compatible with.
 
 | Version | Pytest | Cython  |
 | ------- | ------ | ------- |
+| 0.3.x   | 8      | 0.29, 3 |
 | 0.2.x   | 6, 7   | 0.29, 3 |
 
 ## Issues
 
 If you encounter any problems, please [file an issue](https://github.com/lgpage/pytest-cython/issues) along with a
 detailed description.
```

### Comparing `pytest-cython-0.2.2/src/pytest_cython.egg-info/SOURCES.txt` & `pytest-cython-0.3.0/src/pytest_cython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-cython-0.2.2/tests/example-project/setup.py` & `pytest-cython-0.3.0/tests/example-project/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 
     extensions = [
         Extension('*', ['src/pypackage/*.pyx'])
     ]
 
     setup(
         name='pytest-cython',
-        version='0.2.2',
+        version='0.3.0',
         description="Example Cython project for pytest-cython tests",
         package_dir={'': 'src'},
         packages=['pypackage'],
         zip_safe=False,
         ext_modules=cythonize(extensions, compiler_directives=directives)
     )
```

### Comparing `pytest-cython-0.2.2/tests/example-project/src/pypackage/cython_ext_module.pyx` & `pytest-cython-0.3.0/tests/example-project/src/pypackage/cython_ext_module.pyx`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 cdef int cfoo(int a, int b) except? -1:
     """
     >>> cfoo(1, 1)
     2
     """
     return a + b
 
-cdef int cbar(int a, int b) nogil except? -1:
+cdef int cbar(int a, int b) except? -1 nogil:
     """
     >>> cbar(1, 1)
     2
     """
     return a + b
 
-cdef inline int cspam(int a, int b) nogil except? -1:
+cdef inline int cspam(int a, int b) except? -1 nogil:
     """
     >>> cspam(1, 1)
     2
     """
     return (a + b)
 
 
@@ -38,23 +38,23 @@
         """
         >>> eggs = Eggs(1, 1)
         >>> eggs.foo()
         2
         """
         return self.a + self.b
 
-    cdef int bar(Eggs self) nogil except? -1:
+    cdef int bar(Eggs self) except? -1 nogil:
         """
         >>> eggs = Eggs(1, 1)
         >>> eggs.bar()
         2
         """
         return self.a + self.b
 
-    cdef int spam(Eggs self) nogil except? -1:
+    cdef int spam(Eggs self) except? -1 nogil:
         """
         >>> eggs = Eggs(1, 1)
         >>> eggs.spam()
         2
         """
         return cspam(self.a, self.b)
```

### Comparing `pytest-cython-0.2.2/tests/test_pytest_cython.py` & `pytest-cython-0.3.0/tests/test_pytest_cython.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,33 +2,31 @@
 
 import pathlib
 import pytest
 import shutil
 
 from setuptools.sandbox import run_setup
 
+# import pytest_cython as a quite check to ensure it was installed before running tests
 import pytest_cython.plugin
 
 
 ROOT_PATH = pathlib.Path(__file__).parent
 PROJECT_PATH = ROOT_PATH.joinpath('example-project')
 PACKAGE_PATH = PROJECT_PATH.joinpath('src', 'pypackage')
 
-PYTEST_MAJOR_VERSION = int(pytest.__version__.split('.')[0])
-IMPORT_MODES = ['prepend', 'append']
-if PYTEST_MAJOR_VERSION >= 6:
-    IMPORT_MODES.insert(0, 'importlib')
+IMPORT_MODES = ["append", "prepend", "importlib"]
 
 
-def get_module(basename, suffix='.pyx'):
+def get_module(basename: str, suffix='.pyx') -> pathlib.Path:
     return PACKAGE_PATH.joinpath(basename + suffix)
 
 
-def run_pytest(testdir, module, import_mode):
-    return testdir.runpytest('-vv', '--doctest-cython', '--import-mode', import_mode, str(module))
+def run_pytest(pytester: pytest.Pytester, module: pathlib.Path, import_mode) -> pytest.RunResult:
+    return pytester.runpytest('-vv', '--doctest-cython', '--import-mode', import_mode, str(module))
 
 
 @pytest.fixture(scope='module', autouse=True)
 def build_example_project():
     shutil.rmtree(PROJECT_PATH.joinpath('build'), True)
     shutil.rmtree(PACKAGE_PATH.joinpath('__pycache__'), True)
 
@@ -39,21 +37,21 @@
         file.unlink()
 
     setup_py = PROJECT_PATH.joinpath('setup.py')
     run_setup(str(setup_py), ['build_ext', '--inplace'])
 
 
 @pytest.mark.parametrize('import_mode', IMPORT_MODES)
-def test_cython_ext_module(testdir, import_mode):
+def test_cython_ext_module(pytester, import_mode):
     module = get_module('cython_ext_module')
     assert module.exists()
 
-    result = run_pytest(testdir, module, import_mode)
+    result = run_pytest(pytester, module, import_mode)
     result.stdout.fnmatch_lines([
-        "*Eggs.__init__ *PASSED*",
+        "*Eggs.__init__*PASSED*",
         "*Eggs.blarg*PASSED*",
         "*Eggs.failing_test*FAILED*",
         "*Eggs.fubar*PASSED*",
         "*",
         "*FAILURES*",
         "*pypackage.cython_ext_module.Eggs.failing_test*",
         "078*",
@@ -64,42 +62,42 @@
         "Got:*",
         "    True*"
     ])
     assert result.ret == 1
 
 
 @pytest.mark.parametrize('import_mode', IMPORT_MODES)
-def test_wrap_c_ext_module(testdir, import_mode):
+def test_wrap_c_ext_module(pytester, import_mode):
     module = get_module('wrap_c_ext_module')
     assert module.exists()
 
-    result = run_pytest(testdir, module, import_mode)
+    result = run_pytest(pytester, module, import_mode)
     result.stdout.fnmatch_lines([
         "*sqr*PASSED*",
     ])
     assert result.ret == 0
 
 
 @pytest.mark.parametrize('import_mode', IMPORT_MODES)
-def test_wrap_cpp_ext_module(testdir, import_mode):
+def test_wrap_cpp_ext_module(pytester, import_mode):
     module = get_module('wrap_cpp_ext_module')
     assert module.exists()
 
-    result = run_pytest(testdir, module, import_mode)
+    result = run_pytest(pytester, module, import_mode)
     result.stdout.fnmatch_lines([
         "*sqr*PASSED*",
     ])
     assert result.ret == 0
 
 
 @pytest.mark.parametrize('import_mode', IMPORT_MODES)
-def test_pure_py_module(testdir, import_mode):
+def test_pure_py_module(pytester, import_mode):
     module = get_module('pure_py_module', suffix='.py')
     assert module.exists()
 
-    result = run_pytest(testdir, module, import_mode)
+    result = run_pytest(pytester, module, import_mode)
     result.stdout.fnmatch_lines([
         "*Eggs.__init__*PASSED*",
         "*Eggs.foo*PASSED*",
         "*foo*PASSED*",
     ])
     assert result.ret == 0
```

