# Comparing `tmp/openbb_technical-1.1.4.tar.gz` & `tmp/openbb_technical-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_technical-1.1.4.tar", max compression
+gzip compressed data, was "openbb_technical-1.1.5.tar", max compression
```

## Comparing `openbb_technical-1.1.4.tar` & `openbb_technical-1.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      605 2024-01-17 14:26:16.647950 openbb_technical-1.1.4/README.md
--rw-r--r--   0        0        0       43 2024-01-17 14:26:16.648281 openbb_technical-1.1.4/openbb_technical/__init__.py
--rw-r--r--   0        0        0    16751 2024-03-11 10:41:33.393078 openbb_technical-1.1.4/openbb_technical/helpers.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.648422 openbb_technical-1.1.4/openbb_technical/py.typed
--rw-r--r--   0        0        0    57352 2024-03-11 19:21:12.900290 openbb_technical-1.1.4/openbb_technical/technical_router.py
--rw-r--r--   0        0        0      614 2024-03-11 19:57:51.173566 openbb_technical-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 openbb_technical-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      605 2024-02-29 11:03:36.743618 openbb_technical-1.1.5/README.md
+-rw-r--r--   0        0        0       43 2024-02-29 11:03:36.744125 openbb_technical-1.1.5/openbb_technical/__init__.py
+-rw-r--r--   0        0        0    16751 2024-03-18 09:35:41.446222 openbb_technical-1.1.5/openbb_technical/helpers.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.744320 openbb_technical-1.1.5/openbb_technical/py.typed
+-rw-r--r--   0        0        0    57417 2024-03-25 15:07:22.155086 openbb_technical-1.1.5/openbb_technical/technical_router.py
+-rw-r--r--   0        0        0      614 2024-04-01 14:19:25.552681 openbb_technical-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 openbb_technical-1.1.5/PKG-INFO
```

### Comparing `openbb_technical-1.1.4/README.md` & `openbb_technical-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `openbb_technical-1.1.4/openbb_technical/helpers.py` & `openbb_technical-1.1.5/openbb_technical/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,20 +379,20 @@
 
 def calculate_cones(
     data: pd.DataFrame,
     lower_q: float,
     upper_q: float,
     is_crypto: bool,
     model: Literal[
-        "STD",
-        "Parkinson",
-        "Garman-Klass",
-        "Hodges-Tompkins",
-        "Rogers-Satchell",
-        "Yang-Zhang",
+        "std",
+        "parkinson",
+        "garman_klass",
+        "hodges_tompkins",
+        "rogers_satchell",
+        "yang_zhang",
     ],
     trading_periods: Optional[int] = None,
 ) -> pd.DataFrame:
     """Calculate Cones."""
     estimator = pd.DataFrame()
 
     if lower_q > upper_q:
@@ -411,20 +411,20 @@
     top_q = []
     bottom_q = []
     realized = []
     allowed_windows = []
     data = data.sort_index(ascending=True)
 
     model_functions = {
-        "STD": standard_deviation,
-        "Parkinson": parkinson,
-        "Garman-Klass": garman_klass,
-        "Hodges-Tompkins": hodges_tompkins,
-        "Rogers-Satchell": rogers_satchell,
-        "Yang-Zhang": yang_zhang,
+        "std": standard_deviation,
+        "parkinson": parkinson,
+        "garman_klass": garman_klass,
+        "hodges_tompkins": hodges_tompkins,
+        "rogers_satchell": rogers_satchell,
+        "yang_zhang": yang_zhang,
     }
 
     for window in windows:
         estimator = model_functions[model](  # type: ignore
             window=window,
             data=data,
             is_crypto=is_crypto,
```

### Comparing `openbb_technical-1.1.4/openbb_technical/technical_router.py` & `openbb_technical-1.1.5/openbb_technical/technical_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,14 +311,15 @@
         Number of periods to be used for the slow calculation, by default 10.
     offset : int, optional
         Offset to be used for the calculation, by default 0.
 
     Returns
     -------
     OBBject[List[Data]]
