# Comparing `tmp/pytest-sphinx-0.6.0.tar.gz` & `tmp/pytest-sphinx-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-sphinx-0.6.0.tar", last modified: Sat Feb  3 20:08:07 2024, max compression
+gzip compressed data, was "pytest-sphinx-0.6.2.tar", last modified: Mon Apr  1 19:02:48 2024, max compression
```

## Comparing `pytest-sphinx-0.6.0.tar` & `pytest-sphinx-0.6.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 20:08:06.998249 pytest-sphinx-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-02-03 20:07:57.000000 pytest-sphinx-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-02-03 20:08:06.998249 pytest-sphinx-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-02-03 20:07:57.000000 pytest-sphinx-0.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-02-03 20:07:57.000000 pytest-sphinx-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-03 20:08:06.998249 pytest-sphinx-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 20:08:06.994249 pytest-sphinx-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 20:08:06.994249 pytest-sphinx-0.6.0/src/pytest_sphinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-02-03 20:08:06.000000 pytest-sphinx-0.6.0/src/pytest_sphinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-03 20:08:06.000000 pytest-sphinx-0.6.0/src/pytest_sphinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 20:08:06.000000 pytest-sphinx-0.6.0/src/pytest_sphinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-03 20:08:06.000000 pytest-sphinx-0.6.0/src/pytest_sphinx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-03 20:08:06.000000 pytest-sphinx-0.6.0/src/pytest_sphinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-03 20:08:06.000000 pytest-sphinx-0.6.0/src/pytest_sphinx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20919 2024-02-03 20:07:57.000000 pytest-sphinx-0.6.0/src/pytest_sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 20:08:06.994249 pytest-sphinx-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-02-03 20:07:57.000000 pytest-sphinx-0.6.0/tests/test_doc2test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-02-03 20:07:57.000000 pytest-sphinx-0.6.0/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-02-03 20:07:57.000000 pytest-sphinx-0.6.0/tests/test_python_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-02-03 20:07:57.000000 pytest-sphinx-0.6.0/tests/test_sphinx_doctest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-02-03 20:07:57.000000 pytest-sphinx-0.6.0/tests/test_text_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:02:48.479334 pytest-sphinx-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-01 19:02:48.479334 pytest-sphinx-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-01 19:02:48.479334 pytest-sphinx-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:02:48.475334 pytest-sphinx-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:02:48.479334 pytest-sphinx-0.6.2/src/pytest_sphinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-01 19:02:48.000000 pytest-sphinx-0.6.2/src/pytest_sphinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-01 19:02:48.000000 pytest-sphinx-0.6.2/src/pytest_sphinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:02:48.000000 pytest-sphinx-0.6.2/src/pytest_sphinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-01 19:02:48.000000 pytest-sphinx-0.6.2/src/pytest_sphinx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 19:02:48.000000 pytest-sphinx-0.6.2/src/pytest_sphinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 19:02:48.000000 pytest-sphinx-0.6.2/src/pytest_sphinx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20687 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/src/pytest_sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:02:48.479334 pytest-sphinx-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/tests/test_doc2test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/tests/test_python_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/tests/test_sphinx_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/tests/test_text_files.py
```

### Comparing `pytest-sphinx-0.6.0/LICENSE` & `pytest-sphinx-0.6.2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Copyright (c) 2017, Thomas Hisch
+Copyright (c) 2017-2024, Thomas Wimmer
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `pytest-sphinx-0.6.0/PKG-INFO` & `pytest-sphinx-0.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pytest-sphinx
-Version: 0.6.0
+Version: 0.6.2
 Summary: Doctest plugin for pytest with support for Sphinx-specific doctest-directives
-Author-email: Thomas Hisch <t.hisch@gmail.com>
-Maintainer-email: Thomas Hisch <t.hisch@gmail.com>
+Author-email: Thomas Wimmer <thomaswimmer@posteo.com>
+Maintainer-email: Thomas Wimmer <thomaswimmer@posteo.com>
 License: 
-        Copyright (c) 2017, Thomas Hisch
+        Copyright (c) 2017-2024, Thomas Wimmer
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         * Redistributions of source code must retain the above copyright notice, this
           list of conditions and the following disclaimer.
```

