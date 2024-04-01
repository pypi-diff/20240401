# Comparing `tmp/approxscimate-0.0.1.tar.gz` & `tmp/approxscimate-0.0.2.tar.gz`

## Comparing `approxscimate-0.0.1.tar` & `approxscimate-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 approxscimate-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 approxscimate-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 approxscimate-0.0.1/src/approxscimate/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 approxscimate-0.0.1/src/approxscimate/example.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 approxscimate-0.0.1/LICENSE
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 approxscimate-0.0.1/README.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 approxscimate-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 approxscimate-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 approxscimate-0.0.2/src/approxscimate/__init__.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 approxscimate-0.0.2/src/approxscimate/cbrt.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 approxscimate-0.0.2/src/approxscimate/comb.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 approxscimate-0.0.2/src/approxscimate/perm.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 approxscimate-0.0.2/validation/cbrt_validation.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 approxscimate-0.0.2/validation/comb_validation.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 approxscimate-0.0.2/validation/perm_validation.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 approxscimate-0.0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 approxscimate-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 approxscimate-0.0.2/README.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 approxscimate-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 approxscimate-0.0.2/PKG-INFO
```

### Comparing `approxscimate-0.0.1/LICENSE` & `approxscimate-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `approxscimate-0.0.1/pyproject.toml` & `approxscimate-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "approxscimate"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
-  { name="Lucian Negru", email="l.negru@student.tudelft.nl" },
-  { name="Eleni Papadopoulou", email="e.papadopoulou@student.tudelft.nl" },
-  { name="Yang Li", email="yli59@tudelft.nl" }
+    { name = "Lucian Negru", email = "l.negru@student.tudelft.nl" },
+    { name = "Eleni Papadopoulou", email = "e.papadopoulou@student.tudelft.nl" },
+    { name = "Yang Li", email = "yli59@tudelft.nl" }
 ]
 description = "A package for approximating SciPy functions"
 readme = "README.md"
 requires-python = ">=3.8"
+dependencies = [
+    "scipy >= 1.12.0",
+]
 license = "LGPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

