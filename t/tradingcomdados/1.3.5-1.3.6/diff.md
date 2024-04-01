# Comparing `tmp/tradingcomdados-1.3.5.tar.gz` & `tmp/tradingcomdados-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingcomdados-1.3.5.tar", last modified: Thu Mar 28 17:36:44 2024, max compression
+gzip compressed data, was "tradingcomdados-1.3.6.tar", last modified: Mon Apr  1 14:26:36 2024, max compression
```

## Comparing `tradingcomdados-1.3.5.tar` & `tradingcomdados-1.3.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 17:36:44.461578 tradingcomdados-1.3.5/
--rw-rw-rw-   0        0        0     2779 2024-03-28 17:36:44.459578 tradingcomdados-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     2375 2024-03-20 00:11:50.000000 tradingcomdados-1.3.5/README.md
--rw-rw-rw-   0        0        0      452 2024-03-28 17:34:51.000000 tradingcomdados-1.3.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-28 17:36:44.461578 tradingcomdados-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-28 17:36:44.382250 tradingcomdados-1.3.5/tradingcomdados/
--rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.3.5/tradingcomdados/__init__.py
--rw-rw-rw-   0        0        0     4890 2024-03-20 00:11:50.000000 tradingcomdados-1.3.5/tradingcomdados/alternative_data.py
--rw-rw-rw-   0        0        0    16846 2024-03-22 13:38:14.000000 tradingcomdados-1.3.5/tradingcomdados/data_provider.py
--rw-rw-rw-   0        0        0     4470 2024-03-20 00:11:50.000000 tradingcomdados-1.3.5/tradingcomdados/funds_data.py
--rw-rw-rw-   0        0        0     6915 2023-07-11 00:58:03.000000 tradingcomdados-1.3.5/tradingcomdados/portfolio.py
--rw-rw-rw-   0        0        0     8924 2024-03-20 00:11:50.000000 tradingcomdados-1.3.5/tradingcomdados/supervised_learning.py
--rw-rw-rw-   0        0        0    37098 2023-07-02 18:17:22.000000 tradingcomdados-1.3.5/tradingcomdados/ta_indicators.py
--rw-rw-rw-   0        0        0     6347 2023-06-20 01:15:28.000000 tradingcomdados-1.3.5/tradingcomdados/unsupervised_learning.py
-drwxrwxrwx   0        0        0        0 2024-03-28 17:36:44.458579 tradingcomdados-1.3.5/tradingcomdados.egg-info/
--rw-rw-rw-   0        0        0     2779 2024-03-28 17:36:42.000000 tradingcomdados-1.3.5/tradingcomdados.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2024-03-28 17:36:43.000000 tradingcomdados-1.3.5/tradingcomdados.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 17:36:42.000000 tradingcomdados-1.3.5/tradingcomdados.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2024-03-28 17:36:42.000000 tradingcomdados-1.3.5/tradingcomdados.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-28 17:36:42.000000 tradingcomdados-1.3.5/tradingcomdados.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 14:26:36.127859 tradingcomdados-1.3.6/
+-rw-rw-rw-   0        0        0     2779 2024-04-01 14:26:36.124855 tradingcomdados-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2375 2024-03-20 00:11:50.000000 tradingcomdados-1.3.6/README.md
+-rw-rw-rw-   0        0        0      452 2024-04-01 14:26:29.000000 tradingcomdados-1.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 14:26:36.128855 tradingcomdados-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:26:36.112854 tradingcomdados-1.3.6/tradingcomdados/
+-rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.3.6/tradingcomdados/__init__.py
+-rw-rw-rw-   0        0        0     4912 2024-04-01 14:25:36.000000 tradingcomdados-1.3.6/tradingcomdados/alternative_data.py
+-rw-rw-rw-   0        0        0    16846 2024-03-22 13:38:14.000000 tradingcomdados-1.3.6/tradingcomdados/data_provider.py
+-rw-rw-rw-   0        0        0     4470 2024-03-20 00:11:50.000000 tradingcomdados-1.3.6/tradingcomdados/funds_data.py
+-rw-rw-rw-   0        0        0     6915 2023-07-11 00:58:03.000000 tradingcomdados-1.3.6/tradingcomdados/portfolio.py
+-rw-rw-rw-   0        0        0     8924 2024-03-20 00:11:50.000000 tradingcomdados-1.3.6/tradingcomdados/supervised_learning.py
+-rw-rw-rw-   0        0        0    37098 2023-07-02 18:17:22.000000 tradingcomdados-1.3.6/tradingcomdados/ta_indicators.py
+-rw-rw-rw-   0        0        0     6347 2023-06-20 01:15:28.000000 tradingcomdados-1.3.6/tradingcomdados/unsupervised_learning.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:26:36.122854 tradingcomdados-1.3.6/tradingcomdados.egg-info/
+-rw-rw-rw-   0        0        0     2779 2024-04-01 14:26:35.000000 tradingcomdados-1.3.6/tradingcomdados.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2024-04-01 14:26:35.000000 tradingcomdados-1.3.6/tradingcomdados.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 14:26:35.000000 tradingcomdados-1.3.6/tradingcomdados.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2024-04-01 14:26:35.000000 tradingcomdados-1.3.6/tradingcomdados.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-01 14:26:35.000000 tradingcomdados-1.3.6/tradingcomdados.egg-info/top_level.txt
```

### Comparing `tradingcomdados-1.3.5/PKG-INFO` & `tradingcomdados-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingcomdados
-Version: 1.3.5
+Version: 1.3.6
 Summary: tradingcomdados
 Author: Lucas Roberto Correa
 Description-Content-Type: text/markdown
 Requires-Dist: pandas==1.5.3
 Requires-Dist: requests==2.27.1
 Requires-Dist: requests-oauthlib==1.3.1
 Requires-Dist: requests-unixsocket==0.2.0