### Comparing `pytest-sphinx-0.6.0/README.rst` & `pytest-sphinx-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-sphinx-0.6.0/pyproject.toml` & `pytest-sphinx-0.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "pytest-sphinx"
-version = "0.6.0"
+version = "0.6.2"
 description = "Doctest plugin for pytest with support for Sphinx-specific doctest-directives"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["sphinx", "pytest", "rst"]
 authors = [
-    { name="Thomas Hisch", email="t.hisch@gmail.com" }
+    { name="Thomas Wimmer", email="thomaswimmer@posteo.com" }
 ]
 maintainers = [
-    { name="Thomas Hisch", email="t.hisch@gmail.com" }
+    { name="Thomas Wimmer", email="thomaswimmer@posteo.com" }
 ]
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Pytest",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Testing",
```

### Comparing `pytest-sphinx-0.6.0/src/pytest_sphinx.egg-info/PKG-INFO` & `pytest-sphinx-0.6.2/src/pytest_sphinx.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pytest-sphinx
-Version: 0.6.0
+Version: 0.6.2
 Summary: Doctest plugin for pytest with support for Sphinx-specific doctest-directives
-Author-email: Thomas Hisch <t.hisch@gmail.com>
-Maintainer-email: Thomas Hisch <t.hisch@gmail.com>
+Author-email: Thomas Wimmer <thomaswimmer@posteo.com>
+Maintainer-email: Thomas Wimmer <thomaswimmer@posteo.com>
 License: 
-        Copyright (c) 2017, Thomas Hisch
+        Copyright (c) 2017-2024, Thomas Wimmer
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         * Redistributions of source code must retain the above copyright notice, this
           list of conditions and the following disclaimer.
```

### Comparing `pytest-sphinx-0.6.0/src/pytest_sphinx.py` & `pytest-sphinx-0.6.2/src/pytest_sphinx.py`

 * *Files 2% similar despite different names*

```diff
@@ -552,28 +552,23 @@
                 runner=runner,
                 dtest=test,
             )
 
 
 class SphinxDoctestModule(pytest.Module):
     def collect(self) -> Iterator[_pytest.doctest.DoctestItem]:
-        if self.fspath.basename == "conftest.py":
-            module = self.config.pluginmanager._importconftest(
-                self.path,
-                self.config.getoption("importmode"),
-                rootpath=self.config.rootpath,
+        try:
+            module = import_path(
+                self.path, root=self.config.rootpath, consider_namespace_packages=False
             )
-        else:
-            try:
-                module = import_path(self.path, root=self.config.rootpath)
-            except ImportError:
-                if self.config.getvalue("doctest_ignore_import_errors"):
-                    pytest.skip("unable to import module %r" % self.path)
-                else:
-                    raise
+        except ImportError:
+            if self.config.getvalue("doctest_ignore_import_errors"):
+                pytest.skip("unable to import module %r" % self.path)
+            else:
+                raise
         optionflags = _pytest.doctest.get_optionflags(self.config)  # type:ignore
 
         class MockAwareDocTestFinder(doctest.DocTestFinder):
             """
             a hackish doctest finder that overrides stdlib internals to fix
             a stdlib bug
             https://github.com/pytest-dev/pytest/issues/3456
```

### Comparing `pytest-sphinx-0.6.0/tests/test_doc2test.py` & `pytest-sphinx-0.6.2/tests/test_doc2test.py`

 * *Files identical despite different names*

### Comparing `pytest-sphinx-0.6.0/tests/test_options.py` & `pytest-sphinx-0.6.2/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `pytest-sphinx-0.6.0/tests/test_python_files.py` & `pytest-sphinx-0.6.2/tests/test_python_files.py`

 * *Files identical despite different names*

### Comparing `pytest-sphinx-0.6.0/tests/test_sphinx_doctest.py` & `pytest-sphinx-0.6.2/tests/test_sphinx_doctest.py`

 * *Files identical despite different names*

### Comparing `pytest-sphinx-0.6.0/tests/test_text_files.py` & `pytest-sphinx-0.6.2/tests/test_text_files.py`

 * *Files identical despite different names*

