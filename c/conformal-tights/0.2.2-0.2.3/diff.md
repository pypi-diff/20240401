# Comparing `tmp/conformal_tights-0.2.2.tar.gz` & `tmp/conformal_tights-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conformal_tights-0.2.2.tar", max compression
+gzip compressed data, was "conformal_tights-0.2.3.tar", max compression
```

## Comparing `conformal_tights-0.2.2.tar` & `conformal_tights-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2024-04-01 12:01:19.388492 conformal_tights-0.2.2/LICENSE
--rw-r--r--   0        0        0    10441 2024-04-01 12:01:19.388492 conformal_tights-0.2.2/README.md
--rw-r--r--   0        0        0     4656 2024-04-01 12:01:19.388492 conformal_tights-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      195 2024-04-01 12:01:19.388492 conformal_tights-0.2.2/src/conformal_tights/__init__.py
--rw-r--r--   0        0        0    11652 2024-04-01 12:01:19.388492 conformal_tights-0.2.2/src/conformal_tights/_coherent_linear_quantile_regressor.py
--rw-r--r--   0        0        0    17582 2024-04-01 12:01:19.388492 conformal_tights-0.2.2/src/conformal_tights/_conformal_coherent_quantile_regressor.py
--rw-r--r--   0        0        0      239 2024-04-01 12:01:19.388492 conformal_tights-0.2.2/src/conformal_tights/_typing.py
--rw-r--r--   0        0        0        0 2024-04-01 12:01:19.388492 conformal_tights-0.2.2/src/conformal_tights/py.typed
--rw-r--r--   0        0        0    11168 1970-01-01 00:00:00.000000 conformal_tights-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-01 12:50:03.022235 conformal_tights-0.2.3/LICENSE
+-rw-r--r--   0        0        0    10441 2024-04-01 12:50:03.022235 conformal_tights-0.2.3/README.md
+-rw-r--r--   0        0        0     4656 2024-04-01 12:50:03.026235 conformal_tights-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      195 2024-04-01 12:50:03.026235 conformal_tights-0.2.3/src/conformal_tights/__init__.py
+-rw-r--r--   0        0        0    11839 2024-04-01 12:50:03.026235 conformal_tights-0.2.3/src/conformal_tights/_coherent_linear_quantile_regressor.py
+-rw-r--r--   0        0        0    17582 2024-04-01 12:50:03.026235 conformal_tights-0.2.3/src/conformal_tights/_conformal_coherent_quantile_regressor.py
+-rw-r--r--   0        0        0      239 2024-04-01 12:50:03.026235 conformal_tights-0.2.3/src/conformal_tights/_typing.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:50:03.026235 conformal_tights-0.2.3/src/conformal_tights/py.typed
+-rw-r--r--   0        0        0    11168 1970-01-01 00:00:00.000000 conformal_tights-0.2.3/PKG-INFO
```

### Comparing `conformal_tights-0.2.2/LICENSE` & `conformal_tights-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `conformal_tights-0.2.2/README.md` & `conformal_tights-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `conformal_tights-0.2.2/pyproject.toml` & `conformal_tights-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "conformal-tights"
-version = "0.2.2"
+version = "0.2.3"
 description = "A scikit-learn meta-estimator for computing tight conformal predictions"
 authors = ["Laurent Sorber <laurent@radix.ai>"]
 readme = "README.md"
 repository = "https://github.com/radix-ai/conformal-tights"
 
 [tool.commitizen]  # https://commitizen-tools.github.io/commitizen/config/
 bump_message = "bump(release): v$current_version → v$new_version"
```

### Comparing `conformal_tights-0.2.2/src/conformal_tights/_coherent_linear_quantile_regressor.py` & `conformal_tights-0.2.3/src/conformal_tights/_coherent_linear_quantile_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,21 +212,21 @@
     def fit(
         self, X: FloatMatrix[F], y: FloatVector[F], *, sample_weight: FloatVector[F] | None = None
     ) -> "CoherentLinearQuantileRegressor":
         """Fit this predictor."""
         # Validate input.
         X, y = check_X_y(X, y, y_numeric=True)
         self.n_features_in_: int = X.shape[1]
