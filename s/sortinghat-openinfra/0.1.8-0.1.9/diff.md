# Comparing `tmp/sortinghat_openinfra-0.1.8.tar.gz` & `tmp/sortinghat_openinfra-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortinghat_openinfra-0.1.8.tar", max compression
+gzip compressed data, was "sortinghat_openinfra-0.1.9.tar", max compression
```

## Comparing `sortinghat_openinfra-0.1.8.tar` & `sortinghat_openinfra-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-07-19 09:40:32.598231 sortinghat_openinfra-0.1.8/LICENSE
--rw-r--r--   0        0        0     2244 2023-07-19 09:40:32.598231 sortinghat_openinfra-0.1.8/README.md
--rw-r--r--   0        0        0     1248 2023-07-19 09:40:32.598231 sortinghat_openinfra-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       86 2023-07-19 09:40:32.598231 sortinghat_openinfra-0.1.8/sortinghat/core/importer/backends/_version.py
--rw-r--r--   0        0        0     7917 2023-07-19 09:40:32.598231 sortinghat_openinfra-0.1.8/sortinghat/core/importer/backends/openinfra.py
--rw-r--r--   0        0        0        0 2023-07-19 09:40:32.598231 sortinghat_openinfra-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0     6403 2023-07-19 09:40:32.598231 sortinghat_openinfra-0.1.8/tests/data/openinfra_page_1.json
--rw-r--r--   0        0        0     5073 2023-07-19 09:40:32.598231 sortinghat_openinfra-0.1.8/tests/data/openinfra_page_2.json
--rw-r--r--   0        0        0     2595 2023-07-19 09:40:32.598231 sortinghat_openinfra-0.1.8/tests/data/openinfra_private.json
--rw-r--r--   0        0        0      143 2023-07-19 09:40:32.598231 sortinghat_openinfra-0.1.8/tests/data/openinfra_token_error.json
--rw-r--r--   0        0        0    21169 2023-07-19 09:40:32.598231 sortinghat_openinfra-0.1.8/tests/test_openinfra.py
--rw-r--r--   0        0        0     3359 1970-01-01 00:00:00.000000 sortinghat_openinfra-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-24 09:52:02.717595 sortinghat_openinfra-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2244 2023-07-24 09:52:02.717595 sortinghat_openinfra-0.1.9/README.md
+-rw-r--r--   0        0        0     1248 2023-07-24 09:52:02.721595 sortinghat_openinfra-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-07-24 09:52:02.721595 sortinghat_openinfra-0.1.9/sortinghat/core/importer/backends/_version.py
+-rw-r--r--   0        0        0     7917 2023-07-24 09:52:02.721595 sortinghat_openinfra-0.1.9/sortinghat/core/importer/backends/openinfra.py
+-rw-r--r--   0        0        0        0 2023-07-24 09:52:02.721595 sortinghat_openinfra-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0     6403 2023-07-24 09:52:02.721595 sortinghat_openinfra-0.1.9/tests/data/openinfra_page_1.json
+-rw-r--r--   0        0        0     5073 2023-07-24 09:52:02.721595 sortinghat_openinfra-0.1.9/tests/data/openinfra_page_2.json
+-rw-r--r--   0        0        0     2595 2023-07-24 09:52:02.721595 sortinghat_openinfra-0.1.9/tests/data/openinfra_private.json
+-rw-r--r--   0        0        0      143 2023-07-24 09:52:02.721595 sortinghat_openinfra-0.1.9/tests/data/openinfra_token_error.json
+-rw-r--r--   0        0        0    21169 2023-07-24 09:52:02.721595 sortinghat_openinfra-0.1.9/tests/test_openinfra.py
+-rw-r--r--   0        0        0     3359 1970-01-01 00:00:00.000000 sortinghat_openinfra-0.1.9/PKG-INFO
```

### Comparing `sortinghat_openinfra-0.1.8/LICENSE` & `sortinghat_openinfra-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.8/README.md` & `sortinghat_openinfra-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.8/pyproject.toml` & `sortinghat_openinfra-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sortinghat-openinfra"
-version = "0.1.8"
+version = "0.1.9"
 description = "SortingHat backend to import identities from OpenInfraID"
 authors = [
     "Bitergia Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `sortinghat_openinfra-0.1.8/sortinghat/core/importer/backends/openinfra.py` & `sortinghat_openinfra-0.1.9/sortinghat/core/importer/backends/openinfra.py`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.8/tests/data/openinfra_page_1.json` & `sortinghat_openinfra-0.1.9/tests/data/openinfra_page_1.json`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.8/tests/data/openinfra_page_2.json` & `sortinghat_openinfra-0.1.9/tests/data/openinfra_page_2.json`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.8/tests/data/openinfra_private.json` & `sortinghat_openinfra-0.1.9/tests/data/openinfra_private.json`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.8/tests/test_openinfra.py` & `sortinghat_openinfra-0.1.9/tests/test_openinfra.py`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.8/PKG-INFO` & `sortinghat_openinfra-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortinghat-openinfra
-Version: 0.1.8
+Version: 0.1.9
 Summary: SortingHat backend to import identities from OpenInfraID
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab,sortinghat
 Author: Bitergia Developers
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

