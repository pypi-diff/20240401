# Comparing `tmp/approxscimate-0.0.2.tar.gz` & `tmp/approxscimate-0.0.3.tar.gz`

## Comparing `approxscimate-0.0.2.tar` & `approxscimate-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 approxscimate-0.0.2/src/approxscimate/__init__.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 approxscimate-0.0.2/src/approxscimate/cbrt.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 approxscimate-0.0.2/src/approxscimate/comb.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 approxscimate-0.0.2/src/approxscimate/perm.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 approxscimate-0.0.2/validation/cbrt_validation.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 approxscimate-0.0.2/validation/comb_validation.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 approxscimate-0.0.2/validation/perm_validation.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 approxscimate-0.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 approxscimate-0.0.2/LICENSE
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 approxscimate-0.0.2/README.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 approxscimate-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 approxscimate-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 approxscimate-0.0.3/src/approxscimate/__init__.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 approxscimate-0.0.3/src/approxscimate/cbrt.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 approxscimate-0.0.3/src/approxscimate/comb.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 approxscimate-0.0.3/src/approxscimate/perm.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 approxscimate-0.0.3/validation/cbrt_validation.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 approxscimate-0.0.3/validation/comb_validation.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 approxscimate-0.0.3/validation/perm_validation.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 approxscimate-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 approxscimate-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 approxscimate-0.0.3/README.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 approxscimate-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 approxscimate-0.0.3/PKG-INFO
```

### Comparing `approxscimate-0.0.2/src/approxscimate/cbrt.py` & `approxscimate-0.0.3/src/approxscimate/cbrt.py`

 * *Files identical despite different names*

### Comparing `approxscimate-0.0.2/src/approxscimate/comb.py` & `approxscimate-0.0.3/src/approxscimate/comb.py`

 * *Files identical despite different names*

### Comparing `approxscimate-0.0.2/src/approxscimate/perm.py` & `approxscimate-0.0.3/src/approxscimate/perm.py`

 * *Files identical despite different names*

### Comparing `approxscimate-0.0.2/validation/cbrt_validation.py` & `approxscimate-0.0.3/validation/cbrt_validation.py`

 * *Files identical despite different names*

### Comparing `approxscimate-0.0.2/validation/comb_validation.py` & `approxscimate-0.0.3/validation/comb_validation.py`

 * *Files identical despite different names*

### Comparing `approxscimate-0.0.2/validation/perm_validation.py` & `approxscimate-0.0.3/validation/perm_validation.py`

 * *Files identical despite different names*

### Comparing `approxscimate-0.0.2/.gitignore` & `approxscimate-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `approxscimate-0.0.2/LICENSE` & `approxscimate-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `approxscimate-0.0.2/README.md` & `approxscimate-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `approxscimate-0.0.2/pyproject.toml` & `approxscimate-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "approxscimate"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "Lucian Negru", email = "l.negru@student.tudelft.nl" },
     { name = "Eleni Papadopoulou", email = "e.papadopoulou@student.tudelft.nl" },
     { name = "Yang Li", email = "yli59@tudelft.nl" }
 ]
 description = "A package for approximating SciPy functions"
 readme = "README.md"
```

### Comparing `approxscimate-0.0.2/PKG-INFO` & `approxscimate-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: approxscimate
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for approximating SciPy functions
 Project-URL: Homepage, https://github.com/MissingCurlyBracket/ApproxSciMate
 Project-URL: Issues, https://github.com/MissingCurlyBracket/ApproxSciMate/issues
 Author-email: Lucian Negru <l.negru@student.tudelft.nl>, Eleni Papadopoulou <e.papadopoulou@student.tudelft.nl>, Yang Li <yli59@tudelft.nl>
 License-Expression: LGPL-3.0-only
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
```

