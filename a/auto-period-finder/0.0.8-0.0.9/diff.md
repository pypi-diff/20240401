# Comparing `tmp/auto_period_finder-0.0.8.tar.gz` & `tmp/auto_period_finder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_period_finder-0.0.8.tar", max compression
+gzip compressed data, was "auto_period_finder-0.0.9.tar", max compression
```

## Comparing `auto_period_finder-0.0.8.tar` & `auto_period_finder-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-12-26 19:34:13.552040 auto_period_finder-0.0.8/LICENSE
--rw-r--r--   0        0        0     5689 2023-12-26 19:34:13.552040 auto_period_finder-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-12-26 19:34:13.556040 auto_period_finder-0.0.8/auto_period_finder/__init__.py
--rw-r--r--   0        0        0     8207 2023-12-26 19:34:13.556040 auto_period_finder-0.0.8/auto_period_finder/finder.py
--rw-r--r--   0        0        0      455 2023-12-26 19:34:13.556040 auto_period_finder-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6230 1970-01-01 00:00:00.000000 auto_period_finder-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-01 15:26:09.461456 auto_period_finder-0.0.9/LICENSE
+-rw-r--r--   0        0        0     5726 2024-04-01 15:26:09.461456 auto_period_finder-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-01 15:26:09.465456 auto_period_finder-0.0.9/auto_period_finder/__init__.py
+-rw-r--r--   0        0        0    12285 2024-04-01 15:26:09.465456 auto_period_finder-0.0.9/auto_period_finder/finder.py
+-rw-r--r--   0        0        0      455 2024-04-01 15:26:09.465456 auto_period_finder-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6267 1970-01-01 00:00:00.000000 auto_period_finder-0.0.9/PKG-INFO
```

### Comparing `auto_period_finder-0.0.8/LICENSE` & `auto_period_finder-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_period_finder-0.0.8/README.md` & `auto_period_finder-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 ```
 5. You can run tests using the command:
 ```shell
 poetry run pytest
 ```
 6. To export the list detailed list of dependencies, run the following command:
 ```shell
+poetry self add poetry-plugin-export
 poetry export --output requirements.txt
 ```
 
 ## ACF-Based Seasonality Period Detection Explained
 An easy and quick way to find seasonality periods of a univariate time series is to check its autocorrelation function (ACF) and look for specific charecteristics in lag values that we will detail in a second. You can read more information about time series ACF [here](https://otexts.com/fpp3/acf.html), but intuitively, An autocorrelation coefficient $r_k$ measures the the linear relationship between $k$-lagged values of a given time series. In simpler terms, $r_k$ measures how similar/dissimilar time series values that $k$-length apart from each other. The set of $r_k$ values for each lag $k$ makes ACF. Equipped with this information, I developed a package for finding time series seasonality periods automatically using ACF information.
 
 Simply put, given a univariate time series $T$, the algorithm finds, iteratively, lag values $k$ such that:
```

### Comparing `auto_period_finder-0.0.8/PKG-INFO` & `auto_period_finder-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-period-finder
-Version: 0.0.8
+Version: 0.0.9
 Summary: An autocorrelation function-based seasonality periods automatic finder for univariate time series.
 Author: Iskander Gaba
 Author-email: iskander@hey.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -74,14 +74,15 @@
 ```
 5. You can run tests using the command:
 ```shell
 poetry run pytest
 ```
 6. To export the list detailed list of dependencies, run the following command:
 ```shell
+poetry self add poetry-plugin-export
 poetry export --output requirements.txt
 ```
 
 ## ACF-Based Seasonality Period Detection Explained
 An easy and quick way to find seasonality periods of a univariate time series is to check its autocorrelation function (ACF) and look for specific charecteristics in lag values that we will detail in a second. You can read more information about time series ACF [here](https://otexts.com/fpp3/acf.html), but intuitively, An autocorrelation coefficient $r_k$ measures the the linear relationship between $k$-lagged values of a given time series. In simpler terms, $r_k$ measures how similar/dissimilar time series values that $k$-length apart from each other. The set of $r_k$ values for each lag $k$ makes ACF. Equipped with this information, I developed a package for finding time series seasonality periods automatically using ACF information.
 
 Simply put, given a univariate time series $T$, the algorithm finds, iteratively, lag values $k$ such that:
```