-        self.y_dtype_: npt.DTypeLike = y.dtype  # Used to cast predictions to the correct dtype.
-        if np.all(y.astype(np.intp) == y):
-            self.y_dtype_ = np.intp  # To satisfy sklearn's `check_regressors_int`.
-        y = y.astype(np.float64)  # To support datetime64[ns] and timedelta64[ns].
+        self.y_dtype_: npt.DTypeLike = (  # Used to cast predictions to the correct dtype.
+            X.dtype if np.issubdtype(y.dtype, np.integer) else y.dtype
+        )
+        X, y = X.astype(np.float64), y.astype(np.float64)  # To support datetime64 and timedelta64.
         if sample_weight is not None:
             check_consistent_length(y, sample_weight)
-            sample_weight = np.asarray(sample_weight).astype(np.float64)
+            sample_weight = np.asarray(sample_weight).astype(y.dtype)
         # Add a constant column to X to allow for a bias in the regression.
         if self.fit_intercept:
             X = np.hstack([X, np.ones((X.shape[0], 1), dtype=X.dtype)])
         # Fit the coherent quantile regression model.
         self.β_, self.β_full_ = coherent_linear_quantile_regression(
             X,
             y,
@@ -236,26 +236,31 @@
         )
         return self
 
     def predict(self, X: FloatMatrix[F]) -> FloatMatrix[F]:
         """Predict the output on a given dataset."""
         # Check input.
         check_is_fitted(self)
-        X = check_array(X)
+        X = check_array(X, dtype=np.float64)
         # Add a constant column to X to allow for a bias in the regression.
         if self.fit_intercept:
             X = np.hstack([X, np.ones((X.shape[0], 1), dtype=X.dtype)])
         # Predict the output.
         ŷ: FloatMatrix[F] = X @ self.β_
         # Map back to the training target dtype.
-        ŷ = np.squeeze(ŷ.astype(self.y_dtype_), axis=1 if ŷ.shape[1] == 1 else ())
+        ŷ = np.squeeze(ŷ, axis=1 if ŷ.shape[1] == 1 else ())
+        if not np.issubdtype(self.y_dtype_, np.integer):
+            ŷ.astype(self.y_dtype_)
         return ŷ
 
     def intercept_clip(self, X: FloatMatrix[F], y: FloatVector[F]) -> FloatMatrix[F]:
         """Compute a clip for a delta on the intercept that retains quantile coherence."""
+        check_is_fitted(self)
+        X, y = check_X_y(X, y, y_numeric=True)
+        X, y = X.astype(np.float64), y.astype(np.float64)
         if self.fit_intercept:
             X = np.hstack([X, np.ones((X.shape[0], 1), dtype=X.dtype)])
         Q = X @ self.β_full_ - y[:, np.newaxis]
         β_intercept_clip = np.vstack(
             [
                 np.insert(np.max(Q[:, :-1] - Q[:, 1:], axis=0), 0, -np.inf),
                 np.append(np.min(Q[:, 1:] - Q[:, :-1], axis=0), np.inf),
```

### Comparing `conformal_tights-0.2.2/src/conformal_tights/_conformal_coherent_quantile_regressor.py` & `conformal_tights-0.2.3/src/conformal_tights/_conformal_coherent_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `conformal_tights-0.2.2/PKG-INFO` & `conformal_tights-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conformal-tights
-Version: 0.2.2
+Version: 0.2.3
 Summary: A scikit-learn meta-estimator for computing tight conformal predictions
 Home-page: https://github.com/radix-ai/conformal-tights
 Author: Laurent Sorber
 Author-email: laurent@radix.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