```

### Comparing `tradingcomdados-1.3.5/README.md` & `tradingcomdados-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.3.5/setup.py` & `tradingcomdados-1.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.3.5/tradingcomdados/alternative_data.py` & `tradingcomdados-1.3.6/tradingcomdados/alternative_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 import pandas as pd
 import requests 
 import zipfile  
 import numpy as np
+import urllib.request
+
+path = 'https://raw.githubusercontent.com/victorncg/financas_quantitativas/main/Data%20Extraction/Stock%20Exchange/Index%20Composition/'
+file = 'backend_index.py'
+
+
+with urllib.request.urlopen(path + file) as response:
+    py_content = response.read().decode('utf-8')
+
+exec(py_content)
 
-# Parsing data from IBOV
 
 
 def _parse_ibov():
 
     try:
 
         url = "https://raw.githubusercontent.com/victorncg/financas_quantitativas/main/IBOV.csv"
@@ -19,100 +28,105 @@
         return df
 
     except:
 
         print("An error occurred while parsing data from IBOV.")
 
 
+
 def _standardize_ibov():
 
     try:
-
         df = _parse_ibov()
         df.columns = list(df.iloc[1])
         df = df[2:][["Código", "Ação", "Tipo", "Qtde. Teórica", "Part. (%)"]]
         df.reset_index(drop=True, inplace=True)
 
         return df
-
     except:
 
         print("An error occurred while manipulating data from IBOV.")
 
 
+
 def _standardize_sp500():
+    """
+    This function fetches the updated composition of the S&P 500 index. 
+    
+    Parameters
+    ----------
+    
+    """
 
     table = pd.read_html("https://en.wikipedia.org/wiki/List_of_S%26P_500_companies")
-
     df = table[0]
 
     return df
 
 
