# Comparing `tmp/flake8_builtins-2.3.0.tar.gz` & `tmp/flake8_builtins-2.4.0.tar.gz`

## Comparing `flake8_builtins-2.3.0.tar` & `flake8_builtins-2.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 flake8_builtins-2.3.0/.flake8
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 flake8_builtins-2.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5291 2020-02-02 00:00:00.000000 flake8_builtins-2.3.0/CHANGES.rst
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flake8_builtins-2.3.0/MANIFEST.in
--rw-r--r--   0        0        0    10221 2020-02-02 00:00:00.000000 flake8_builtins-2.3.0/flake8_builtins.py
--rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 flake8_builtins-2.3.0/run_tests.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 flake8_builtins-2.3.0/tox.ini
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 flake8_builtins-2.3.0/.github/workflows/testing.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 flake8_builtins-2.3.0/.gitignore
--rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 flake8_builtins-2.3.0/LICENSE
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 flake8_builtins-2.3.0/README.rst
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 flake8_builtins-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 flake8_builtins-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/.flake8
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/CHANGES.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/MANIFEST.in
+-rw-r--r--   0        0        0    10967 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/flake8_builtins.py
+-rw-r--r--   0        0        0    11332 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/run_tests.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/tox.ini
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/.github/workflows/testing.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/.gitignore
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/LICENSE
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/README.rst
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/PKG-INFO
```

### Comparing `flake8_builtins-2.3.0/.pre-commit-config.yaml` & `flake8_builtins-2.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flake8_builtins-2.3.0/CHANGES.rst` & `flake8_builtins-2.4.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 .. -*- coding: utf-8 -*-
 
 Changelog
 =========
 
+2.4.0 (2024-04-01)
+------------------
+
+- Add rule for lambda argument shadowing (`A006`).
+  [cielavenir]
+
+
 2.3.0 (2024-03-29)
 ------------------
 
 - Add rule for builtin module name shadowing (`A005`).
   [asfaltboy]
```

### Comparing `flake8_builtins-2.3.0/flake8_builtins.py` & `flake8_builtins-2.4.0/flake8_builtins.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     name = 'flake8_builtins'
     version = '1.5.2'
     assign_msg = 'A001 variable "{0}" is shadowing a Python builtin'
     argument_msg = 'A002 argument "{0}" is shadowing a Python builtin'
     class_attribute_msg = 'A003 class attribute "{0}" is shadowing a Python builtin'
     import_msg = 'A004 import statement "{0}" is shadowing a Python builtin'
     module_name_msg = 'A005 the module is shadowing a Python builtin module "{0}"'
