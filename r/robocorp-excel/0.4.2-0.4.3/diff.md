# Comparing `tmp/robocorp_excel-0.4.2.tar.gz` & `tmp/robocorp_excel-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_excel-0.4.2.tar", max compression
+gzip compressed data, was "robocorp_excel-0.4.3.tar", max compression
```

## Comparing `robocorp_excel-0.4.2.tar` & `robocorp_excel-0.4.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0     1217 2024-01-15 11:51:40.102405 robocorp_excel-0.4.2/README.md
--rw-r--r--   0        0        0      803 2024-01-15 11:51:40.106405 robocorp_excel-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      198 2024-01-15 11:51:40.106405 robocorp_excel-0.4.2/src/robocorp/excel/__init__.py
--rw-r--r--   0        0        0      598 2024-01-15 11:51:40.106405 robocorp_excel-0.4.2/src/robocorp/excel/_types.py
--rw-r--r--   0        0        0    23050 2024-01-15 11:51:40.106405 robocorp_excel-0.4.2/src/robocorp/excel/_workbooks.py
--rw-r--r--   0        0        0     2657 2024-01-15 11:51:40.106405 robocorp_excel-0.4.2/src/robocorp/excel/excel.py
--rw-r--r--   0        0        0        0 2024-01-15 11:51:40.106405 robocorp_excel-0.4.2/src/robocorp/excel/py.typed
--rw-r--r--   0        0        0    65761 2024-01-15 11:51:40.106405 robocorp_excel-0.4.2/src/robocorp/excel/tables.py
--rw-r--r--   0        0        0     2681 2024-01-15 11:51:40.106405 robocorp_excel-0.4.2/src/robocorp/excel/workbook.py
--rw-r--r--   0        0        0     5059 2024-01-15 11:51:40.106405 robocorp_excel-0.4.2/src/robocorp/excel/worksheet.py
--rw-r--r--   0        0        0     2129 1970-01-01 00:00:00.000000 robocorp_excel-0.4.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1692 2024-04-01 13:48:59.185861 robocorp_excel-0.4.3/README.md
+-rw-r--r--   0        0        0      840 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      418 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/src/robocorp/excel/__init__.py
+-rw-r--r--   0        0        0      598 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/src/robocorp/excel/_types.py
+-rw-r--r--   0        0        0    23050 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/src/robocorp/excel/_workbooks.py
+-rw-r--r--   0        0        0     2657 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/src/robocorp/excel/excel.py
+-rw-r--r--   0        0        0        0 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/src/robocorp/excel/py.typed
+-rw-r--r--   0        0        0    65761 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/src/robocorp/excel/tables.py
+-rw-r--r--   0        0        0     2681 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/src/robocorp/excel/workbook.py
+-rw-r--r--   0        0        0     5059 2024-04-01 13:48:59.189861 robocorp_excel-0.4.3/src/robocorp/excel/worksheet.py
+-rw-r--r--   0        0        0     2604 1970-01-01 00:00:00.000000 robocorp_excel-0.4.3/PKG-INFO
```

### Comparing `robocorp_excel-0.4.2/README.md` & `robocorp_excel-0.4.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 # robocorp-excel
 
 This library provides a simple way to deal with both legacy `.xls` files
 and newer `.xlsx` files directly. It can be used to read and edit them
 directly without having Microsoft Excel installed.
 
