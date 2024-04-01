# Comparing `tmp/tradeset-0.0.3.tar.gz` & `tmp/tradeset-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradeset-0.0.3.tar", last modified: Sun Mar 31 06:39:48 2024, max compression
+gzip compressed data, was "tradeset-0.0.4.tar", last modified: Mon Apr  1 21:05:26 2024, max compression
```

## Comparing `tradeset-0.0.3.tar` & `tradeset-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 06:39:48.918931 tradeset-0.0.3/
--rw-rw-rw-   0        0        0    11526 2024-03-23 13:41:33.000000 tradeset-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      920 2024-03-31 06:39:48.914932 tradeset-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      167 2024-03-31 06:06:46.000000 tradeset-0.0.3/README.md
--rw-rw-rw-   0        0        0      729 2024-03-31 06:39:21.000000 tradeset-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-31 06:39:48.918931 tradeset-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-31 06:39:48.878932 tradeset-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-03-31 06:39:48.892931 tradeset-0.0.3/src/tradeset/
--rw-rw-rw-   0        0        0      124 2024-03-31 06:36:47.000000 tradeset-0.0.3/src/tradeset/__init__.py
--rw-rw-rw-   0        0        0     7373 2024-03-31 06:35:59.000000 tradeset-0.0.3/src/tradeset/tools.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:39:48.911934 tradeset-0.0.3/src/tradeset.egg-info/
--rw-rw-rw-   0        0        0      920 2024-03-31 06:39:48.000000 tradeset-0.0.3/src/tradeset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-03-31 06:39:48.000000 tradeset-0.0.3/src/tradeset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 06:39:48.000000 tradeset-0.0.3/src/tradeset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-03-31 06:39:48.000000 tradeset-0.0.3/src/tradeset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-31 06:39:48.000000 tradeset-0.0.3/src/tradeset.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 21:05:26.327686 tradeset-0.0.4/
+-rw-rw-rw-   0        0        0    11526 2024-03-29 19:28:02.000000 tradeset-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      916 2024-04-01 21:05:26.324686 tradeset-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2024-04-01 16:27:26.000000 tradeset-0.0.4/README.md
+-rw-rw-rw-   0        0        0      725 2024-04-01 20:59:14.000000 tradeset-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 21:05:26.327686 tradeset-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 21:05:26.258684 tradeset-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 21:05:26.283687 tradeset-0.0.4/src/tradeset/
+-rw-rw-rw-   0        0        0      146 2024-04-01 21:02:11.000000 tradeset-0.0.4/src/tradeset/__init__.py
+-rw-rw-rw-   0        0        0     7929 2024-04-01 21:02:05.000000 tradeset-0.0.4/src/tradeset/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:05:26.323684 tradeset-0.0.4/src/tradeset.egg-info/
+-rw-rw-rw-   0        0        0      916 2024-04-01 21:05:26.000000 tradeset-0.0.4/src/tradeset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-04-01 21:05:26.000000 tradeset-0.0.4/src/tradeset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 21:05:26.000000 tradeset-0.0.4/src/tradeset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-01 21:05:26.000000 tradeset-0.0.4/src/tradeset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-01 21:05:26.000000 tradeset-0.0.4/src/tradeset.egg-info/top_level.txt
```

### Comparing `tradeset-0.0.3/LICENSE` & `tradeset-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tradeset-0.0.3/PKG-INFO` & `tradeset-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tradeset
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tradeset
-Author-email: Mohammad Talaei <mohammadstar1375@gmail.com>, Morteza Omidi <Mortezaomidi24@yahoo.com>
+Author-email: Mohammad Talaei <m.talaei.sut@gmail.com>, Morteza Omidi <mortezaomidi24@yahoo.com>
 Project-URL: Homepage, https://tradeset.ai/
 Project-URL: Documents, https://docs.tradeset.ai/
 Project-URL: Issues, https://github.com/tradeset/tradeset-public/issues/
 Project-URL: Source, https://github.com/tradeset/tradeset-public/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tradeset-0.0.3/pyproject.toml` & `tradeset-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "tradeset"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
-  { name="Mohammad Talaei", email="mohammadstar1375@gmail.com" },
-  { name="Morteza Omidi", email="Mortezaomidi24@yahoo.com" },
+  { name="Mohammad Talaei", email="m.talaei.sut@gmail.com" },
+  { name="Morteza Omidi", email="mortezaomidi24@yahoo.com" },
 ]
 description = "Tradeset"
 readme = "README.md"
 requires-python = ">=3.8"
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `tradeset-0.0.3/src/tradeset/tools.py` & `tradeset-0.0.4/src/tradeset/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+import io
+import gc
 import requests
 import pandas as pd
 from sklearn.model_selection import TimeSeriesSplit
 import time
-from typing import Union 
+from typing import Union, Dict
 import pandas as pd
 import numpy as np
 from sklearn.metrics import classification_report, confusion_matrix
-import gc
 
 
 def create_target(forex_pair:str,
                   trade_mode:str,
                   target_look_ahead:int,
                   target_take_profit:int,
                   target_stop_loss:int,
@@ -64,15 +65,15 @@
 ):
     """
     Return a nested dictionary key is k number and value is dicitonary of train, valid and test Dates
     :max_train_size: maximum size we for train
     :n_splits: K in cross-folds
     :test_size: test size
     """
-    all_dates = df_all.index.get_level_values("_time").unique().sort_values()
+    all_dates = df_all.index.get_level_values("_time").unique().sort_values("_time")
     tscv = TimeSeriesSplit(
         gap = train_test_gap_size,
         max_train_size=max_train_size + test_size,
         n_splits=n_splits,
         test_size=test_size,
     )
     folds = {}
@@ -231,7 +232,19 @@
         print(evals.iloc[-len(folds[i].keys()):])
 
     return (
         evals,
         df[df.model_prediction != -1][["K", "model_prediction", "model_prediction_proba", "target"]],
     )
 
+def backtest_strategy(df_model_signal: pd.DataFrame, strategy_config:Dict[str,Union[int,str]], api_key:str):
+    buffer = io.BytesIO()
+    df_model_signal.to_parquet(buffer)
+    parquet_bytes = buffer.getvalue()
+
+    headers = {"Authorization": api_key}
+
+    # Create files dictionary with in-memory Parquet bytes
+    files = {"df_model_signal_file": ("df_model_signal.parquet", parquet_bytes)}
+
+    res = requests.post("http://127.0.0.1:8001/backtest", headers=headers, params=strategy_config, files=files)
+    return res
```

### Comparing `tradeset-0.0.3/src/tradeset.egg-info/PKG-INFO` & `tradeset-0.0.4/src/tradeset.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tradeset
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tradeset
-Author-email: Mohammad Talaei <mohammadstar1375@gmail.com>, Morteza Omidi <Mortezaomidi24@yahoo.com>
+Author-email: Mohammad Talaei <m.talaei.sut@gmail.com>, Morteza Omidi <mortezaomidi24@yahoo.com>
 Project-URL: Homepage, https://tradeset.ai/
 Project-URL: Documents, https://docs.tradeset.ai/
 Project-URL: Issues, https://github.com/tradeset/tradeset-public/issues/
 Project-URL: Source, https://github.com/tradeset/tradeset-public/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

