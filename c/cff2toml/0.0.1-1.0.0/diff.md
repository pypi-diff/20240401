# Comparing `tmp/cff2toml-0.0.1.tar.gz` & `tmp/cff2toml-1.0.0.tar.gz`

## Comparing `cff2toml-0.0.1.tar` & `cff2toml-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 cff2toml-0.0.1/CITATION.cff
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-0.0.1/src/cff2toml/__init__.py
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 cff2toml-0.0.1/src/cff2toml/cff2toml.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0    11182 2020-02-02 00:00:00.000000 cff2toml-0.0.1/tests/test_cff2toml.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-0.0.1/tests/dummy_files/dummy_CITATION.cff
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-0.0.1/tests/dummy_files/dummy_pyproject.toml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-0.0.1/.gitignore
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-0.0.1/LICENSE
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 cff2toml-0.0.1/README.md
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cff2toml-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 cff2toml-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-1.0.0/CITATION.cff
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-1.0.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-1.0.0/src/cff2toml/__init__.py
+-rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 cff2toml-1.0.0/src/cff2toml/cff2toml.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0    11182 2020-02-02 00:00:00.000000 cff2toml-1.0.0/tests/test_cff2toml.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-1.0.0/tests/dummy_files/dummy_CITATION.cff
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-1.0.0/tests/dummy_files/dummy_pyproject.toml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-1.0.0/.gitignore
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 cff2toml-1.0.0/README.md
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 cff2toml-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 cff2toml-1.0.0/PKG-INFO
```

### Comparing `cff2toml-0.0.1/CITATION.cff` & `cff2toml-1.0.0/CITATION.cff`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,17 @@
   - given-names: Will
     family-names: Riley
     email: wanderingwill@gmail.com
     orcid: "https://orcid.org/0000-0003-1822-6756"
 repository-code: >-
   https://github.com/willynilly/cff2toml
 abstract: >-
-  A module that updates TOML files, including 
-  pyproject.toml files, with metadata from 
-  a CITATION.cff file.
+  A module to synchronize metadata between TOML 
+  and CFF files, including between pyproject.toml 
+  and CITATION.cff files.
 keywords:
   - Citation File Format
   - TOML
+  - pyproject.toml
+  - CITATION.cff
 license: Apache-2.0
-version: "0.0.1"
+version: "1.0.0"
```

### Comparing `cff2toml-0.0.1/.github/workflows/python-publish.yml` & `cff2toml-1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cff2toml-0.0.1/src/cff2toml/cff2toml.py` & `cff2toml-1.0.0/src/cff2toml/cff2toml.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     save_toml_object(toml_object=toml_object,
                      toml_file_path=toml_file_path)
 
     return toml_object
 
 
-def update_cff_with_toml(toml_file_path: str, cff_file_path: str, transform_cff_object_func: TransformCFFObjectWithTOMLObjectFunction) -> CFFObject:
+def update_cff_with_toml(cff_file_path: str, toml_file_path: str, transform_cff_object_func: TransformCFFObjectWithTOMLObjectFunction) -> CFFObject:
 
     toml_object: TOMLObject = load_toml_object(toml_file_path=toml_file_path)
     cff_object: CFFObject = load_cff_object(cff_file_path=cff_file_path)
 
     cff_object: CFFObject = transform_cff_object_func(cff_object, toml_object)
 
     save_cff_object(cff_object=cff_object,
@@ -108,15 +108,15 @@
         pyproject_toml_object['project']['license'] = citation_cff_object['license']
         pyproject_toml_object['project']['urls']['Source'] = citation_cff_object['repository-code']
 
         return pyproject_toml_object
     return update_toml_with_cff(toml_file_path=pyproject_toml_file_path, cff_file_path=citation_cff_file_path, transform_toml_object_func=transformer)
 
 
-def update_citation_cff_with_pyproject_toml(pyproject_toml_file_path=DEFAULT_PYPROJECT_TOML_FILE_PATH, citation_cff_file_path=DEFAULT_CITATION_CFF_FILE_PATH) -> CFFObject:
+def update_citation_cff_with_pyproject_toml(citation_cff_file_path=DEFAULT_CITATION_CFF_FILE_PATH, pyproject_toml_file_path=DEFAULT_PYPROJECT_TOML_FILE_PATH) -> CFFObject:
     def transformer(citation_cff_object: CFFObject, pyproject_toml_object: TOMLObject) -> CFFObject:
         citation_cff_object['title'] = pyproject_toml_object['project']['name']
         citation_cff_object['version'] = pyproject_toml_object['project']['version']
         citation_cff_object['abstract'] = pyproject_toml_object['project']['description']
         citation_cff_object['license'] = pyproject_toml_object['project']['license']
         citation_cff_object['repository-code'] = pyproject_toml_object['project']['urls']['Source']
```

### Comparing `cff2toml-0.0.1/tests/test_cff2toml.py` & `cff2toml-1.0.0/tests/test_cff2toml.py`

 * *Files identical despite different names*

### Comparing `cff2toml-0.0.1/tests/dummy_files/dummy_CITATION.cff` & `cff2toml-1.0.0/tests/dummy_files/dummy_CITATION.cff`

 * *Files identical despite different names*

### Comparing `cff2toml-0.0.1/tests/dummy_files/dummy_pyproject.toml` & `cff2toml-1.0.0/tests/dummy_files/dummy_pyproject.toml`

 * *Files identical despite different names*

### Comparing `cff2toml-0.0.1/LICENSE` & `cff2toml-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cff2toml-0.0.1/pyproject.toml` & `cff2toml-1.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cff2toml"
-version = "0.0.1"
-description = "A library that updates TOML files, including pyproject.toml, with metadata from a CITATION.cff file."
+version = "1.0.0"
+description = "A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "Will Riley", email = "wanderingwill@gmail.com" },
 ]
 classifiers = [
-  "Programming Language :: Python",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: 3.12",
-  "Programming Language :: Python :: Implementation :: CPython",
-  "Programming Language :: Python :: Implementation :: PyPy",
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Education",
+    "Intended Audience :: Information Technology",
+    "Intended Audience :: Science/Research",
+    "Intended Audience :: System Administrators",
+    "License :: OSI Approved :: Apache Software License",
+    "Natural Language :: English",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Topic :: Scientific/Engineering",
+    "Topic :: Software Development",
+    "Topic :: Utilities"
 ]
 dependencies = ["toml==0.10.2", "PyYAML==6.0.1"]
 
 [project.urls]
 Documentation = "https://github.com/willynilly/cff2toml#readme"
 Issues = "https://github.com/willynilly/cff2toml/issues"
-Source = "https://github.com/willnilly/cff2toml"
+Source = "https://github.com/willynilly/cff2toml"
 
 [project.optional-dependencies]
 testing = [
     "pytest==8.1.1",
 ]
```

