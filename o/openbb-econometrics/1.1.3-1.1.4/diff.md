# Comparing `tmp/openbb_econometrics-1.1.3.tar.gz` & `tmp/openbb_econometrics-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_econometrics-1.1.3.tar", max compression
+gzip compressed data, was "openbb_econometrics-1.1.4.tar", max compression
```

## Comparing `openbb_econometrics-1.1.3.tar` & `openbb_econometrics-1.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      448 2024-01-17 14:26:16.635901 openbb_econometrics-1.1.3/README.md
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.636169 openbb_econometrics-1.1.3/openbb_econometrics/__init__.py
--rw-r--r--   0        0        0    28122 2024-03-11 19:21:12.899263 openbb_econometrics-1.1.3/openbb_econometrics/econometrics_router.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.636336 openbb_econometrics-1.1.3/openbb_econometrics/py.typed
--rw-r--r--   0        0        0     4036 2024-01-17 14:26:16.636410 openbb_econometrics-1.1.3/openbb_econometrics/utils.py
--rw-r--r--   0        0        0      689 2024-03-11 19:56:56.180788 openbb_econometrics-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1126 1970-01-01 00:00:00.000000 openbb_econometrics-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      448 2024-02-29 11:03:36.733012 openbb_econometrics-1.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.733220 openbb_econometrics-1.1.4/openbb_econometrics/__init__.py
+-rw-r--r--   0        0        0    28108 2024-03-14 20:24:16.775321 openbb_econometrics-1.1.4/openbb_econometrics/econometrics_router.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.733411 openbb_econometrics-1.1.4/openbb_econometrics/py.typed
+-rw-r--r--   0        0        0     4036 2024-02-29 11:03:36.733509 openbb_econometrics-1.1.4/openbb_econometrics/utils.py
+-rw-r--r--   0        0        0      689 2024-04-01 14:18:35.488207 openbb_econometrics-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1126 1970-01-01 00:00:00.000000 openbb_econometrics-1.1.4/PKG-INFO
```

### Comparing `openbb_econometrics-1.1.3/openbb_econometrics/econometrics_router.py` & `openbb_econometrics-1.1.4/openbb_econometrics/econometrics_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     Parameters
     ----------
     data : List[Data]
         Input dataset.
 
     Returns
     -------
-    OBBject[List[Data]]:
+    OBBject[List[Data]]
         Correlation matrix.
     """
     df = basemodel_to_df(data)
     # remove non float columns from the dataframe to perform the correlation
     df = df.select_dtypes(include=["float64"])
 
     corr = df.corr()
@@ -116,15 +116,15 @@
     y_column: str
         Target column.
     x_columns: List[str]
         List of columns to use as exogenous variables.
 
     Returns
     -------
-    OBBject[Dict]:
+    OBBject[Dict]
         OBBject with the results being model and results objects.
     """
     X = sm.add_constant(get_target_columns(basemodel_to_df(data), x_columns))
     y = get_target_column(basemodel_to_df(data), y_column)
     model = sm.OLS(y, X)
     results = model.fit()
     return OBBject(results={"model": model, "results": results})
@@ -165,15 +165,15 @@
     y_column: str
         Target column.
     x_columns: List[str]
         List of columns to use as exogenous variables.
 
     Returns
     -------
-    OBBject[Data]:
+    OBBject[Data]
         OBBject with the results being summary object.
     """
     X = sm.add_constant(get_target_columns(basemodel_to_df(data), x_columns))
     y = get_target_column(basemodel_to_df(data), y_column)
 
     try:
         X = X.astype(float)
@@ -256,15 +256,15 @@
     y_column: str
         Target column.
     x_columns: List[str]
         List of columns to use as exogenous variables.
 
     Returns
     -------
-    OBBject[Dict]:
+    OBBject[Dict]
         OBBject with the results being the score from the test.
     """
     X = sm.add_constant(get_target_columns(basemodel_to_df(data), x_columns))
     y = get_target_column(basemodel_to_df(data), y_column)
     results = sm.OLS(y, X).fit()
     return OBBject(results=Data(score=durbin_watson(results.resid)))
 
@@ -313,15 +313,15 @@
     x_columns: List[str]
         List of columns to use as exogenous variables.
     lags: PositiveInt
         Number of lags to use in the test.
 
     Returns
     -------
