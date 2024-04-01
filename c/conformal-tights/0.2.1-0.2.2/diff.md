# Comparing `tmp/conformal_tights-0.2.1.tar.gz` & `tmp/conformal_tights-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conformal_tights-0.2.1.tar", max compression
+gzip compressed data, was "conformal_tights-0.2.2.tar", max compression
```

## Comparing `conformal_tights-0.2.1.tar` & `conformal_tights-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2024-03-31 08:51:13.886067 conformal_tights-0.2.1/LICENSE
--rw-r--r--   0        0        0    10441 2024-03-31 08:51:13.886067 conformal_tights-0.2.1/README.md
--rw-r--r--   0        0        0     4610 2024-03-31 08:51:13.890067 conformal_tights-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      195 2024-03-31 08:51:13.890067 conformal_tights-0.2.1/src/conformal_tights/__init__.py
--rw-r--r--   0        0        0    11652 2024-03-31 08:51:13.890067 conformal_tights-0.2.1/src/conformal_tights/_coherent_linear_quantile_regressor.py
--rw-r--r--   0        0        0    17583 2024-03-31 08:51:13.890067 conformal_tights-0.2.1/src/conformal_tights/_conformal_coherent_quantile_regressor.py
--rw-r--r--   0        0        0      239 2024-03-31 08:51:13.890067 conformal_tights-0.2.1/src/conformal_tights/_typing.py
--rw-r--r--   0        0        0        0 2024-03-31 08:51:13.890067 conformal_tights-0.2.1/src/conformal_tights/py.typed
--rw-r--r--   0        0        0    11168 1970-01-01 00:00:00.000000 conformal_tights-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-01 12:01:19.388492 conformal_tights-0.2.2/LICENSE
+-rw-r--r--   0        0        0    10441 2024-04-01 12:01:19.388492 conformal_tights-0.2.2/README.md
+-rw-r--r--   0        0        0     4656 2024-04-01 12:01:19.388492 conformal_tights-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      195 2024-04-01 12:01:19.388492 conformal_tights-0.2.2/src/conformal_tights/__init__.py
+-rw-r--r--   0        0        0    11652 2024-04-01 12:01:19.388492 conformal_tights-0.2.2/src/conformal_tights/_coherent_linear_quantile_regressor.py
+-rw-r--r--   0        0        0    17582 2024-04-01 12:01:19.388492 conformal_tights-0.2.2/src/conformal_tights/_conformal_coherent_quantile_regressor.py
+-rw-r--r--   0        0        0      239 2024-04-01 12:01:19.388492 conformal_tights-0.2.2/src/conformal_tights/_typing.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:01:19.388492 conformal_tights-0.2.2/src/conformal_tights/py.typed
+-rw-r--r--   0        0        0    11168 1970-01-01 00:00:00.000000 conformal_tights-0.2.2/PKG-INFO
```

### Comparing `conformal_tights-0.2.1/LICENSE` & `conformal_tights-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `conformal_tights-0.2.1/README.md` & `conformal_tights-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `conformal_tights-0.2.1/pyproject.toml` & `conformal_tights-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "conformal-tights"
-version = "0.2.1"
+version = "0.2.2"
 description = "A scikit-learn meta-estimator for computing tight conformal predictions"
 authors = ["Laurent Sorber <laurent@radix.ai>"]
 readme = "README.md"
 repository = "https://github.com/radix-ai/conformal-tights"
 
 [tool.commitizen]  # https://commitizen-tools.github.io/commitizen/config/
 bump_message = "bump(release): v$current_version → v$new_version"
@@ -71,15 +71,15 @@
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 warn_unreachable = true
 
 [tool.pytest.ini_options]  # https://docs.pytest.org/en/latest/reference/reference.html#ini-options-ref
 addopts = "--color=yes --doctest-modules --exitfirst --failed-first --strict-config --strict-markers --verbosity=2 --junitxml=reports/pytest.xml"
