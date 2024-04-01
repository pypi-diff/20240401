# Comparing `tmp/my_first_python_package_0-0.1.4.tar.gz` & `tmp/my_first_python_package_0-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_first_python_package_0-0.1.4.tar", max compression
+gzip compressed data, was "my_first_python_package_0-1.1.0.tar", max compression
```

## Comparing `my_first_python_package_0-0.1.4.tar` & `my_first_python_package_0-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1499 2024-03-30 18:09:26.219800 my_first_python_package_0-0.1.4/LICENSE
--rw-r--r--   0        0        0       25 2024-03-30 18:09:26.219800 my_first_python_package_0-0.1.4/README.md
--rw-r--r--   0        0        0       34 2024-03-31 17:47:02.415572 my_first_python_package_0-0.1.4/my_first_python_package/__init__.py
--rw-r--r--   0        0        0      819 2024-03-31 17:45:27.219574 my_first_python_package_0-0.1.4/my_first_python_package/module1.py
--rw-r--r--   0        0        0      456 2024-03-31 17:46:43.775572 my_first_python_package_0-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 my_first_python_package_0-0.1.4/setup.py
--rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 my_first_python_package_0-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1499 2024-04-01 14:49:41.450012 my_first_python_package_0-1.1.0/LICENSE
+-rw-r--r--   0        0        0       25 2024-04-01 14:49:41.450012 my_first_python_package_0-1.1.0/README.md
+-rw-r--r--   0        0        0       34 2024-04-01 14:49:41.450012 my_first_python_package_0-1.1.0/my_first_python_package/__init__.py
+-rw-r--r--   0        0        0      819 2024-04-01 14:49:41.450012 my_first_python_package_0-1.1.0/my_first_python_package/module1.py
+-rw-r--r--   0        0        0      456 2024-04-01 14:49:41.450012 my_first_python_package_0-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 my_first_python_package_0-1.1.0/PKG-INFO
```

### Comparing `my_first_python_package_0-0.1.4/LICENSE` & `my_first_python_package_0-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `my_first_python_package_0-0.1.4/my_first_python_package/module1.py` & `my_first_python_package_0-1.1.0/my_first_python_package/module1.py`

 * *Files identical despite different names*

### Comparing `my_first_python_package_0-0.1.4/PKG-INFO` & `my_first_python_package_0-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: my-first-python-package-0
-Version: 0.1.4
+Version: 1.1.0
 Summary: A simple package to demonstrate how to create a python package
 License: BSD-3-Clause
 Author: Hassan Abedi
 Author-email: hassan.abedi.t@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Description-Content-Type: text/markdown
 
 # my-first-python-package
```

