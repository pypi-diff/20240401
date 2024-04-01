# Comparing `tmp/ficamp-0.8.0.tar.gz` & `tmp/ficamp-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ficamp-0.8.0.tar", max compression
+gzip compressed data, was "ficamp-0.9.0.tar", max compression
```

## Comparing `ficamp-0.8.0.tar` & `ficamp-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2024-03-31 14:20:19.953129 ficamp-0.8.0/LICENSE
--rw-r--r--   0        0        0      562 2024-03-31 14:20:19.953129 ficamp-0.8.0/README.md
--rw-r--r--   0        0        0     1072 2024-03-31 14:20:19.953129 ficamp-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/__init__.py
--rw-r--r--   0        0        0     6488 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/__main__.py
--rw-r--r--   0        0        0        0 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/classifier/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/classifier/encoding.py
--rw-r--r--   0        0        0     2226 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/classifier/features.py
--rw-r--r--   0        0        0        0 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/classifier/features_config.py
--rw-r--r--   0        0        0     4151 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/classifier/google_apis.py
--rw-r--r--   0        0        0      359 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/classifier/infer.py
--rw-r--r--   0        0        0        1 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/classifier/payment_method.py
--rw-r--r--   0        0        0      735 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/classifier/preprocessing.py
--rw-r--r--   0        0        0        0 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/data/.gitkeep
--rw-r--r--   0        0        0     1040 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/datastructures.py
--rw-r--r--   0        0        0     5261 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/parsers/abn.py
--rw-r--r--   0        0        0     2421 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/parsers/bbva.py
--rw-r--r--   0        0        0     2859 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/parsers/bsabadell.py
--rw-r--r--   0        0        0     1146 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/parsers/caixabank.py
--rw-r--r--   0        0        0     1031 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/parsers/enums.py
--rw-r--r--   0        0        0      259 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/parsers/protocols.py
--rw-r--r--   0        0        0        0 2024-03-31 14:20:19.953129 ficamp-0.8.0/src/ficamp/py.typed
--rw-r--r--   0        0        0     1296 1970-01-01 00:00:00.000000 ficamp-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-31 14:29:04.326719 ficamp-0.9.0/LICENSE
+-rw-r--r--   0        0        0      562 2024-03-31 14:29:04.326719 ficamp-0.9.0/README.md
+-rw-r--r--   0        0        0     1072 2024-03-31 14:29:04.326719 ficamp-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/__init__.py
+-rw-r--r--   0        0        0     6488 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/__main__.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/classifier/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/classifier/encoding.py
+-rw-r--r--   0        0        0     2226 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/classifier/features.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/classifier/features_config.py
+-rw-r--r--   0        0        0     4151 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/classifier/google_apis.py
+-rw-r--r--   0        0        0      359 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/classifier/infer.py
+-rw-r--r--   0        0        0        1 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/classifier/payment_method.py
+-rw-r--r--   0        0        0      917 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/classifier/preprocessing.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/data/.gitkeep
+-rw-r--r--   0        0        0     1040 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/datastructures.py
+-rw-r--r--   0        0        0     5261 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/parsers/abn.py
+-rw-r--r--   0        0        0     2421 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/parsers/bbva.py
+-rw-r--r--   0        0        0     2859 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/parsers/bsabadell.py
+-rw-r--r--   0        0        0     1146 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/parsers/caixabank.py
+-rw-r--r--   0        0        0     1031 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/parsers/enums.py
+-rw-r--r--   0        0        0      259 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/parsers/protocols.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:29:04.326719 ficamp-0.9.0/src/ficamp/py.typed
+-rw-r--r--   0        0        0     1296 1970-01-01 00:00:00.000000 ficamp-0.9.0/PKG-INFO
```

### Comparing `ficamp-0.8.0/LICENSE` & `ficamp-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ficamp-0.8.0/README.md` & `ficamp-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ficamp-0.8.0/pyproject.toml` & `ficamp-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ficamp"
-version = "0.8.0"
+version = "0.9.0"
 description = "Analyze your bank data and categorize it."
 authors = ["Santiago Fraire Willemoes <santiwilly@gmail.com>"]
 readme = "README.md"
 packages = [
   { include = "ficamp", from = "src" }
 ]
```

### Comparing `ficamp-0.8.0/src/ficamp/__main__.py` & `ficamp-0.9.0/src/ficamp/__main__.py`

 * *Files identical despite different names*

### Comparing `ficamp-0.8.0/src/ficamp/classifier/features.py` & `ficamp-0.9.0/src/ficamp/classifier/features.py`

 * *Files identical despite different names*

### Comparing `ficamp-0.8.0/src/ficamp/classifier/google_apis.py` & `ficamp-0.9.0/src/ficamp/classifier/google_apis.py`

 * *Files identical despite different names*

### Comparing `ficamp-0.8.0/src/ficamp/classifier/preprocessing.py` & `ficamp-0.9.0/src/ficamp/classifier/preprocessing.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,18 +17,28 @@
     return " ".join(clean)
 
 
 def remove_pipes(s: str) -> str:
     return " ".join(s.split("|"))
 
 
+def remove_colon(s: str) -> str:
+    return " ".join(s.split(":"))
+
+
+def remove_comma(s: str) -> str:
+    return " ".join(s.split(","))
+
+
 def preprocess(s: str) -> str:
     "Clean up transaction description"
     steps = (
         lambda s: s.lower(),
         remove_pipes,
+        remove_colon,
+        remove_comma,
         remove_digits,
     )
     out = s
     for func in steps:
         out = func(out)
     return out
```

### Comparing `ficamp-0.8.0/src/ficamp/datastructures.py` & `ficamp-0.9.0/src/ficamp/datastructures.py`

 * *Files identical despite different names*

### Comparing `ficamp-0.8.0/src/ficamp/parsers/abn.py` & `ficamp-0.9.0/src/ficamp/parsers/abn.py`

 * *Files identical despite different names*

### Comparing `ficamp-0.8.0/src/ficamp/parsers/bbva.py` & `ficamp-0.9.0/src/ficamp/parsers/bbva.py`

 * *Files identical despite different names*

### Comparing `ficamp-0.8.0/src/ficamp/parsers/bsabadell.py` & `ficamp-0.9.0/src/ficamp/parsers/bsabadell.py`

 * *Files identical despite different names*

### Comparing `ficamp-0.8.0/src/ficamp/parsers/caixabank.py` & `ficamp-0.9.0/src/ficamp/parsers/caixabank.py`

 * *Files identical despite different names*

### Comparing `ficamp-0.8.0/src/ficamp/parsers/enums.py` & `ficamp-0.9.0/src/ficamp/parsers/enums.py`

 * *Files identical despite different names*

### Comparing `ficamp-0.8.0/PKG-INFO` & `ficamp-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ficamp
-Version: 0.8.0
+Version: 0.9.0
 Summary: Analyze your bank data and categorize it.
 Author: Santiago Fraire Willemoes
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