+> ⚠️ This library isn't included by default in `robocorp`. In order to use this, you
+> have to make it available in your Python environment by listing
+> ![`robocorp-excel`](https://img.shields.io/pypi/v/robocorp-excel?label=robocorp-excel)
+> as a requirement in your dependencies configuration file:
+> - _conda.yaml_ for an automation Task Package
+> - _action-package.yaml_ for an automation Action Package
+> - _requirements.txt_, _pyproject.toml_ etc. for the rest
+
 > 👉 `robocorp-excel` is not yet production ready. 
-> We work in semver and consider versions below 1.0.0 as development phase releases, you can use them but to get to v1 we need to get the 
-> feature support and testing to a level where we feel comfortable recommending production usage.
+> We work in semver and consider versions below 1.0.0 as development phase releases,
+> you can use them but to get to v1 we need to get the feature support and testing to a
+> level where we feel comfortable recommending production usage.
 
 ## Getting started
 
 ```python
 from robocorp import excel
 from robocorp.tasks import task
 
 @task
 def inspect_workbook():
     workbook = excel.open_workbook("orders.xlsx")
     worksheet = workbook.worksheet("Sheet1")
 
     for row in worksheet.as_table(header=True):
-    	print(row)
+        print(row)
 ```
 
 Further user guides and tutorials can be found in [Robocorp Docs](https://robocorp.com/docs).
 
 ## API Reference
 
 Information on specific functions or classes: [robocorp.excel](https://github.com/robocorp/robocorp/blob/master/excel/docs/api/robocorp.excel.md)
```

### Comparing `robocorp_excel-0.4.2/pyproject.toml` & `robocorp_excel-0.4.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-excel"
-version = "0.4.2"
+version = "0.4.3"
 description = "Robocorp Excel automation library"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Cosmin P. <cosmin@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
@@ -23,13 +23,16 @@
 pillow = ">=9.1.1,<11.0.0"
 xlrd = "^2.0.1"
 xlwt = "^1.3.0"
 xlutils = "^2.0.0"
 openpyxl = "^3.0.9"
 typing-extensions = "^4.5.0"
 
+[tool.mypy]
+mypy_path = "src:tests"
+
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = {path = "../devutils/", develop = true}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `robocorp_excel-0.4.2/src/robocorp/excel/_types.py` & `robocorp_excel-0.4.3/src/robocorp/excel/_types.py`

 * *Files identical despite different names*

### Comparing `robocorp_excel-0.4.2/src/robocorp/excel/_workbooks.py` & `robocorp_excel-0.4.3/src/robocorp/excel/_workbooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_excel-0.4.2/src/robocorp/excel/excel.py` & `robocorp_excel-0.4.3/src/robocorp/excel/excel.py`

 * *Files identical despite different names*

### Comparing `robocorp_excel-0.4.2/src/robocorp/excel/tables.py` & `robocorp_excel-0.4.3/src/robocorp/excel/tables.py`

 * *Files identical despite different names*

### Comparing `robocorp_excel-0.4.2/src/robocorp/excel/workbook.py` & `robocorp_excel-0.4.3/src/robocorp/excel/workbook.py`

 * *Files identical despite different names*

### Comparing `robocorp_excel-0.4.2/src/robocorp/excel/worksheet.py` & `robocorp_excel-0.4.3/src/robocorp/excel/worksheet.py`

 * *Files identical despite different names*

### Comparing `robocorp_excel-0.4.2/PKG-INFO` & `robocorp_excel-0.4.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-excel
-Version: 0.4.2
+Version: 0.4.3
 Summary: Robocorp Excel automation library
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -24,31 +24,40 @@
 
 # robocorp-excel
 
 This library provides a simple way to deal with both legacy `.xls` files
 and newer `.xlsx` files directly. It can be used to read and edit them
 directly without having Microsoft Excel installed.
 
+> ⚠️ This library isn't included by default in `robocorp`. In order to use this, you
+> have to make it available in your Python environment by listing
+> ![`robocorp-excel`](https://img.shields.io/pypi/v/robocorp-excel?label=robocorp-excel)
+> as a requirement in your dependencies configuration file:
+> - _conda.yaml_ for an automation Task Package
+> - _action-package.yaml_ for an automation Action Package
+> - _requirements.txt_, _pyproject.toml_ etc. for the rest
+
 > 👉 `robocorp-excel` is not yet production ready. 
-> We work in semver and consider versions below 1.0.0 as development phase releases, you can use them but to get to v1 we need to get the 
-> feature support and testing to a level where we feel comfortable recommending production usage.
+> We work in semver and consider versions below 1.0.0 as development phase releases,
+> you can use them but to get to v1 we need to get the feature support and testing to a
+> level where we feel comfortable recommending production usage.
 
 ## Getting started
 
 ```python
 from robocorp import excel
 from robocorp.tasks import task
 
 @task
 def inspect_workbook():
     workbook = excel.open_workbook("orders.xlsx")
     worksheet = workbook.worksheet("Sheet1")
 
     for row in worksheet.as_table(header=True):
-    	print(row)
+        print(row)
 ```
 
 Further user guides and tutorials can be found in [Robocorp Docs](https://robocorp.com/docs).
 
 ## API Reference
 
 Information on specific functions or classes: [robocorp.excel](https://github.com/robocorp/robocorp/blob/master/excel/docs/api/robocorp.excel.md)
```