-    OBBject[Data]:
+    OBBject[Data]
         OBBject with the results being the score from the test.
     """
     X = sm.add_constant(get_target_columns(basemodel_to_df(data), x_columns))
     y = get_target_column(basemodel_to_df(data), y_column)
     model = sm.OLS(y, X)
     results = model.fit()
     lm_stat, p_value, f_stat, fp_value = acorr_breusch_godfrey(results, nlags=lags)
@@ -370,15 +370,15 @@
     columns: List[str]
         Data columns to check cointegration
     maxlag: PositiveInt
         Number of lags to use in the test.
 
     Returns
     -------
-    OBBject[Data]:
+    OBBject[Data]
         OBBject with the results being the score from the test.
     """
     pairs = list(combinations(columns, 2))
     dataset = get_target_columns(basemodel_to_df(data), columns)
     result = {}
     for x, y in pairs:
         (
@@ -446,15 +446,15 @@
     x_column: str
         Columns to use as exogenous variables.
     lag: PositiveInt
         Number of lags to use in the test.
 
     Returns
     -------
-    OBBject[Data]:
+    OBBject[Data]
         OBBject with the results being the score from the test.
     """
     X = get_target_column(basemodel_to_df(data), x_column)
     y = get_target_column(basemodel_to_df(data), y_column)
 
     granger = grangercausalitytests(pd.concat([y, X], axis=1), [lag], verbose=False)
 
@@ -514,15 +514,15 @@
         Data columns to check unit root
     regression: Literal["c", "ct", "ctt"]
         Regression type to use in the test.  Either "c" for constant only, "ct" for constant and trend, or "ctt" for
         constant, trend, and trend-squared.
 
     Returns
     -------
-    OBBject[Data]:
+    OBBject[Data]
         OBBject with the results being the score from the test.
     """
     dataset = get_target_column(basemodel_to_df(data), column)
     adfstat, pvalue, usedlag, nobs, _, icbest = adfuller(dataset, regression=regression)
     results = {
         "adfstat": adfstat,
         "pvalue": pvalue,
@@ -564,15 +564,15 @@
     y_column: str
         Target column.
     x_columns: List[str]
         List of columns to use as exogenous variables.
 
     Returns
     -------
-    OBBject[Dict]:
+    OBBject[Dict]
         OBBject with the fit model returned
     """
     X = get_target_columns(basemodel_to_df(data), x_columns)
     if len(X) < 3:
         raise ValueError("This analysis requires at least 3 items in the dataset.")
     y = get_target_column(basemodel_to_df(data), y_column)
     exogenous = sm.add_constant(X)
@@ -611,15 +611,15 @@
     y_column: str
         Target column.
     x_columns: List[str]
         List of columns to use as exogenous variables.
 
     Returns
     -------
-    OBBject[Dict]:
+    OBBject[Dict]
         OBBject with the fit model returned
     """
     X = get_target_columns(basemodel_to_df(data), x_columns)
     y = get_target_column(basemodel_to_df(data), y_column)
     exogenous = sm.add_constant(X)
     results = BetweenOLS(y, exogenous).fit()
     return OBBject(results={"results": results})
@@ -657,15 +657,15 @@
     y_column: str
         Target column.
     x_columns: List[str]
         List of columns to use as exogenous variables.
 
     Returns
     -------
-    OBBject[Dict]:
+    OBBject[Dict]
         OBBject with the fit model returned
     """
     X = get_target_columns(basemodel_to_df(data), x_columns)
     y = get_target_column(basemodel_to_df(data), y_column)
     exogenous = sm.add_constant(X)
     results = PooledOLS(y, exogenous).fit()
     return OBBject(results={"results": results})
@@ -702,15 +702,15 @@
     y_column: str
         Target column.
     x_columns: List[str]
         List of columns to use as exogenous variables.
 
     Returns
     -------
-    OBBject[Dict]:
+    OBBject[Dict]
         OBBject with the fit model returned
     """
     X = get_target_columns(basemodel_to_df(data), x_columns)
     y = get_target_column(basemodel_to_df(data), y_column)
     exogenous = sm.add_constant(X)
     results = PanelOLS(y, exogenous).fit()
     return OBBject(results={"results": results})
@@ -747,15 +747,15 @@
     y_column: str
         Target column.
     x_columns: List[str]
         List of columns to use as exogenous variables.
 
     Returns
     -------
-    OBBject[Dict]:
+    OBBject[Dict]
         OBBject with the fit model returned
     """
     X = get_target_columns(basemodel_to_df(data), x_columns)
     y = get_target_column(basemodel_to_df(data), y_column)
     exogenous = X
     results = FirstDifferenceOLS(y, exogenous).fit()
     return OBBject(results={"results": results})
@@ -793,15 +793,15 @@
     y_column: str
         Target column.
     x_columns: List[str]
         List of columns to use as exogenous variables.
 
     Returns
     -------
-    OBBject[Dict]:
+    OBBject[Dict]
         OBBject with the fit model returned
     """
     X = get_target_columns(basemodel_to_df(data), x_columns)
     y = get_target_column(basemodel_to_df(data), y_column)
     exogenous = sm.add_constant(X)
     results = FamaMacBeth(y, exogenous).fit()
     return OBBject(results={"results": results})
```

### Comparing `openbb_econometrics-1.1.3/openbb_econometrics/utils.py` & `openbb_econometrics-1.1.4/openbb_econometrics/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_econometrics-1.1.3/pyproject.toml` & `openbb_econometrics-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "openbb-econometrics"
-version = "1.1.3"
+version = "1.1.4"
 description = "Econometrics Toolkit for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 readme = "README.md"
 packages = [{ include = "openbb_econometrics" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"                 # scipy forces python <4.0 explicitly
 scipy = "^1.10.1"
 statsmodels = "^0.14.0"
 arch = "^5.5.0"
 linearmodels = "<=4.25"                # ^4.26 has setuptools-scm in setup_requires
-openbb-core = "^1.1.3"
+openbb-core = "^1.1.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_core_extension"]
 econometrics = "openbb_econometrics.econometrics_router:router"
```

### Comparing `openbb_econometrics-1.1.3/PKG-INFO` & `openbb_econometrics-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: openbb-econometrics
-Version: 1.1.3
+Version: 1.1.4
 Summary: Econometrics Toolkit for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arch (>=5.5.0,<6.0.0)
 Requires-Dist: linearmodels (<=4.25)
-Requires-Dist: openbb-core (>=1.1.3,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
 # Econometrics extension for OpenBB Platform
 
 This extension provides a set of econometrics tools.
```