-filterwarnings = ["error", "ignore::DeprecationWarning"]
+filterwarnings = ["error", "ignore::DeprecationWarning", "ignore::sklearn.exceptions.SkipTestWarning"]
 testpaths = ["src", "tests"]
 xfail_strict = true
 
 [tool.ruff]  # https://github.com/charliermarsh/ruff
 fix = true
 line-length = 100
 src = ["src", "tests"]
```

### Comparing `conformal_tights-0.2.1/src/conformal_tights/_coherent_linear_quantile_regressor.py` & `conformal_tights-0.2.2/src/conformal_tights/_coherent_linear_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `conformal_tights-0.2.1/src/conformal_tights/_conformal_coherent_quantile_regressor.py` & `conformal_tights-0.2.2/src/conformal_tights/_conformal_coherent_quantile_regressor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Conformal Coherent Quantile Regressor meta-estimator."""
 
-from typing import TYPE_CHECKING, Literal, TypeVar, overload
+from typing import TYPE_CHECKING, Any, Literal, TypeVar, overload
 
 import numpy as np
 import numpy.typing as npt
 from sklearn.base import BaseEstimator, MetaEstimatorMixin, RegressorMixin, clone
 from sklearn.model_selection import train_test_split
 from sklearn.utils.validation import (
     check_array,
@@ -98,16 +98,14 @@
         # Learn dimensionality and dtypes.
         if not hasattr(X, "dtypes"):
             X = np.asarray(X)
         y = np.ravel(np.asarray(y))
         self.n_features_in_: int = X.shape[1]
         self.y_dtype_: npt.DTypeLike = y.dtype  # Used to cast predictions to the correct dtype.
         self.y_is_integer_: bool = bool(np.all(y.astype(np.intp) == y))
-        if self.y_is_integer_:
-            self.y_dtype_ = np.intp  # To satisfy sklearn's `check_regressors_int`.
         y = y.astype(np.float64)  # To support datetime64[ns] and timedelta64[ns].
         if sample_weight is not None:
             check_consistent_length(y, sample_weight)
             sample_weight = np.ravel(np.asarray(sample_weight).astype(np.float64))
         # Use the smallest of the relative and absolute calibration sizes.
         calib_size = min(
             int(self.conformal_calibration_size[0] * X.shape[0]), self.conformal_calibration_size[1]
@@ -272,15 +270,15 @@
         # Choose between the the absolute and relative quantiles for each example in order to
         # minimise the dispersion of the predicted quantiles.
         dispersion = np.std(Δŷ_quantiles, axis=1)
         Δŷ_quantiles = Δŷ_quantiles[
             np.arange(Δŷ_quantiles.shape[0]), :, np.argmin(dispersion, axis=-1)
         ]
         ŷ_quantiles: FloatMatrix[F] = ŷ[:, np.newaxis] + Δŷ_quantiles
-        if self.y_is_integer_:
+        if self.y_is_integer_ and np.issubdtype(self.y_dtype_, np.integer):
             ŷ_quantiles = np.round(ŷ_quantiles)
         ŷ_quantiles = ŷ_quantiles.astype(self.y_dtype_)
         # Convert ŷ_quantiles to a pandas DataFrame if X is a pandas DataFrame.
         if hasattr(X, "dtypes") and hasattr(X, "index"):
             try:
                 import pandas as pd
             except ImportError:
@@ -365,10 +363,10 @@
             except ImportError:
                 pass
             else:
                 ŷ_series = pd.Series(ŷ, index=X.index)
                 return ŷ_series
         return ŷ
 
-    def _more_tags(self) -> dict[str, bool]:
+    def _more_tags(self) -> dict[str, Any]:
         """Return more tags for the estimator."""
-        return {"allow_nan": True}
+        return {"allow_nan": True, "_xfail_checks": {"check_regressors_int": "Incompatible check"}}
```

### Comparing `conformal_tights-0.2.1/PKG-INFO` & `conformal_tights-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conformal-tights
-Version: 0.2.1
+Version: 0.2.2
 Summary: A scikit-learn meta-estimator for computing tight conformal predictions
 Home-page: https://github.com/radix-ai/conformal-tights
 Author: Laurent Sorber
 Author-email: laurent@radix.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