+    lambda_argument_msg = 'A006 lambda argument "{0}" is shadowing a Python builtin'
 
     names = []
     ignore_list = {
         '__name__',
         '__doc__',
         'credits',
         '_',
@@ -109,14 +110,17 @@
         for statement in ast.walk(tree):
             if isinstance(statement, (ast.Assign, ast.AnnAssign, ast.NamedExpr)):
                 value = self.check_assignment(statement)
 
             elif isinstance(statement, function_nodes):
                 value = self.check_function_definition(statement)
 
+            elif isinstance(statement, ast.Lambda):
+                value = self.check_lambda_definition(statement)
+
             elif isinstance(statement, for_nodes):
                 value = self.check_for_loop(statement)
 
             elif isinstance(statement, with_nodes):
                 value = self.check_with(statement)
 
             elif isinstance(statement, ast.excepthandler):
@@ -177,14 +181,28 @@
             if isinstance(arg, ast.arg) and arg.arg in self.names:
                 yield self.error(
                     arg,
                     message=self.argument_msg,
                     variable=arg.arg,
                 )
 
+    def check_lambda_definition(self, statement):
+        all_arguments = []
+        all_arguments.extend(statement.args.args)
+        all_arguments.extend(getattr(statement.args, 'kwonlyargs', []))
+        all_arguments.extend(getattr(statement.args, 'posonlyargs', []))
+
+        for arg in all_arguments:
+            if isinstance(arg, ast.arg) and arg.arg in self.names:
+                yield self.error(
+                    arg,
+                    message=self.lambda_argument_msg,
+                    variable=arg.arg,
+                )
+
     def check_for_loop(self, statement):
         stack = [statement.target]
         while stack:
             item = stack.pop()
             if isinstance(item, (ast.Tuple, ast.List)):
                 stack.extend(list(item.elts))
             elif isinstance(item, ast.Name) and item.id in self.names:
```

### Comparing `flake8_builtins-2.3.0/run_tests.py` & `flake8_builtins-2.4.0/run_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,14 +152,19 @@
 def test_argument_message():
     source = """
     def bla(list):
         a = 4"""
     check_code(source, 'A002')
 
 
+def test_lambda_argument_message():
+    source = 'takefirst = lambda list: list[0]'
+    check_code(source, 'A006')
+
+
 def test_keyword_argument_message():
     source = """
     def bla(dict=3):
         b = 4"""
     check_code(source, 'A002')
 
 
@@ -179,14 +184,25 @@
     source = """
     def bla(list, /):
         a = 4
     """
     check_code(source, 'A002')
 
 
+@pytest.mark.skipif(
+    sys.version_info < (3, 8),
+    reason='This syntax is only valid in Python 3.8+',
+)
+def test_lambda_posonly_argument_message():
+    source = """
+    takefirst = lambda list, /: list[0]
+    """
+    check_code(source, 'A006')
+
+
 def test_no_error():
     source = """def bla(first):\n    b = 4"""
     check_code(source)
 
 
 def test_method_without_arguments():
     source = """
```

### Comparing `flake8_builtins-2.3.0/tox.ini` & `flake8_builtins-2.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `flake8_builtins-2.3.0/.github/workflows/testing.yml` & `flake8_builtins-2.4.0/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `flake8_builtins-2.3.0/LICENSE` & `flake8_builtins-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_builtins-2.3.0/README.rst` & `flake8_builtins-2.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -100,10 +100,13 @@
 
 A004:
   An import statement is shadowing a Python builtin.
 
 A005:
   A module is shadowing a Python builtin module (e.g: `logging` or `socket`)
 
+A006:
+  A lambda argument is shadowing a Python builtin.
+
 License
 -------
 GPL 2.0
```

### Comparing `flake8_builtins-2.3.0/pyproject.toml` & `flake8_builtins-2.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flake8-builtins"
-version = "2.3.0"
+version = "2.4.0"
 authors = [
   { name="Gil Forcada Codinachs", email="gil.gnome@gmail.com" },
 ]
 description = "Check for python builtins being used as variables or parameters"
 keywords = ["pep8", "flake8", "python", ]
 readme = "README.rst"
 requires-python = ">=3.8"
```

### Comparing `flake8_builtins-2.3.0/PKG-INFO` & `flake8_builtins-2.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-builtins
-Version: 2.3.0
+Version: 2.4.0
 Summary: Check for python builtins being used as variables or parameters
 Project-URL: Homepage, https://github.com/gforcada/flake8-builtins
 Project-URL: Bug Tracker, https://github.com/gforcada/flake8-builtins/issues
 Project-URL: Changelog, https://github.com/gforcada/flake8-builtins/blob/main/CHANGES.rst
 Author-email: Gil Forcada Codinachs <gil.gnome@gmail.com>
 License-File: LICENSE
 Keywords: flake8,pep8,python
@@ -134,10 +134,13 @@
 
 A004:
   An import statement is shadowing a Python builtin.
 
 A005:
   A module is shadowing a Python builtin module (e.g: `logging` or `socket`)
 
+A006:
+  A lambda argument is shadowing a Python builtin.
+
 License
 -------
 GPL 2.0
```

