# Comparing `tmp/neo_ls_svm-0.2.0.tar.gz` & `tmp/neo_ls_svm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo_ls_svm-0.2.0.tar", max compression
+gzip compressed data, was "neo_ls_svm-0.3.0.tar", max compression
```

## Comparing `neo_ls_svm-0.2.0.tar` & `neo_ls_svm-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1071 2024-02-25 15:15:18.461865 neo_ls_svm-0.2.0/LICENSE
--rw-r--r--   0        0        0    13935 2024-02-25 15:15:18.461865 neo_ls_svm-0.2.0/README.md
--rw-r--r--   0        0        0     4624 2024-02-25 15:15:18.461865 neo_ls_svm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       95 2024-02-25 15:15:18.461865 neo_ls_svm-0.2.0/src/neo_ls_svm/__init__.py
--rw-r--r--   0        0        0     5487 2024-02-25 15:15:18.461865 neo_ls_svm-0.2.0/src/neo_ls_svm/_affine_feature_map.py
--rw-r--r--   0        0        0     5580 2024-02-25 15:15:18.461865 neo_ls_svm-0.2.0/src/neo_ls_svm/_affine_normalizer.py
--rw-r--r--   0        0        0     9656 2024-02-25 15:15:18.461865 neo_ls_svm-0.2.0/src/neo_ls_svm/_affine_separator.py
--rw-r--r--   0        0        0     9993 2024-02-25 15:15:18.461865 neo_ls_svm-0.2.0/src/neo_ls_svm/_feature_maps.py
--rw-r--r--   0        0        0    28250 2024-02-25 15:15:18.461865 neo_ls_svm-0.2.0/src/neo_ls_svm/_neo_ls_svm.py
--rw-r--r--   0        0        0    11452 2024-02-25 15:15:18.461865 neo_ls_svm-0.2.0/src/neo_ls_svm/_quantizer.py
--rw-r--r--   0        0        0     1070 2024-02-25 15:15:18.461865 neo_ls_svm-0.2.0/src/neo_ls_svm/_typing.py
--rw-r--r--   0        0        0     2830 2024-02-25 15:15:18.461865 neo_ls_svm-0.2.0/src/neo_ls_svm/_weighted_quantile.py
--rw-r--r--   0        0        0        0 2024-02-25 15:15:18.461865 neo_ls_svm-0.2.0/src/neo_ls_svm/py.typed
--rw-r--r--   0        0        0    14588 1970-01-01 00:00:00.000000 neo_ls_svm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-01 19:58:02.805134 neo_ls_svm-0.3.0/LICENSE
+-rw-r--r--   0        0        0    15760 2024-04-01 19:58:02.805134 neo_ls_svm-0.3.0/README.md
+-rw-r--r--   0        0        0     4624 2024-04-01 19:58:02.809134 neo_ls_svm-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       95 2024-04-01 19:58:02.809134 neo_ls_svm-0.3.0/src/neo_ls_svm/__init__.py
+-rw-r--r--   0        0        0     5487 2024-04-01 19:58:02.809134 neo_ls_svm-0.3.0/src/neo_ls_svm/_affine_feature_map.py
+-rw-r--r--   0        0        0     5580 2024-04-01 19:58:02.809134 neo_ls_svm-0.3.0/src/neo_ls_svm/_affine_normalizer.py
+-rw-r--r--   0        0        0     9656 2024-04-01 19:58:02.809134 neo_ls_svm-0.3.0/src/neo_ls_svm/_affine_separator.py
+-rw-r--r--   0        0        0    11964 2024-04-01 19:58:02.809134 neo_ls_svm-0.3.0/src/neo_ls_svm/_coherent_linear_quantile_regressor.py
+-rw-r--r--   0        0        0     9993 2024-04-01 19:58:02.809134 neo_ls_svm-0.3.0/src/neo_ls_svm/_feature_maps.py
+-rw-r--r--   0        0        0    38959 2024-04-01 19:58:02.809134 neo_ls_svm-0.3.0/src/neo_ls_svm/_neo_ls_svm.py
+-rw-r--r--   0        0        0    11452 2024-04-01 19:58:02.809134 neo_ls_svm-0.3.0/src/neo_ls_svm/_quantizer.py
+-rw-r--r--   0        0        0     1070 2024-04-01 19:58:02.809134 neo_ls_svm-0.3.0/src/neo_ls_svm/_typing.py
+-rw-r--r--   0        0        0     2830 2024-04-01 19:58:02.809134 neo_ls_svm-0.3.0/src/neo_ls_svm/_weighted_quantile.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:58:02.809134 neo_ls_svm-0.3.0/src/neo_ls_svm/py.typed
+-rw-r--r--   0        0        0    16413 1970-01-01 00:00:00.000000 neo_ls_svm-0.3.0/PKG-INFO
```

### Comparing `neo_ls_svm-0.2.0/LICENSE` & `neo_ls_svm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neo_ls_svm-0.2.0/README.md` & `neo_ls_svm-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [![Open in Dev Containers](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/lsorber/neo-ls-svm) [![Open in GitHub Codespaces](https://img.shields.io/static/v1?label=GitHub%20Codespaces&message=Open&color=blue&logo=github)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=739301655)
 
 # Neo LS-SVM
 
 Neo LS-SVM is a modern [Least-Squares Support Vector Machine](https://en.wikipedia.org/wiki/Least-squares_support_vector_machine) implementation in Python that offers several benefits over sklearn's classic `sklearn.svm.SVC` classifier and `sklearn.svm.SVR` regressor:
 
 1. ⚡ Linear complexity in the number of training examples with [Orthogonal Random Features](https://arxiv.org/abs/1610.09072).
-2. 🚀 Hyperparameter free: zero-cost optimization of the regularisation parameter γ and kernel parameter σ.
+2. 🚀 Hyperparameter free: zero-cost optimization of the [regularisation parameter γ](https://en.wikipedia.org/wiki/Ridge_regression#Tikhonov_regularization) and [kernel parameter σ](https://en.wikipedia.org/wiki/Radial_basis_function_kernel).
 3. 🏔️ Adds a new tertiary objective that minimizes the complexity of the prediction surface.
 4. 🎁 Returns the leave-one-out residuals and error for free after fitting.
 5. 🌀 Learns an affine transformation of the feature matrix to optimally separate the target's bins.
 6. 🪞 Can solve the LS-SVM both in the primal and dual space.
-7. 🌡️ Isotonically calibrated `predict_proba` based on the leave-one-out predictions.
-8. 🎲 Asymmetric conformal Bayesian confidence intervals for classification and regression.
+7. 🌡️ Isotonically calibrated `predict_proba`.
+8. ✅ Conformally calibrated `predict_quantiles` and `predict_interval`.
+9. 🔔 Bayesian estimation of the predictive standard deviation with `predict_std`.
+10. 🐼 Pandas DataFrame output when the input is a pandas DataFrame.
 
 ## Using
 
 ### Installing
 
 First, install this package with:
+
 ```bash
 pip install neo-ls-svm
 ```
 
 ### Classification and regression
 
 Then, you can import `neo_ls_svm.NeoLSSVM` as an sklearn-compatible binary classifier and regressor. Example usage:
@@ -41,131 +44,162 @@
 # Regression example:
 X, y = fetch_openml("ames_housing", version=1, return_X_y=True, as_frame=True, parser="auto")
 X_train, X_test, y_train, y_test = train_test_split(get_dummies(X), y, test_size=0.15, random_state=42)
 model = NeoLSSVM().fit(X_train, y_train)
 model.score(X_test, y_test)  # 82.4% (compared to sklearn.svm.SVR's -11.8%)
 ```
 
-### Confidence intervals
+### Predicting quantiles
 
-Neo LS-SVM implements conformal prediction with a Bayesian nonconformity estimate to compute confidence intervals for both classification and regression. Example usage:
+Neo LS-SVM implements conformal prediction with a Bayesian nonconformity estimate to compute quantiles and prediction intervals for both classification and regression. Example usage:
 
 ```python
-from neo_ls_svm import NeoLSSVM
-from pandas import get_dummies
-from sklearn.datasets import fetch_openml
-from sklearn.model_selection import train_test_split
-
-# Load a regression problem and split in train and test.
-X, y = fetch_openml("ames_housing", version=1, return_X_y=True, as_frame=True, parser="auto")
-X_train, X_test, y_train, y_test = train_test_split(get_dummies(X), y, test_size=50, random_state=42)
+# Predict the house prices and their quantiles.
+ŷ_test = model.predict(X_test)
+ŷ_test_quantiles = model.predict_quantiles(X_test, quantiles=(0.025, 0.05, 0.1, 0.9, 0.95, 0.975))
+```
 
-# Fit a Neo LS-SVM model.
-model = NeoLSSVM().fit(X_train, y_train)
+When the input data is a pandas DataFrame, the output is also a pandas DataFrame. For example, printing the head of `ŷ_test_quantiles` yields:
 
-# Predict the house prices and confidence intervals on the test set.
-ŷ = model.predict(X_test)
-ŷ_conf = model.predict_proba(X_test, confidence_interval=True, confidence_level=0.95)
-# ŷ_conf[:, 0] and ŷ_conf[:, 1] are the lower and upper bound of the confidence interval for the predictions ŷ, respectively
-```
+|   house_id |    0.025 |     0.05 |      0.1 |      0.9 |     0.95 |    0.975 |
+|-----------:|---------:|---------:|---------:|---------:|---------:|---------:|
+|       1357 | 114283.0 | 124767.6 | 133314.0 | 203162.0 | 220407.5 | 245655.3 |
+|       2367 |  85518.3 |  91787.2 |  93709.8 | 107464.3 | 108472.6 | 114482.3 |
+|       2822 | 147165.9 | 157462.8 | 167193.1 | 243646.5 | 263324.4 | 291963.3 |
+|       2126 |  81788.7 |  88738.1 |  91367.4 | 111944.9 | 114800.7 | 122874.5 |
+|       1544 |  94507.1 | 108288.2 | 120184.3 | 222630.5 | 248668.2 | 283703.4 |
 
-Let's visualize the confidence intervals on the test set:
+Let's visualize the predicted quantiles on the test set:
 
-<img src="https://github.com/lsorber/neo-ls-svm/assets/4543654/472bf358-34d7-4a1a-8b5c-595fe65dbf77" width="512">
+<img src="https://github.com/lsorber/neo-ls-svm/assets/4543654/cd24e739-e857-4045-8a70-07e92367a901" width="512">
 
 <details>
-<summary>Expand to see the code that generated the above graph.</summary>
+<summary>Expand to see the code that generated the graph above</summary>
 
 ```python
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
-import numpy as np
 
-idx = np.argsort(-ŷ)
-y_ticks = np.arange(1, len(X_test) + 1)
+%config InlineBackend.figure_format = "retina"
+plt.rcParams["font.size"] = 8
+idx = (-ŷ_test.sample(50, random_state=42)).sort_values().index
+y_ticks = list(range(1, len(idx) + 1))
 plt.figure(figsize=(4, 5))
-plt.barh(y_ticks, ŷ_conf[idx, 1] - ŷ_conf[idx, 0], left=ŷ_conf[idx, 0], label="95% Confidence interval", color="lightblue")
-plt.plot(y_test.iloc[idx], y_ticks, "s", markersize=3, markerfacecolor="none", markeredgecolor="cornflowerblue", label="Actual value")
-plt.plot(ŷ[idx], y_ticks, "s", color="mediumblue", markersize=0.6, label="Predicted value")
+for j in range(3):
+    end = ŷ_test_quantiles.shape[1] - 1 - j
+    coverage = round(100 * (ŷ_test_quantiles.columns[end] - ŷ_test_quantiles.columns[j]))
+    plt.barh(
+        y_ticks,
+        ŷ_test_quantiles.loc[idx].iloc[:, end] - ŷ_test_quantiles.loc[idx].iloc[:, j],
+        left=ŷ_test_quantiles.loc[idx].iloc[:, j],
+        label=f"{coverage}% Prediction interval",
+        color=["#b3d9ff", "#86bfff", "#4da6ff"][j],
+    )
+plt.plot(y_test.loc[idx], y_ticks, "s", markersize=3, markerfacecolor="none", markeredgecolor="#e74c3c", label="Actual value")
+plt.plot(ŷ_test.loc[idx], y_ticks, "s", color="blue", markersize=0.6, label="Predicted value")
 plt.xlabel("House price")
 plt.ylabel("Test house index")
+plt.xlim(0, 500e3)
 plt.yticks(y_ticks, y_ticks)
 plt.tick_params(axis="y", labelsize=6)
 plt.grid(axis="x", color="lightsteelblue", linestyle=":", linewidth=0.5)
-plt.gca().xaxis.set_major_formatter(ticker.StrMethodFormatter('${x:,.0f}'))
+plt.gca().xaxis.set_major_formatter(ticker.StrMethodFormatter("${x:,.0f}"))
 plt.gca().spines["top"].set_visible(False)
 plt.gca().spines["right"].set_visible(False)
 plt.legend()
 plt.tight_layout()
 plt.show()
 ```
 </details>
 
+### Predicting intervals
+
+In addition to quantile prediction, you can use `predict_interval` to predict conformally calibrated prediction intervals. Compared to quantiles, these focus on reliable coverage over quantile accuracy. Example usage:
+
+```python
+# Compute prediction intervals for the houses in the test set.
+ŷ_test_interval = model.predict_interval(X_test, coverage=0.95)
+
+# Measure the coverage of the prediction intervals on the test set
+coverage = ((ŷ_test_interval.iloc[:, 0] <= y_test) & (y_test <= ŷ_test_interval.iloc[:, 1])).mean()
+print(coverage)  # 94.3%
+```
+
+When the input data is a pandas DataFrame, the output is also a pandas DataFrame. For example, printing the head of `ŷ_test_interval` yields:
+
+|   house_id |    0.025 |    0.975 |
+|-----------:|---------:|---------:|
+|       1357 | 114283.0 | 245849.2 |
+|       2367 |  85518.3 | 114411.4 |
+|       2822 | 147165.9 | 292179.2 |
+|       2126 |  81788.7 | 122838.1 |
+|       1544 |  94507.1 | 284062.6 |
+
 ## Benchmarks
 
 We select all binary classification and regression datasets below 1M entries from the [AutoML Benchmark](https://arxiv.org/abs/2207.12560). Each dataset is split into 85% for training and 15% for testing. We apply `skrub.TableVectorizer` as a preprocessing step for `neo_ls_svm.NeoLSSVM` and `sklearn.svm.SVC,SVR` to vectorize the pandas DataFrame training data into a NumPy array. Models are fitted only once on each dataset, with their default settings and no hyperparameter tuning.
 
 <details open>
 <summary>Binary classification</summary>
 
 ROC-AUC on 15% test set:
 
-|                          dataset |   LGBMClassifier |        NeoLSSVM |             SVC |
-|---------------------------------:|-----------------:|----------------:|----------------:|
-|                              ada |  🥈 90.9% (0.1s) | 🥇 90.9% (0.8s) |    83.1% (1.0s) |
-|                            adult |  🥇 93.0% (0.5s) | 🥈 89.1% (6.0s) |               / |
-|           amazon_employee_access |  🥇 85.6% (0.5s) | 🥈 64.5% (2.8s) |               / |
-|                           arcene |  🥈 78.0% (0.6s) |    70.0% (4.4s) | 🥇 82.0% (3.4s) |
-|                       australian |  🥇 88.3% (0.2s) |    79.9% (0.4s) | 🥈 81.9% (0.0s) |
-|                   bank-marketing |  🥇 93.5% (0.3s) | 🥈 91.0% (4.1s) |               / |
-| blood-transfusion-service-center |     62.0% (0.1s) | 🥇 71.0% (0.5s) | 🥈 69.7% (0.0s) |
-|                            churn |  🥇 91.7% (0.4s) | 🥈 81.0% (0.8s) |    70.6% (0.8s) |
-|           click_prediction_small |  🥇 67.7% (0.4s) | 🥈 66.6% (3.3s) |               / |
-|                          jasmine |  🥇 86.1% (0.3s) |    79.5% (1.2s) | 🥈 85.3% (1.8s) |
-|                              kc1 |  🥇 78.9% (0.2s) | 🥈 76.6% (0.5s) |    45.7% (0.2s) |
-|                         kr-vs-kp | 🥇 100.0% (0.2s) |    99.2% (0.8s) | 🥈 99.4% (0.6s) |
-|                         madeline |  🥇 93.1% (0.4s) |    65.6% (0.8s) | 🥈 82.5% (4.5s) |
-|                  ozone-level-8hr |  🥈 91.2% (0.3s) | 🥇 91.6% (0.7s) |    72.8% (0.2s) |
-|                              pc4 |  🥇 95.3% (0.3s) | 🥈 90.9% (0.5s) |    25.7% (0.1s) |
-|                 phishingwebsites |  🥇 99.5% (0.3s) | 🥈 98.9% (1.3s) |    98.7% (2.6s) |
-|                          phoneme |  🥇 95.6% (0.2s) | 🥈 93.5% (0.8s) |    91.2% (0.7s) |
-|                      qsar-biodeg |  🥇 92.7% (0.2s) | 🥈 91.1% (1.2s) |    86.8% (0.1s) |
-|                        satellite |  🥈 98.7% (0.2s) | 🥇 99.5% (0.8s) |    98.5% (0.1s) |
-|                          sylvine |  🥇 98.5% (0.2s) | 🥈 97.1% (0.8s) |    96.5% (1.0s) |
-|                             wilt |  🥈 99.5% (0.2s) | 🥇 99.8% (0.9s) |    98.9% (0.2s) |
+|                          dataset |   LGBMClassifier |         NeoLSSVM |              SVC |
+|---------------------------------:|-----------------:|-----------------:|-----------------:|
+|                              ada |  🥈 90.9% (0.1s) |  🥇 90.9% (1.9s) |     83.1% (4.5s) |
+|                            adult |  🥇 93.0% (0.5s) | 🥈 89.0% (15.7s) |                / |
+|           amazon_employee_access |  🥇 85.6% (0.5s) |  🥈 64.5% (9.0s) |                / |
+|                           arcene |  🥈 78.0% (0.6s) |     70.0% (6.3s) |  🥇 82.0% (4.0s) |
+|                       australian |  🥇 88.3% (0.2s) |     79.9% (1.7s) |  🥈 81.9% (0.1s) |
+|                   bank-marketing |  🥇 93.5% (0.5s) | 🥈 91.0% (11.8s) |                / |
+| blood-transfusion-service-center |     62.0% (0.3s) |  🥇 71.0% (2.2s) |  🥈 69.7% (0.1s) |
+|                            churn |  🥇 91.7% (0.6s) |  🥈 81.0% (2.1s) |     70.6% (2.9s) |
+|           click_prediction_small |  🥇 67.7% (0.5s) | 🥈 66.6% (10.9s) |                / |
+|                          jasmine |  🥇 86.1% (0.3s) |     79.5% (1.9s) |  🥈 85.3% (7.4s) |
+|                              kc1 |  🥇 78.9% (0.3s) |  🥈 76.6% (1.4s) |     45.7% (0.6s) |
+|                         kr-vs-kp | 🥇 100.0% (0.6s) |     99.2% (1.6s) |  🥈 99.4% (2.3s) |
+|                         madeline |  🥇 93.1% (0.5s) |     65.6% (1.9s) | 🥈 82.5% (19.8s) |
+|                  ozone-level-8hr |  🥈 91.2% (0.4s) |  🥇 91.6% (1.7s) |     72.9% (0.6s) |
+|                              pc4 |  🥇 95.3% (0.3s) |  🥈 90.9% (1.5s) |     25.7% (0.3s) |
+|                 phishingwebsites |  🥇 99.5% (0.5s) |  🥈 98.9% (3.6s) |    98.7% (10.0s) |
+|                          phoneme |  🥇 95.6% (0.3s) |  🥈 93.5% (2.1s) |     91.2% (2.0s) |
+|                      qsar-biodeg |  🥇 92.7% (0.4s) |  🥈 91.1% (5.2s) |     86.8% (0.3s) |
+|                        satellite |  🥈 98.7% (0.2s) |  🥇 99.5% (1.9s) |     98.5% (0.4s) |
+|                          sylvine |  🥇 98.5% (0.2s) |  🥈 97.1% (2.0s) |     96.5% (3.8s) |
+|                             wilt |  🥈 99.5% (0.2s) |  🥇 99.8% (1.8s) |     98.9% (0.5s) |
 
 </details>
 
 <details open>
 <summary>Regression</summary>
 
 R² on 15% test set:
 
-|                       dataset |   LGBMRegressor |        NeoLSSVM |              SVR |
-|------------------------------:|----------------:|----------------:|-----------------:|
-|                       abalone | 🥈 56.2% (0.1s) | 🥇 59.5% (1.1s) |     51.3% (0.2s) |
-|                        boston | 🥇 91.7% (0.2s) | 🥈 89.3% (0.4s) |     35.1% (0.0s) |
-|              brazilian_houses | 🥈 55.9% (0.4s) | 🥇 88.3% (1.5s) |      5.4% (2.0s) |
-|                      colleges | 🥇 58.5% (0.4s) | 🥈 43.7% (4.1s) |     40.2% (5.1s) |
-|                      diamonds | 🥇 98.2% (0.7s) | 🥈 95.2% (4.5s) |                / |
-|                     elevators | 🥇 87.7% (0.4s) | 🥈 82.6% (2.6s) |                / |
-|                     house_16h | 🥇 67.7% (0.3s) | 🥈 52.8% (2.4s) |                / |
-|          house_prices_nominal | 🥇 89.0% (0.6s) | 🥈 78.2% (1.3s) |     -2.9% (0.3s) |
-|                   house_sales | 🥇 89.2% (1.3s) | 🥈 77.8% (2.2s) |                / |
-|           mip-2016-regression | 🥇 59.2% (0.4s) | 🥈 34.9% (2.6s) |    -27.3% (0.1s) |
-|                     moneyball | 🥇 93.2% (0.2s) | 🥈 91.2% (0.6s) |      0.8% (0.1s) |
-|                           pol | 🥇 98.7% (0.3s) | 🥈 75.2% (1.7s) |                / |
-|                         quake |   -10.7% (0.2s) | 🥇 -0.1% (0.5s) | 🥈 -10.7% (0.0s) |
-| sat11-hand-runtime-regression | 🥇 78.3% (0.5s) | 🥈 61.7% (1.0s) |    -56.3% (1.0s) |
-|                       sensory | 🥇 29.2% (0.2s) |     3.8% (0.4s) |  🥈 16.4% (0.0s) |
-|                        socmob | 🥇 79.6% (0.2s) | 🥈 72.5% (1.5s) |     30.8% (0.0s) |
-|                      space_ga | 🥇 70.3% (0.2s) | 🥈 43.7% (0.6s) |     35.9% (0.1s) |
-|                       tecator | 🥈 98.3% (0.1s) | 🥇 99.4% (0.2s) |     78.5% (0.0s) |
-|                      us_crime | 🥈 62.8% (0.4s) | 🥇 63.0% (0.8s) |      6.7% (0.2s) |
-|                  wine_quality | 🥇 45.6% (0.6s) |    -8.0% (0.9s) |  🥈 16.4% (0.5s) |
+|                       dataset |   LGBMRegressor |         NeoLSSVM |              SVR |
+|------------------------------:|----------------:|-----------------:|-----------------:|
+|                       abalone | 🥈 56.2% (0.1s) |  🥇 59.5% (2.5s) |     51.3% (0.7s) |
+|                        boston | 🥇 91.7% (0.2s) |  🥈 89.6% (1.1s) |     35.1% (0.0s) |
+|              brazilian_houses | 🥈 55.9% (0.3s) |  🥇 88.4% (3.7s) |      5.4% (7.0s) |
+|                      colleges | 🥇 58.5% (0.4s) |  🥈 42.2% (6.6s) |    40.2% (15.1s) |
+|                      diamonds | 🥇 98.2% (0.3s) | 🥈 95.2% (13.7s) |                / |
+|                     elevators | 🥇 87.7% (0.5s) |  🥈 82.6% (6.5s) |                / |
+|                     house_16h | 🥇 67.7% (0.4s) |  🥈 52.8% (6.0s) |                / |
+|          house_prices_nominal | 🥇 89.0% (0.3s) |  🥈 78.3% (2.1s) |     -2.9% (1.2s) |
+|                   house_sales | 🥇 89.2% (0.4s) |  🥈 77.8% (5.9s) |                / |
+|           mip-2016-regression | 🥇 59.2% (0.4s) |  🥈 34.9% (5.8s) |    -27.3% (0.4s) |
+|                     moneyball | 🥇 93.2% (0.3s) |  🥈 91.3% (1.1s) |      0.8% (0.2s) |
+|                           pol | 🥇 98.7% (0.3s) |  🥈 74.9% (4.6s) |                / |
+|                         quake |   -10.7% (0.2s) |  🥇 -1.0% (1.6s) | 🥈 -10.7% (0.1s) |
+| sat11-hand-runtime-regression | 🥇 78.3% (0.4s) |  🥈 61.7% (2.1s) |    -56.3% (5.1s) |
+|                       sensory | 🥇 29.2% (0.1s) |      3.0% (1.6s) |  🥈 16.4% (0.0s) |
+|                        socmob | 🥇 79.6% (0.2s) |  🥈 72.5% (6.6s) |     30.8% (0.1s) |
+|                      space_ga | 🥇 70.3% (0.3s) |  🥈 43.6% (1.5s) |     35.9% (0.2s) |
+|                       tecator | 🥈 98.3% (0.1s) |  🥇 99.4% (0.9s) |     78.5% (0.0s) |
+|                      us_crime | 🥈 62.8% (0.6s) |  🥇 63.0% (2.3s) |      6.7% (0.8s) |
+|                  wine_quality | 🥇 45.6% (0.2s) |  🥈 36.5% (2.8s) |     16.4% (1.6s) |
 
 </details>
 
 ## Contributing
 
 <details>
 <summary>Prerequisites</summary>
```

### Comparing `neo_ls_svm-0.2.0/pyproject.toml` & `neo_ls_svm-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "neo-ls-svm"
-version = "0.2.0"
+version = "0.3.0"
 description = "Neo LS-SVM"
 authors = ["Laurent Sorber <laurent.sorber@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/lsorber/neo-ls-svm"
 
 [tool.commitizen]  # https://commitizen-tools.github.io/commitizen/config/
 bump_message = "bump(release): v$current_version → v$new_version"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "0.2.0"
+version = "0.3.0"
 version_files = ["pyproject.toml:version"]
 
 [tool.poetry.dependencies]  # https://python-poetry.org/docs/dependency-specification/
 python = ">=3.10,<4.0"
 numba = ">=0.56.4"
 numpy = ">=1.22.4"
 scikit-learn = ">=1.1.3"
```

### Comparing `neo_ls_svm-0.2.0/src/neo_ls_svm/_affine_feature_map.py` & `neo_ls_svm-0.3.0/src/neo_ls_svm/_affine_feature_map.py`

 * *Files identical despite different names*

### Comparing `neo_ls_svm-0.2.0/src/neo_ls_svm/_affine_normalizer.py` & `neo_ls_svm-0.3.0/src/neo_ls_svm/_affine_normalizer.py`

 * *Files identical despite different names*

### Comparing `neo_ls_svm-0.2.0/src/neo_ls_svm/_affine_separator.py` & `neo_ls_svm-0.3.0/src/neo_ls_svm/_affine_separator.py`

 * *Files identical despite different names*

### Comparing `neo_ls_svm-0.2.0/src/neo_ls_svm/_feature_maps.py` & `neo_ls_svm-0.3.0/src/neo_ls_svm/_feature_maps.py`

 * *Files identical despite different names*

### Comparing `neo_ls_svm-0.2.0/src/neo_ls_svm/_quantizer.py` & `neo_ls_svm-0.3.0/src/neo_ls_svm/_quantizer.py`

 * *Files identical despite different names*

### Comparing `neo_ls_svm-0.2.0/src/neo_ls_svm/_typing.py` & `neo_ls_svm-0.3.0/src/neo_ls_svm/_typing.py`

 * *Files identical despite different names*

### Comparing `neo_ls_svm-0.2.0/src/neo_ls_svm/_weighted_quantile.py` & `neo_ls_svm-0.3.0/src/neo_ls_svm/_weighted_quantile.py`

 * *Files identical despite different names*

### Comparing `neo_ls_svm-0.2.0/PKG-INFO` & `neo_ls_svm-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-ls-svm
-Version: 0.2.0
+Version: 0.3.0
 Summary: Neo LS-SVM
 Home-page: https://github.com/lsorber/neo-ls-svm
 Author: Laurent Sorber
 Author-email: laurent.sorber@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -20,27 +20,30 @@
 [![Open in Dev Containers](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/lsorber/neo-ls-svm) [![Open in GitHub Codespaces](https://img.shields.io/static/v1?label=GitHub%20Codespaces&message=Open&color=blue&logo=github)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=739301655)
 
 # Neo LS-SVM
 
 Neo LS-SVM is a modern [Least-Squares Support Vector Machine](https://en.wikipedia.org/wiki/Least-squares_support_vector_machine) implementation in Python that offers several benefits over sklearn's classic `sklearn.svm.SVC` classifier and `sklearn.svm.SVR` regressor:
 
 1. ⚡ Linear complexity in the number of training examples with [Orthogonal Random Features](https://arxiv.org/abs/1610.09072).
-2. 🚀 Hyperparameter free: zero-cost optimization of the regularisation parameter γ and kernel parameter σ.
+2. 🚀 Hyperparameter free: zero-cost optimization of the [regularisation parameter γ](https://en.wikipedia.org/wiki/Ridge_regression#Tikhonov_regularization) and [kernel parameter σ](https://en.wikipedia.org/wiki/Radial_basis_function_kernel).
 3. 🏔️ Adds a new tertiary objective that minimizes the complexity of the prediction surface.
 4. 🎁 Returns the leave-one-out residuals and error for free after fitting.
 5. 🌀 Learns an affine transformation of the feature matrix to optimally separate the target's bins.
 6. 🪞 Can solve the LS-SVM both in the primal and dual space.
-7. 🌡️ Isotonically calibrated `predict_proba` based on the leave-one-out predictions.
-8. 🎲 Asymmetric conformal Bayesian confidence intervals for classification and regression.
+7. 🌡️ Isotonically calibrated `predict_proba`.
+8. ✅ Conformally calibrated `predict_quantiles` and `predict_interval`.
+9. 🔔 Bayesian estimation of the predictive standard deviation with `predict_std`.
+10. 🐼 Pandas DataFrame output when the input is a pandas DataFrame.
 
 ## Using
 
 ### Installing
 
 First, install this package with:
+
 ```bash
 pip install neo-ls-svm
 ```
 
 ### Classification and regression
 
 Then, you can import `neo_ls_svm.NeoLSSVM` as an sklearn-compatible binary classifier and regressor. Example usage:
@@ -60,131 +63,162 @@
 # Regression example:
 X, y = fetch_openml("ames_housing", version=1, return_X_y=True, as_frame=True, parser="auto")
 X_train, X_test, y_train, y_test = train_test_split(get_dummies(X), y, test_size=0.15, random_state=42)
 model = NeoLSSVM().fit(X_train, y_train)
 model.score(X_test, y_test)  # 82.4% (compared to sklearn.svm.SVR's -11.8%)
 ```
 
-### Confidence intervals
+### Predicting quantiles
 
-Neo LS-SVM implements conformal prediction with a Bayesian nonconformity estimate to compute confidence intervals for both classification and regression. Example usage:
+Neo LS-SVM implements conformal prediction with a Bayesian nonconformity estimate to compute quantiles and prediction intervals for both classification and regression. Example usage:
 
 ```python
-from neo_ls_svm import NeoLSSVM
-from pandas import get_dummies
-from sklearn.datasets import fetch_openml
-from sklearn.model_selection import train_test_split
-
-# Load a regression problem and split in train and test.
-X, y = fetch_openml("ames_housing", version=1, return_X_y=True, as_frame=True, parser="auto")
-X_train, X_test, y_train, y_test = train_test_split(get_dummies(X), y, test_size=50, random_state=42)
+# Predict the house prices and their quantiles.
+ŷ_test = model.predict(X_test)
+ŷ_test_quantiles = model.predict_quantiles(X_test, quantiles=(0.025, 0.05, 0.1, 0.9, 0.95, 0.975))
+```
 
-# Fit a Neo LS-SVM model.
-model = NeoLSSVM().fit(X_train, y_train)
+When the input data is a pandas DataFrame, the output is also a pandas DataFrame. For example, printing the head of `ŷ_test_quantiles` yields:
 
-# Predict the house prices and confidence intervals on the test set.
-ŷ = model.predict(X_test)
-ŷ_conf = model.predict_proba(X_test, confidence_interval=True, confidence_level=0.95)
-# ŷ_conf[:, 0] and ŷ_conf[:, 1] are the lower and upper bound of the confidence interval for the predictions ŷ, respectively
-```
+|   house_id |    0.025 |     0.05 |      0.1 |      0.9 |     0.95 |    0.975 |
+|-----------:|---------:|---------:|---------:|---------:|---------:|---------:|
+|       1357 | 114283.0 | 124767.6 | 133314.0 | 203162.0 | 220407.5 | 245655.3 |
+|       2367 |  85518.3 |  91787.2 |  93709.8 | 107464.3 | 108472.6 | 114482.3 |
+|       2822 | 147165.9 | 157462.8 | 167193.1 | 243646.5 | 263324.4 | 291963.3 |
+|       2126 |  81788.7 |  88738.1 |  91367.4 | 111944.9 | 114800.7 | 122874.5 |
+|       1544 |  94507.1 | 108288.2 | 120184.3 | 222630.5 | 248668.2 | 283703.4 |
 
-Let's visualize the confidence intervals on the test set:
+Let's visualize the predicted quantiles on the test set:
 
-<img src="https://github.com/lsorber/neo-ls-svm/assets/4543654/472bf358-34d7-4a1a-8b5c-595fe65dbf77" width="512">
+<img src="https://github.com/lsorber/neo-ls-svm/assets/4543654/cd24e739-e857-4045-8a70-07e92367a901" width="512">
 
 <details>
-<summary>Expand to see the code that generated the above graph.</summary>
+<summary>Expand to see the code that generated the graph above</summary>
 
 ```python
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
-import numpy as np
 
-idx = np.argsort(-ŷ)
-y_ticks = np.arange(1, len(X_test) + 1)
+%config InlineBackend.figure_format = "retina"
+plt.rcParams["font.size"] = 8
+idx = (-ŷ_test.sample(50, random_state=42)).sort_values().index
+y_ticks = list(range(1, len(idx) + 1))
 plt.figure(figsize=(4, 5))
-plt.barh(y_ticks, ŷ_conf[idx, 1] - ŷ_conf[idx, 0], left=ŷ_conf[idx, 0], label="95% Confidence interval", color="lightblue")
-plt.plot(y_test.iloc[idx], y_ticks, "s", markersize=3, markerfacecolor="none", markeredgecolor="cornflowerblue", label="Actual value")
-plt.plot(ŷ[idx], y_ticks, "s", color="mediumblue", markersize=0.6, label="Predicted value")
+for j in range(3):
+    end = ŷ_test_quantiles.shape[1] - 1 - j
+    coverage = round(100 * (ŷ_test_quantiles.columns[end] - ŷ_test_quantiles.columns[j]))
+    plt.barh(
+        y_ticks,
+        ŷ_test_quantiles.loc[idx].iloc[:, end] - ŷ_test_quantiles.loc[idx].iloc[:, j],
+        left=ŷ_test_quantiles.loc[idx].iloc[:, j],
+        label=f"{coverage}% Prediction interval",
+        color=["#b3d9ff", "#86bfff", "#4da6ff"][j],
+    )
+plt.plot(y_test.loc[idx], y_ticks, "s", markersize=3, markerfacecolor="none", markeredgecolor="#e74c3c", label="Actual value")
+plt.plot(ŷ_test.loc[idx], y_ticks, "s", color="blue", markersize=0.6, label="Predicted value")
 plt.xlabel("House price")
 plt.ylabel("Test house index")
+plt.xlim(0, 500e3)
 plt.yticks(y_ticks, y_ticks)
 plt.tick_params(axis="y", labelsize=6)
 plt.grid(axis="x", color="lightsteelblue", linestyle=":", linewidth=0.5)
-plt.gca().xaxis.set_major_formatter(ticker.StrMethodFormatter('${x:,.0f}'))
+plt.gca().xaxis.set_major_formatter(ticker.StrMethodFormatter("${x:,.0f}"))
 plt.gca().spines["top"].set_visible(False)
 plt.gca().spines["right"].set_visible(False)
 plt.legend()
 plt.tight_layout()
 plt.show()
 ```
 </details>
 
+### Predicting intervals
+
+In addition to quantile prediction, you can use `predict_interval` to predict conformally calibrated prediction intervals. Compared to quantiles, these focus on reliable coverage over quantile accuracy. Example usage:
+
+```python
+# Compute prediction intervals for the houses in the test set.
+ŷ_test_interval = model.predict_interval(X_test, coverage=0.95)
+
+# Measure the coverage of the prediction intervals on the test set
+coverage = ((ŷ_test_interval.iloc[:, 0] <= y_test) & (y_test <= ŷ_test_interval.iloc[:, 1])).mean()
+print(coverage)  # 94.3%
+```
+
+When the input data is a pandas DataFrame, the output is also a pandas DataFrame. For example, printing the head of `ŷ_test_interval` yields:
+
+|   house_id |    0.025 |    0.975 |
+|-----------:|---------:|---------:|
+|       1357 | 114283.0 | 245849.2 |
+|       2367 |  85518.3 | 114411.4 |
+|       2822 | 147165.9 | 292179.2 |
+|       2126 |  81788.7 | 122838.1 |
+|       1544 |  94507.1 | 284062.6 |
+
 ## Benchmarks
 
 We select all binary classification and regression datasets below 1M entries from the [AutoML Benchmark](https://arxiv.org/abs/2207.12560). Each dataset is split into 85% for training and 15% for testing. We apply `skrub.TableVectorizer` as a preprocessing step for `neo_ls_svm.NeoLSSVM` and `sklearn.svm.SVC,SVR` to vectorize the pandas DataFrame training data into a NumPy array. Models are fitted only once on each dataset, with their default settings and no hyperparameter tuning.
 
 <details open>
 <summary>Binary classification</summary>
 
 ROC-AUC on 15% test set:
 
-|                          dataset |   LGBMClassifier |        NeoLSSVM |             SVC |
-|---------------------------------:|-----------------:|----------------:|----------------:|
-|                              ada |  🥈 90.9% (0.1s) | 🥇 90.9% (0.8s) |    83.1% (1.0s) |
-|                            adult |  🥇 93.0% (0.5s) | 🥈 89.1% (6.0s) |               / |
-|           amazon_employee_access |  🥇 85.6% (0.5s) | 🥈 64.5% (2.8s) |               / |
-|                           arcene |  🥈 78.0% (0.6s) |    70.0% (4.4s) | 🥇 82.0% (3.4s) |
-|                       australian |  🥇 88.3% (0.2s) |    79.9% (0.4s) | 🥈 81.9% (0.0s) |
-|                   bank-marketing |  🥇 93.5% (0.3s) | 🥈 91.0% (4.1s) |               / |
-| blood-transfusion-service-center |     62.0% (0.1s) | 🥇 71.0% (0.5s) | 🥈 69.7% (0.0s) |
-|                            churn |  🥇 91.7% (0.4s) | 🥈 81.0% (0.8s) |    70.6% (0.8s) |
-|           click_prediction_small |  🥇 67.7% (0.4s) | 🥈 66.6% (3.3s) |               / |
-|                          jasmine |  🥇 86.1% (0.3s) |    79.5% (1.2s) | 🥈 85.3% (1.8s) |
-|                              kc1 |  🥇 78.9% (0.2s) | 🥈 76.6% (0.5s) |    45.7% (0.2s) |
-|                         kr-vs-kp | 🥇 100.0% (0.2s) |    99.2% (0.8s) | 🥈 99.4% (0.6s) |
-|                         madeline |  🥇 93.1% (0.4s) |    65.6% (0.8s) | 🥈 82.5% (4.5s) |
-|                  ozone-level-8hr |  🥈 91.2% (0.3s) | 🥇 91.6% (0.7s) |    72.8% (0.2s) |
-|                              pc4 |  🥇 95.3% (0.3s) | 🥈 90.9% (0.5s) |    25.7% (0.1s) |
-|                 phishingwebsites |  🥇 99.5% (0.3s) | 🥈 98.9% (1.3s) |    98.7% (2.6s) |
-|                          phoneme |  🥇 95.6% (0.2s) | 🥈 93.5% (0.8s) |    91.2% (0.7s) |
-|                      qsar-biodeg |  🥇 92.7% (0.2s) | 🥈 91.1% (1.2s) |    86.8% (0.1s) |
-|                        satellite |  🥈 98.7% (0.2s) | 🥇 99.5% (0.8s) |    98.5% (0.1s) |
-|                          sylvine |  🥇 98.5% (0.2s) | 🥈 97.1% (0.8s) |    96.5% (1.0s) |
-|                             wilt |  🥈 99.5% (0.2s) | 🥇 99.8% (0.9s) |    98.9% (0.2s) |
+|                          dataset |   LGBMClassifier |         NeoLSSVM |              SVC |
+|---------------------------------:|-----------------:|-----------------:|-----------------:|
+|                              ada |  🥈 90.9% (0.1s) |  🥇 90.9% (1.9s) |     83.1% (4.5s) |
+|                            adult |  🥇 93.0% (0.5s) | 🥈 89.0% (15.7s) |                / |
+|           amazon_employee_access |  🥇 85.6% (0.5s) |  🥈 64.5% (9.0s) |                / |
+|                           arcene |  🥈 78.0% (0.6s) |     70.0% (6.3s) |  🥇 82.0% (4.0s) |
+|                       australian |  🥇 88.3% (0.2s) |     79.9% (1.7s) |  🥈 81.9% (0.1s) |
+|                   bank-marketing |  🥇 93.5% (0.5s) | 🥈 91.0% (11.8s) |                / |
+| blood-transfusion-service-center |     62.0% (0.3s) |  🥇 71.0% (2.2s) |  🥈 69.7% (0.1s) |
+|                            churn |  🥇 91.7% (0.6s) |  🥈 81.0% (2.1s) |     70.6% (2.9s) |
+|           click_prediction_small |  🥇 67.7% (0.5s) | 🥈 66.6% (10.9s) |                / |
+|                          jasmine |  🥇 86.1% (0.3s) |     79.5% (1.9s) |  🥈 85.3% (7.4s) |
+|                              kc1 |  🥇 78.9% (0.3s) |  🥈 76.6% (1.4s) |     45.7% (0.6s) |
+|                         kr-vs-kp | 🥇 100.0% (0.6s) |     99.2% (1.6s) |  🥈 99.4% (2.3s) |
+|                         madeline |  🥇 93.1% (0.5s) |     65.6% (1.9s) | 🥈 82.5% (19.8s) |
+|                  ozone-level-8hr |  🥈 91.2% (0.4s) |  🥇 91.6% (1.7s) |     72.9% (0.6s) |
+|                              pc4 |  🥇 95.3% (0.3s) |  🥈 90.9% (1.5s) |     25.7% (0.3s) |
+|                 phishingwebsites |  🥇 99.5% (0.5s) |  🥈 98.9% (3.6s) |    98.7% (10.0s) |
+|                          phoneme |  🥇 95.6% (0.3s) |  🥈 93.5% (2.1s) |     91.2% (2.0s) |
+|                      qsar-biodeg |  🥇 92.7% (0.4s) |  🥈 91.1% (5.2s) |     86.8% (0.3s) |
+|                        satellite |  🥈 98.7% (0.2s) |  🥇 99.5% (1.9s) |     98.5% (0.4s) |
+|                          sylvine |  🥇 98.5% (0.2s) |  🥈 97.1% (2.0s) |     96.5% (3.8s) |
+|                             wilt |  🥈 99.5% (0.2s) |  🥇 99.8% (1.8s) |     98.9% (0.5s) |
 
 </details>
 
 <details open>
 <summary>Regression</summary>
 
 R² on 15% test set:
 
-|                       dataset |   LGBMRegressor |        NeoLSSVM |              SVR |
-|------------------------------:|----------------:|----------------:|-----------------:|
-|                       abalone | 🥈 56.2% (0.1s) | 🥇 59.5% (1.1s) |     51.3% (0.2s) |
-|                        boston | 🥇 91.7% (0.2s) | 🥈 89.3% (0.4s) |     35.1% (0.0s) |
-|              brazilian_houses | 🥈 55.9% (0.4s) | 🥇 88.3% (1.5s) |      5.4% (2.0s) |
-|                      colleges | 🥇 58.5% (0.4s) | 🥈 43.7% (4.1s) |     40.2% (5.1s) |
-|                      diamonds | 🥇 98.2% (0.7s) | 🥈 95.2% (4.5s) |                / |
-|                     elevators | 🥇 87.7% (0.4s) | 🥈 82.6% (2.6s) |                / |
-|                     house_16h | 🥇 67.7% (0.3s) | 🥈 52.8% (2.4s) |                / |
-|          house_prices_nominal | 🥇 89.0% (0.6s) | 🥈 78.2% (1.3s) |     -2.9% (0.3s) |
-|                   house_sales | 🥇 89.2% (1.3s) | 🥈 77.8% (2.2s) |                / |
-|           mip-2016-regression | 🥇 59.2% (0.4s) | 🥈 34.9% (2.6s) |    -27.3% (0.1s) |
-|                     moneyball | 🥇 93.2% (0.2s) | 🥈 91.2% (0.6s) |      0.8% (0.1s) |
-|                           pol | 🥇 98.7% (0.3s) | 🥈 75.2% (1.7s) |                / |
-|                         quake |   -10.7% (0.2s) | 🥇 -0.1% (0.5s) | 🥈 -10.7% (0.0s) |
-| sat11-hand-runtime-regression | 🥇 78.3% (0.5s) | 🥈 61.7% (1.0s) |    -56.3% (1.0s) |
-|                       sensory | 🥇 29.2% (0.2s) |     3.8% (0.4s) |  🥈 16.4% (0.0s) |
-|                        socmob | 🥇 79.6% (0.2s) | 🥈 72.5% (1.5s) |     30.8% (0.0s) |
-|                      space_ga | 🥇 70.3% (0.2s) | 🥈 43.7% (0.6s) |     35.9% (0.1s) |
-|                       tecator | 🥈 98.3% (0.1s) | 🥇 99.4% (0.2s) |     78.5% (0.0s) |
-|                      us_crime | 🥈 62.8% (0.4s) | 🥇 63.0% (0.8s) |      6.7% (0.2s) |
-|                  wine_quality | 🥇 45.6% (0.6s) |    -8.0% (0.9s) |  🥈 16.4% (0.5s) |
+|                       dataset |   LGBMRegressor |         NeoLSSVM |              SVR |
+|------------------------------:|----------------:|-----------------:|-----------------:|
+|                       abalone | 🥈 56.2% (0.1s) |  🥇 59.5% (2.5s) |     51.3% (0.7s) |
+|                        boston | 🥇 91.7% (0.2s) |  🥈 89.6% (1.1s) |     35.1% (0.0s) |
+|              brazilian_houses | 🥈 55.9% (0.3s) |  🥇 88.4% (3.7s) |      5.4% (7.0s) |
+|                      colleges | 🥇 58.5% (0.4s) |  🥈 42.2% (6.6s) |    40.2% (15.1s) |
+|                      diamonds | 🥇 98.2% (0.3s) | 🥈 95.2% (13.7s) |                / |
+|                     elevators | 🥇 87.7% (0.5s) |  🥈 82.6% (6.5s) |                / |
+|                     house_16h | 🥇 67.7% (0.4s) |  🥈 52.8% (6.0s) |                / |
+|          house_prices_nominal | 🥇 89.0% (0.3s) |  🥈 78.3% (2.1s) |     -2.9% (1.2s) |
+|                   house_sales | 🥇 89.2% (0.4s) |  🥈 77.8% (5.9s) |                / |
+|           mip-2016-regression | 🥇 59.2% (0.4s) |  🥈 34.9% (5.8s) |    -27.3% (0.4s) |
+|                     moneyball | 🥇 93.2% (0.3s) |  🥈 91.3% (1.1s) |      0.8% (0.2s) |
+|                           pol | 🥇 98.7% (0.3s) |  🥈 74.9% (4.6s) |                / |
+|                         quake |   -10.7% (0.2s) |  🥇 -1.0% (1.6s) | 🥈 -10.7% (0.1s) |
+| sat11-hand-runtime-regression | 🥇 78.3% (0.4s) |  🥈 61.7% (2.1s) |    -56.3% (5.1s) |
+|                       sensory | 🥇 29.2% (0.1s) |      3.0% (1.6s) |  🥈 16.4% (0.0s) |
+|                        socmob | 🥇 79.6% (0.2s) |  🥈 72.5% (6.6s) |     30.8% (0.1s) |
+|                      space_ga | 🥇 70.3% (0.3s) |  🥈 43.6% (1.5s) |     35.9% (0.2s) |
+|                       tecator | 🥈 98.3% (0.1s) |  🥇 99.4% (0.9s) |     78.5% (0.0s) |
+|                      us_crime | 🥈 62.8% (0.6s) |  🥇 63.0% (2.3s) |      6.7% (0.8s) |
+|                  wine_quality | 🥇 45.6% (0.2s) |  🥈 36.5% (2.8s) |     16.4% (1.6s) |
 
 </details>
 
 ## Contributing
 
 <details>
 <summary>Prerequisites</summary>
```

