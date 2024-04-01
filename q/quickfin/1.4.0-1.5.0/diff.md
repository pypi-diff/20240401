# Comparing `tmp/quickfin-1.4.0.tar.gz` & `tmp/quickfin-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickfin-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quickfin-1.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quickfin-1.4.0.tar` & `quickfin-1.5.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       66 2024-04-01 12:12:25.158711 quickfin-1.4.0/README.md
--rw-r--r--   0        0        0      770 2024-04-01 12:32:41.881155 quickfin-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    28569 2024-04-01 12:31:52.629652 quickfin-1.4.0/quickfin.py
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 quickfin-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-01 12:12:25.158711 quickfin-1.5.0/README.md
+-rw-r--r--   0        0        0      770 2024-04-01 12:34:56.676433 quickfin-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    28708 2024-04-01 12:34:50.989524 quickfin-1.5.0/quickfin.py
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 quickfin-1.5.0/PKG-INFO
```

### Comparing `quickfin-1.4.0/pyproject.toml` & `quickfin-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quickfin"
-version = "1.4.0"
+version = "1.5.0"
 authors = [{name = "Derek Evans", email = "derek.evans@deinfoservice.com"}]
 description = "A Python module providing instant access to live and historical stock market price data, automated Plotly data visualization generators and a metadata catalog for referencing equities, stock symbols, sectors, and industry information."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `quickfin-1.4.0/quickfin.py` & `quickfin-1.5.0/quickfin.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 A Python module providing instant access to live
 and historical stock market price data, automated
 Plotly data visualization generators and a metadata
 catalog for referencing equities, stock symbols, sectors,
 and industry information.
 """
 
-__version__ = "1.4.0"
+__version__ = "1.5.0"
 __author__ = "Derek Evans <https://github.com/REPNOT>"
 __date__ = "28 March 2024"
 
 import json
 from pprint import pprint
 import requests
 import datetime
@@ -44,14 +44,16 @@
         """
         Initialize the FinInfo class and retreive metadata catalog.
         """
 
         self.url = "https://gist.githubusercontent.com/REPNOT/6bffda0dd727d63a0bd727d4ff1c890a/raw/ec1ea323068b45739ddd595dfab897cc5f7c6487/fin_data.json"
         self.data = requests.get(self.url).json()
 
+        # self.data = fileOps.rd_json_file("data", "fin_data")
+
 
     def equity(self, symbol, payload=True):
 
         """
         Return object containing the symbol, company name,
         sector, and industry for the stock symbol passed to
         the `symbol` parameter.
@@ -544,15 +546,17 @@
         data for all available dates.
 
 
         """
 
         self.symbol = symbol
 
-        if (date_start != None and date_end == None) or (date_start == None and date_end != None):
+        if date_start == None and date_end == None:
+            pass
+        elif (date_start != None and date_end == None) or (date_start == None and date_end != None):
             return '===  ERROR: BOTH date_start & date_end MUST BE POSITIVE INTEGER VALUES FOR DATE RANGES  ==='
         elif date_start != None and date_end != None and type(date_start) is not int or type(date_end) is not int or date_start <= 0 or date_start <= 0:
             return '===  ERROR: BOTH date_start & date_end MUST BE POSITIVE INTEGER VALUES FOR DATE RANGES  ==='
         else:
             pass
 
         try:
```

### Comparing `quickfin-1.4.0/PKG-INFO` & `quickfin-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickfin
-Version: 1.4.0
+Version: 1.5.0
 Summary: A Python module providing instant access to live and historical stock market price data, automated Plotly data visualization generators and a metadata catalog for referencing equities, stock symbols, sectors, and industry information.
 Author-email: Derek Evans <derek.evans@deinfoservice.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

