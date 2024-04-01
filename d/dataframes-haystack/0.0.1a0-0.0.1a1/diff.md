# Comparing `tmp/dataframes_haystack-0.0.1a0.tar.gz` & `tmp/dataframes_haystack-0.0.1a1.tar.gz`

## Comparing `dataframes_haystack-0.0.1a0.tar` & `dataframes_haystack-0.0.1a1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a0/.github/workflows/test.yml
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a0/src/dataframes_haystack/__about__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a0/src/dataframes_haystack/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a0/src/dataframes_haystack/components/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a0/src/dataframes_haystack/components/converters/__init__.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a0/src/dataframes_haystack/components/converters/pandas.py
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a0/src/dataframes_haystack/components/converters/polars.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a0/tests/__init__.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a0/tests/test_converters_pandas.py
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a0/tests/test_converters_polars.py
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a0/.gitignore
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a0/LICENSE.txt
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a0/README.md
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a1/src/dataframes_haystack/__about__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a1/src/dataframes_haystack/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a1/src/dataframes_haystack/components/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a1/src/dataframes_haystack/components/converters/__init__.py
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a1/src/dataframes_haystack/components/converters/pandas.py
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a1/src/dataframes_haystack/components/converters/polars.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a1/tests/__init__.py
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a1/tests/test_converters_pandas.py
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a1/tests/test_converters_polars.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a1/.gitignore
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a1/LICENSE.txt
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a1/README.md
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 dataframes_haystack-0.0.1a1/PKG-INFO
```

### Comparing `dataframes_haystack-0.0.1a0/.pre-commit-config.yaml` & `dataframes_haystack-0.0.1a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dataframes_haystack-0.0.1a0/.github/workflows/test.yml` & `dataframes_haystack-0.0.1a1/.github/workflows/test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: test
+name: Run tests
 
 on:
   push:
     branches: [main]
   pull_request:
     branches: [main]
 
@@ -34,9 +34,9 @@
 
     - name: Install Hatch
       run: pip install --upgrade hatch
 
     # - name: Run mypy types checking
     #   run: hatch run types:check
 
-    - name: Run tests
+    - name: Run unit tests
       run: hatch run test-cov-all
```

### Comparing `dataframes_haystack-0.0.1a0/src/dataframes_haystack/components/converters/pandas.py` & `dataframes_haystack-0.0.1a1/src/dataframes_haystack/components/converters/pandas.py`

 * *Files identical despite different names*

### Comparing `dataframes_haystack-0.0.1a0/src/dataframes_haystack/components/converters/polars.py` & `dataframes_haystack-0.0.1a1/src/dataframes_haystack/components/converters/polars.py`

 * *Files identical despite different names*

### Comparing `dataframes_haystack-0.0.1a0/tests/test_converters_pandas.py` & `dataframes_haystack-0.0.1a1/tests/test_converters_pandas.py`

 * *Files identical despite different names*

### Comparing `dataframes_haystack-0.0.1a0/tests/test_converters_polars.py` & `dataframes_haystack-0.0.1a1/tests/test_converters_polars.py`

 * *Files identical despite different names*

### Comparing `dataframes_haystack-0.0.1a0/.gitignore` & `dataframes_haystack-0.0.1a1/.gitignore`

 * *Files identical despite different names*

### Comparing `dataframes_haystack-0.0.1a0/LICENSE.txt` & `dataframes_haystack-0.0.1a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataframes_haystack-0.0.1a0/README.md` & `dataframes_haystack-0.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `dataframes_haystack-0.0.1a0/pyproject.toml` & `dataframes_haystack-0.0.1a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dataframes_haystack-0.0.1a0/PKG-INFO` & `dataframes_haystack-0.0.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dataframes-haystack
-Version: 0.0.1a0
+Version: 0.0.1a1
 Project-URL: Documentation, https://github.com/EdAbati/dataframes-haystack#readme
 Project-URL: Issues, https://github.com/EdAbati/dataframes-haystack/issues
 Project-URL: Source, https://github.com/EdAbati/dataframes-haystack
 Author-email: Edoardo Abati <29585319+EdAbati@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