+        The calculated data.
     """
     validate_data(data, [fast, slow])
     df = basemodel_to_df(data, index=index)
     df_target = get_target_columns(df, ["open", "high", "low", "close", "volume"])
     df_adosc = pd.DataFrame(df_target.ta.adosc(fast=fast, slow=slow, offset=offset))
 
     output = pd.concat([df, df_adosc], axis=1)
@@ -1089,14 +1090,15 @@
         Index column name to use with `data`, by default "date".
     offset : int, optional
         Offset of the AD, by default 0.
 
     Returns
     -------
     OBBject[List[Data]]
+        The calculated data.
     """
     df = basemodel_to_df(data, index=index)
     df_target = get_target_columns(df, ["high", "low", "close", "volume"])
     ad_df = pd.DataFrame(df_target.ta.ad(offset=offset).dropna())
 
     output = pd.concat([df, ad_df], axis=1)
     results = df_to_basemodel(output.reset_index())
@@ -1524,36 +1526,36 @@
     return OBBject(results=results)
 
 
 @router.command(
     methods=["POST"],
     examples=[
         PythonEx(
-            description="Get the cones indicator.",
+            description="Realized Volatility Cones.",
             code=[
-                "stock_data = obb.equity.price.historical(symbol='TSLA', start_date='2023-01-01', provider='fmp')",
-                "cones_data = obb.technical.cones(data=stock_data.results, lower_q=0.25, upper_q=0.75, model='STD')",
+                "stock_data = obb.equity.price.historical(symbol='TSLA', start_date='2023-01-01', provider='yfinance')",
+                "cones_data = obb.technical.cones(data=stock_data.results, lower_q=0.25, upper_q=0.75, model='std')",
             ],
         ),
         APIEx(parameters={"data": APIEx.mock_data("timeseries")}),
     ],
 )
 def cones(
     data: List[Data],
     index: str = "date",
     lower_q: float = 0.25,
     upper_q: float = 0.75,
     model: Literal[
-        "STD",
-        "Parkinson",
-        "Garman-Klass",
-        "Hodges-Tompkins",
-        "Rogers-Satchell",
-        "Yang-Zhang",
-    ] = "STD",
+        "std",
+        "parkinson",
+        "garman_klass",
+        "hodges_tompkins",
+        "rogers_satchell",
+        "yang_zhang",
+    ] = "std",
     is_crypto: bool = False,
     trading_periods: Optional[int] = None,
 ) -> OBBject[List[Data]]:
     """Calculate the realized volatility quantiles over rolling windows of time.
 
     The cones indicator is designed to map out the ebb and flow of price movements through a detailed analysis of
     volatility quantiles. By examining the range of volatility within specific time frames, it offers a nuanced view of
@@ -1575,15 +1577,15 @@
         The data to use for the calculation.
     index : str, optional
         Index column name to use with `data`, by default "date"
     lower_q : float, optional
         The lower quantile value for calculations
     upper_q : float, optional
         The upper quantile value for calculations
-    model : Literal["STD", "Parkinson", "Garman-Klass", "Hodges-Tompkins", "Rogers-Satchell", "Yang-Zhang"], optional
+    model : Literal["std", "parkinson", "garman_klass", "hodges_tompkins", "rogers_satchell", "yang_zhang"], optional
         The model used to calculate realized volatility
 
             Standard deviation measures how widely returns are dispersed from the average return.
             It is the most common (and biased) estimator of volatility.
 
             Parkinson volatility uses the high and low price of the day rather than just close to close prices.
             It is useful for capturing large price movements during the day.
```

### Comparing `openbb_technical-1.1.4/pyproject.toml` & `openbb_technical-1.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "openbb-technical"
-version = "1.1.4"
+version = "1.1.5"
 description = "Technical Analysis extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 readme = "README.md"
 packages = [{ include = "openbb_technical" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"  # scipy forces python <4.0 explicitly
 scipy = "^1.10.1"
 statsmodels = "^0.14.0"
 scikit-learn = "^1.3.1"
 pandas-ta = "^0.3.14b"
-openbb-core = "^1.1.3"
+openbb-core = "^1.1.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_core_extension"]
 technical = "openbb_technical.technical_router:router"
```

### Comparing `openbb_technical-1.1.4/PKG-INFO` & `openbb_technical-1.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: openbb-technical
-Version: 1.1.4
+Version: 1.1.5
 Summary: Technical Analysis extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openbb-core (>=1.1.3,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
 Requires-Dist: pandas-ta (>=0.3.14b,<0.4.0)
 Requires-Dist: scikit-learn (>=1.3.1,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Technical Analysis Extension
```

