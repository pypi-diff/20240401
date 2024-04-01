# Comparing `tmp/knnclassifier-0.0.1.tar.gz` & `tmp/knnclassifier-0.0.3.tar.gz`

## Comparing `knnclassifier-0.0.1.tar` & `knnclassifier-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 knnclassifier-0.0.1/.gitattributes
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 knnclassifier-0.0.1/src/knnclassifier/__init__.py
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 knnclassifier-0.0.1/src/knnclassifier/knn_module.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 knnclassifier-0.0.1/tests/main.py
--rw-r--r--   0        0        0   188259 2020-02-02 00:00:00.000000 knnclassifier-0.0.1/tests/data/knn_test.txt
--rw-r--r--   0        0        0    80649 2020-02-02 00:00:00.000000 knnclassifier-0.0.1/tests/data/knn_train.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 knnclassifier-0.0.1/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 knnclassifier-0.0.1/LICENSE
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 knnclassifier-0.0.1/README.md
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 knnclassifier-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 knnclassifier-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 knnclassifier-0.0.3/.gitattributes
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 knnclassifier-0.0.3/src/knnclassifier/__init__.py
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 knnclassifier-0.0.3/src/knnclassifier/knn_module.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 knnclassifier-0.0.3/tests/main.py
+-rw-r--r--   0        0        0   188259 2020-02-02 00:00:00.000000 knnclassifier-0.0.3/tests/data/knn_test.txt
+-rw-r--r--   0        0        0    80649 2020-02-02 00:00:00.000000 knnclassifier-0.0.3/tests/data/knn_train.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 knnclassifier-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 knnclassifier-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 knnclassifier-0.0.3/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 knnclassifier-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 knnclassifier-0.0.3/PKG-INFO
```

### Comparing `knnclassifier-0.0.1/src/knnclassifier/knn_module.py` & `knnclassifier-0.0.3/src/knnclassifier/knn_module.py`

 * *Files identical despite different names*

### Comparing `knnclassifier-0.0.1/tests/main.py` & `knnclassifier-0.0.3/tests/main.py`

 * *Files identical despite different names*

### Comparing `knnclassifier-0.0.1/tests/data/knn_test.txt` & `knnclassifier-0.0.3/tests/data/knn_test.txt`

 * *Files identical despite different names*

### Comparing `knnclassifier-0.0.1/tests/data/knn_train.txt` & `knnclassifier-0.0.3/tests/data/knn_train.txt`

 * *Files identical despite different names*

### Comparing `knnclassifier-0.0.1/LICENSE` & `knnclassifier-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `knnclassifier-0.0.1/README.md` & `knnclassifier-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `knnclassifier-0.0.1/pyproject.toml` & `knnclassifier-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [build-system]
-requires = ["hatchling", "numpy"]
+requires = ["hatchling", "numpy", "statistics"]
 build-backend = "hatchling.build"
 
 [project]
 name = "knnclassifier"
-version = "0.0.1"
+version = "0.0.3"
 authors = [
-    { name = "Justin Roche", email = "justinroche03@gmail.com" },
+  { name="Justin Roche", email="justinroche03@gmail.com" },
 ]
 description = "A k-nearest neighbors classifier in Python 3.11.7"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["numpy>=1.23.5"]
 
 [project.urls]
 Homepage = "https://github.com/justinroche/knnclassifier"
 Issues = "https://github.com/justinroche/knnclassifier/issues"
```

### Comparing `knnclassifier-0.0.1/PKG-INFO` & `knnclassifier-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.3
 Name: knnclassifier
-Version: 0.0.1
+Version: 0.0.3
 Summary: A k-nearest neighbors classifier in Python 3.11.7
 Project-URL: Homepage, https://github.com/justinroche/knnclassifier
 Project-URL: Issues, https://github.com/justinroche/knnclassifier/issues
 Author-email: Justin Roche <justinroche03@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: numpy>=1.23.5
 Description-Content-Type: text/markdown
 
 # KNN Classifier
 
 **A k-Nearest Neighbors supervised classifier in Python 3.11.7**
 
 ---
```

