# Comparing `tmp/python-criteria-0.0.1.tar.gz` & `tmp/python-criteria-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-criteria-0.0.1.tar", last modified: Fri Mar 29 16:46:16 2024, max compression
+gzip compressed data, was "python-criteria-0.1.0.tar", last modified: Mon Apr  1 10:44:12 2024, max compression
```

## Comparing `python-criteria-0.0.1.tar` & `python-criteria-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:46:16.112240 python-criteria-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:46:16.112240 python-criteria-0.0.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-29 16:46:11.000000 python-criteria-0.0.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-03-29 16:46:11.000000 python-criteria-0.0.1/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-29 16:46:11.000000 python-criteria-0.0.1/.devcontainer/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-29 16:46:11.000000 python-criteria-0.0.1/.devcontainer/postCreateCommand.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:46:16.112240 python-criteria-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-29 16:46:11.000000 python-criteria-0.0.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:46:16.112240 python-criteria-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-29 16:46:11.000000 python-criteria-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-03-29 16:46:11.000000 python-criteria-0.0.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:46:16.112240 python-criteria-0.0.1/.husky/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-29 16:46:11.000000 python-criteria-0.0.1/.husky/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-03-29 16:46:11.000000 python-criteria-0.0.1/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:46:16.112240 python-criteria-0.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-29 16:46:11.000000 python-criteria-0.0.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-29 16:46:11.000000 python-criteria-0.0.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-29 16:46:11.000000 python-criteria-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-29 16:46:16.112240 python-criteria-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-29 16:46:11.000000 python-criteria-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-29 16:46:11.000000 python-criteria-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:46:16.112240 python-criteria-0.0.1/python_criteria/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-29 16:46:11.000000 python-criteria-0.0.1/python_criteria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-03-29 16:46:11.000000 python-criteria-0.0.1/python_criteria/clauses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-03-29 16:46:11.000000 python-criteria-0.0.1/python_criteria/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-03-29 16:46:11.000000 python-criteria-0.0.1/python_criteria/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-03-29 16:46:11.000000 python-criteria-0.0.1/python_criteria/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-03-29 16:46:11.000000 python-criteria-0.0.1/python_criteria/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:46:16.112240 python-criteria-0.0.1/python_criteria.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-29 16:46:16.000000 python-criteria-0.0.1/python_criteria.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-29 16:46:16.000000 python-criteria-0.0.1/python_criteria.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 16:46:16.000000 python-criteria-0.0.1/python_criteria.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-29 16:46:16.000000 python-criteria-0.0.1/python_criteria.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 16:46:16.112240 python-criteria-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:12.424087 python-criteria-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:12.420087 python-criteria-0.1.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-01 10:44:07.000000 python-criteria-0.1.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-01 10:44:07.000000 python-criteria-0.1.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-01 10:44:07.000000 python-criteria-0.1.0/.devcontainer/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-01 10:44:07.000000 python-criteria-0.1.0/.devcontainer/postCreateCommand.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:12.424087 python-criteria-0.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-01 10:44:07.000000 python-criteria-0.1.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:12.424087 python-criteria-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-01 10:44:07.000000 python-criteria-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-01 10:44:07.000000 python-criteria-0.1.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:12.424087 python-criteria-0.1.0/.husky/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 10:44:07.000000 python-criteria-0.1.0/.husky/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-01 10:44:07.000000 python-criteria-0.1.0/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:12.424087 python-criteria-0.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-01 10:44:07.000000 python-criteria-0.1.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-01 10:44:07.000000 python-criteria-0.1.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-01 10:44:07.000000 python-criteria-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-01 10:44:12.424087 python-criteria-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-01 10:44:07.000000 python-criteria-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-01 10:44:07.000000 python-criteria-0.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:12.424087 python-criteria-0.1.0/python_criteria/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-01 10:44:07.000000 python-criteria-0.1.0/python_criteria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-01 10:44:07.000000 python-criteria-0.1.0/python_criteria/clauses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-01 10:44:07.000000 python-criteria-0.1.0/python_criteria/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-01 10:44:07.000000 python-criteria-0.1.0/python_criteria/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-01 10:44:07.000000 python-criteria-0.1.0/python_criteria/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-01 10:44:07.000000 python-criteria-0.1.0/python_criteria/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:12.424087 python-criteria-0.1.0/python_criteria.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-01 10:44:12.000000 python-criteria-0.1.0/python_criteria.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-01 10:44:12.000000 python-criteria-0.1.0/python_criteria.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 10:44:12.000000 python-criteria-0.1.0/python_criteria.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 10:44:12.000000 python-criteria-0.1.0/python_criteria.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 10:44:12.424087 python-criteria-0.1.0/setup.cfg
```

### Comparing `python-criteria-0.0.1/.devcontainer/devcontainer.json` & `python-criteria-0.1.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `python-criteria-0.0.1/.devcontainer/docker-compose.yml` & `python-criteria-0.1.0/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `python-criteria-0.0.1/.github/workflows/python-publish.yml` & `python-criteria-0.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `python-criteria-0.0.1/.gitignore` & `python-criteria-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python-criteria-0.0.1/.pylintrc` & `python-criteria-0.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `python-criteria-0.0.1/.vscode/tasks.json` & `python-criteria-0.1.0/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `python-criteria-0.0.1/LICENSE` & `python-criteria-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-criteria-0.0.1/pyproject.toml` & `python-criteria-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-criteria-0.0.1/python_criteria/clauses.py` & `python-criteria-0.1.0/python_criteria/clauses.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.0.1/python_criteria/entity.py` & `python-criteria-0.1.0/python_criteria/entity.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.0.1/python_criteria/filter.py` & `python-criteria-0.1.0/python_criteria/filter.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.0.1/python_criteria/visitor.py` & `python-criteria-0.1.0/python_criteria/visitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,14 @@
 from typing import Any
 
 from .clauses import BooleanClause, BooleanClauseList
 from .filter import FilterableAttribute
 
 
 class BaseVisitor(metaclass=abc.ABCMeta):
-    mapping_object: Any
-
-    def __init__(self, mapping_object: Any) -> None:
-        self.mapping_object = mapping_object
-
     @classmethod
     def __subclasshook__(cls, subclass):
         return (
             hasattr(subclass, "visit_eq")
             and callable(subclass.visit_eq)
             and hasattr(subclass, "visit_ne")
             and callable(subclass.visit_ne)
@@ -39,82 +34,83 @@
             and hasattr(subclass, "visit_xor")
             and callable(subclass.visit_xor)
             and hasattr(subclass, "visit_not")
             and callable(subclass.visit_not)
             or NotImplemented
         )
 
-    def _attr(self, field: FilterableAttribute):
-        if not hasattr(self.mapping_object, field.name):
+    def _attr(self, mapping_object: Any, field: FilterableAttribute):
+        if not hasattr(mapping_object, field.name):
             raise ValueError(
                 f"'{field.name}' is not a valid attribute of '{field.parent_class.__name__}'"
             )
 
-        return getattr(self.mapping_object, field.name)
+        return getattr(mapping_object, field.name)
 
     def visit(
         self,
+        mapping_object: Any,
         filter_or_comparison: FilterableAttribute | BooleanClause | BooleanClauseList,
     ):
         name = filter_or_comparison.__class__.__name__.lower()
         method = getattr(self, "visit_" + name)
 
         if isinstance(filter_or_comparison, BooleanClauseList):
             comparisons = []
             for _filter in filter_or_comparison.clause_list:
-                comparisons.append(self.visit(_filter))
+                comparisons.append(self.visit(mapping_object, _filter))
 
-            return method(comparisons)
+            return method(mapping_object, comparisons)
 
-        return method(filter_or_comparison)
+        return method(mapping_object, filter_or_comparison)
 
     @abc.abstractmethod
-    def visit_eq(self, comparison: BooleanClause):
+    def visit_eq(self, mapping_object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_ne(self, comparison: BooleanClause):
+    def visit_ne(self, mapping_object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_lt(self, comparison: BooleanClause):
+    def visit_lt(self, mapping_object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_le(self, comparison: BooleanClause):
+    def visit_le(self, mapping_object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_gt(self, comparison: BooleanClause):
+    def visit_gt(self, mapping_object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_ge(self, comparison: BooleanClause):
+    def visit_ge(self, mapping_object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_in(self, comparison: BooleanClause):
+    def visit_in(self, mapping_object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_like(self, comparison: BooleanClause):
+    def visit_like(self, mapping_object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_not_like(self, comparison: BooleanClause):
+    def visit_not_like(self, mapping_object: Any, comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_or(self, comparisons: list[Any]):
+    def visit_or(self, mapping_object: Any, comparisons: list[Any]):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_and(self, comparisons: list[Any]):
+    def visit_and(self, mapping_object: Any, comparisons: list[Any]):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_xor(self, comparisons: list[Any]):
+    def visit_xor(self, mapping_object: Any, comparisons: list[Any]):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_not(self, comparisons: list[Any]):
+    def visit_not(self, mapping_object: Any, comparisons: list[Any]):
         raise NotImplementedError
```

### Comparing `python-criteria-0.0.1/python_criteria.egg-info/SOURCES.txt` & `python-criteria-0.1.0/python_criteria.egg-info/SOURCES.txt`

 * *Files identical despite different names*