+
 def _adapt_index(
-    index: object, assets: object = "all", mode: object = "df", reduction: bool = True
+    index: object, assets: object = "all", mode: object = "df"
 ):
     """
     This function processes the data from the latest composition of either IBOV or S&P 500. 
     
     Parameters
     ----------
     index : choose the index to be returned, if IBOV or S&P 500
     ativos : you can pass a list with the desired tickets. Default = 'all'.
     mode: you can return either the whole dataframe from B3, or just the list containing the tickers which compose IBOV. Default = 'df'.
-    reduction: you can choose whether the result should come with the reduction and theorical quantitiy provided by B3. Default = True.
     
     """
 
-    if index == "ibov":
-
-        df = _standardize_ibov()
+    if index == "sp500":
 
-        if reduction == False:
-            df = df[:-2]
+        df = _standardize_sp500()
 
         if assets != "all":
-            df = df[df["Código"].isin(assets)]
+            df = df[df["Symbol"].isin(assets)]
 
         if mode == "list":
-            df = list(df.Código)
+            df = list(df.Symbol)
 
-    if index == "sp500":
+    else:
 
-        df = _standardize_sp500()
+        df = return_index(index)
 
         if assets != "all":
-            df = df[df["Symbol"].isin(assets)]
+            df = df[df["cod"].isin(assets)]
 
         if mode == "list":
-            df = list(df.Symbol)
-
+            df = list(df.cod)
+    
     return df
 
 
+
 def index_composition(
-    index: object, assets: object = "all", mode: object = "df", reduction: bool = True
+    index: object, assets: object = "all", mode: object = "df"
 ):
     """
     This function captures the latest composition of either IBOV or S&P 500. It is updated every 4 months.
     
     Parameters
     ----------
     index : choose the index to be returned, if IBOV or S&P 500
     ativos : you can pass a list with the desired tickets. Default = 'all'.
     mode: you can return either the whole dataframe from B3, or just the list containing the tickers which compose IBOV. Default = 'df'.
-    reduction: you can choose whether the result should come with the reduction and theorical quantitiy provided by B3. Default = True.
     
     """
 
-    df = _adapt_index(index, assets, mode, reduction)
+    df = _adapt_index(index, assets, mode)
 
     return df
 
 
+
+
 def get_sectors(ticker:object = None):
     """
     This function get the B3 listed companies' classification into economic and activity sectors.
     You can leave the parameter 'ticker' empty if you wish to return all companies, or 
     specify a ticker without the numbers at the end, for example: "PETR"
     
     Parameters
@@ -154,8 +168,8 @@
     if ticker == None:
         df = df
 
     else:
         ticker = ticker[:4]
         df = df[df['CÓDIGO'] == ticker]
 
-    return df
+    return df
```

### Comparing `tradingcomdados-1.3.5/tradingcomdados/data_provider.py` & `tradingcomdados-1.3.6/tradingcomdados/data_provider.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.3.5/tradingcomdados/funds_data.py` & `tradingcomdados-1.3.6/tradingcomdados/funds_data.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.3.5/tradingcomdados/portfolio.py` & `tradingcomdados-1.3.6/tradingcomdados/portfolio.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.3.5/tradingcomdados/supervised_learning.py` & `tradingcomdados-1.3.6/tradingcomdados/supervised_learning.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.3.5/tradingcomdados/ta_indicators.py` & `tradingcomdados-1.3.6/tradingcomdados/ta_indicators.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.3.5/tradingcomdados/unsupervised_learning.py` & `tradingcomdados-1.3.6/tradingcomdados/unsupervised_learning.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.3.5/tradingcomdados.egg-info/PKG-INFO` & `tradingcomdados-1.3.6/tradingcomdados.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingcomdados
-Version: 1.3.5
+Version: 1.3.6
 Summary: tradingcomdados
 Author: Lucas Roberto Correa
 Description-Content-Type: text/markdown
 Requires-Dist: pandas==1.5.3
 Requires-Dist: requests==2.27.1
 Requires-Dist: requests-oauthlib==1.3.1
 Requires-Dist: requests-unixsocket==0.2.0
```

