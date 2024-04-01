# Comparing `tmp/mlimputer-1.0.55-py3-none-any.whl.zip` & `tmp/mlimputer-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8985 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat        0 b- defN 24-Jan-02 00:48 mlimputer/__init__.py
--rw-rw-rw-  2.0 fat     5174 b- defN 24-Jan-02 00:54 mlimputer/imputation.py
--rw-rw-rw-  2.0 fat     6344 b- defN 24-Jan-02 00:48 mlimputer/model_selection.py
--rw-rw-rw-  2.0 fat     1240 b- defN 24-Jan-02 00:48 mlimputer/parameters.py
--rw-rw-rw-  2.0 fat     1090 b- defN 24-Apr-01 18:04 mlimputer-1.0.55.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7033 b- defN 24-Apr-01 18:04 mlimputer-1.0.55.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-01 18:04 mlimputer-1.0.55.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-01 18:04 mlimputer-1.0.55.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      721 b- defN 24-Apr-01 18:04 mlimputer-1.0.55.dist-info/RECORD
-9 files, 21704 bytes uncompressed, 7741 bytes compressed:  64.3%
+Zip file size: 9246 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      389 b- defN 23-Feb-20 00:15 mlimputer/__init__.py
+-rw-rw-rw-  2.0 fat     4834 b- defN 23-May-06 15:58 mlimputer/mli_imputation.py
+-rw-rw-rw-  2.0 fat     6293 b- defN 23-Jul-04 20:19 mlimputer/mli_model_selection.py
+-rw-rw-rw-  2.0 fat     1358 b- defN 23-Jul-04 20:20 mlimputer/mli_parameters.py
+-rw-rw-rw-  2.0 fat     1090 b- defN 23-Jul-04 20:22 mlimputer-1.0.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6896 b- defN 23-Jul-04 20:22 mlimputer-1.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 20:22 mlimputer-1.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-04 20:22 mlimputer-1.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      730 b- defN 23-Jul-04 20:22 mlimputer-1.0.6.dist-info/RECORD
+9 files, 21692 bytes uncompressed, 7988 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: mlimputer/__init__.py
 Comment: 
 
-Filename: mlimputer/imputation.py
+Filename: mlimputer/mli_imputation.py
 Comment: 
 
-Filename: mlimputer/model_selection.py
+Filename: mlimputer/mli_model_selection.py
 Comment: 
 
-Filename: mlimputer/parameters.py
+Filename: mlimputer/mli_parameters.py
 Comment: 
 
-Filename: mlimputer-1.0.55.dist-info/LICENSE
+Filename: mlimputer-1.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: mlimputer-1.0.55.dist-info/METADATA
+Filename: mlimputer-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: mlimputer-1.0.55.dist-info/WHEEL
+Filename: mlimputer-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: mlimputer-1.0.55.dist-info/top_level.txt
+Filename: mlimputer-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: mlimputer-1.0.55.dist-info/RECORD
+Filename: mlimputer-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlimputer/__init__.py

```diff
@@ -0,0 +1,25 @@
+00000000: 696d 706f 7274 2069 6d70 6f72 746c 6962  import importlib
+00000010: 0d0a 696d 706f 7274 2070 6b67 7574 696c  ..import pkgutil
+00000020: 0d0a 0d0a 2320 496d 706f 7274 2061 6c6c  ....# Import all
+00000030: 2073 7562 2d6d 6f64 756c 6573 0d0a 666f   sub-modules..fo
+00000040: 7220 6c6f 6164 6572 2c20 6d6f 6475 6c65  r loader, module
+00000050: 5f6e 616d 652c 2069 735f 706b 6720 696e  _name, is_pkg in
+00000060: 2070 6b67 7574 696c 2e77 616c 6b5f 7061   pkgutil.walk_pa
+00000070: 636b 6167 6573 285f 5f70 6174 685f 5f29  ckages(__path__)
+00000080: 3a0d 0a20 2020 206d 6f64 756c 6520 3d20  :..    module = 
+00000090: 696d 706f 7274 6c69 622e 696d 706f 7274  importlib.import
+000000a0: 5f6d 6f64 756c 6528 6622 7b5f 5f6e 616d  _module(f"{__nam
+000000b0: 655f 5f7d 2e7b 6d6f 6475 6c65 5f6e 616d  e__}.{module_nam
+000000c0: 657d 2229 0d0a 2020 2020 676c 6f62 616c  e}")..    global
+000000d0: 7328 292e 7570 6461 7465 287b 6e61 6d65  s().update({name
+000000e0: 3a20 6765 7461 7474 7228 6d6f 6475 6c65  : getattr(module
+000000f0: 2c20 6e61 6d65 2920 666f 7220 6e61 6d65  , name) for name
+00000100: 2069 6e20 6469 7228 6d6f 6475 6c65 2920   in dir(module) 
+00000110: 6966 206e 6f74 206e 616d 652e 7374 6172  if not name.star
+00000120: 7473 7769 7468 2822 5f22 297d 290d 0a0d  tswith("_")})...
+00000130: 0a23 2044 6566 696e 6520 5f5f 616c 6c5f  .# Define __all_
+00000140: 5f0d 0a5f 5f61 6c6c 5f5f 203d 205b 6e61  _..__all__ = [na
+00000150: 6d65 2066 6f72 206e 616d 6520 696e 2067  me for name in g
+00000160: 6c6f 6261 6c73 2829 2069 6620 6e6f 7420  lobals() if not 
+00000170: 6e61 6d65 2e73 7461 7274 7377 6974 6828  name.startswith(
+00000180: 225f 2229 5d                             "_")]
```

## Comparing `mlimputer/model_selection.py` & `mlimputer/mli_model_selection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-from atlantic.analysis import Analysis
-from atlantic.evaluation import Evaluation
+import pandas as pd
+import numpy as np
+import sys
+from tqdm import tqdm
+from sklearn.metrics import *
 from sklearn.model_selection import train_test_split
-from sklearn.ensemble import RandomForestRegressor, ExtraTreesRegressor, GradientBoostingRegressor
+from sklearn.ensemble import RandomForestRegressor, ExtraTreesRegressor, GradientBoostingRegressor, StackingRegressor
 from sklearn.neighbors import KNeighborsRegressor
-import pandas as pd
+from sklearn.linear_model import TweedieRegressor
+import atlantic as atl
 import catboost as cb
 import xgboost
 import lightgbm as lgb 
-from mlimputer.parameters import imputer_parameters
+from .mli_parameters import imputer_parameters
 
 parameters=imputer_parameters()
 
-def imput_models(train : pd.DataFrame,
-                 target : str = "y",
-                 algo : str = 'RandomForest',
-                 parameters : dict = parameters):
+def imput_models(train:pd.DataFrame,
+                 target:str="y",
+                 algo:str='RandomForest',
+                 parameters:dict=parameters):
     """
     This function trains and returns a regression model based on the input data and specified algorithm.
     
     Parameters:
     train (pd.DataFrame): The input training data
     target (str, optional): The target column name in the training data. Default is 'y'
     algo (str, optional): The algorithm to be used for training. Default is 'RandomForest'
@@ -27,134 +31,128 @@
     Returns:
     model: trained machine learning model.
     """
     
     sel_cols=list(train.columns)
     sel_cols.remove(target)
     sel_cols.append(target)
-    train = train[sel_cols]
+    train=train[sel_cols]
     
     X_train = train.iloc[:, 0:(len(sel_cols)-1)].values
     y_train = train.iloc[:, (len(sel_cols)-1)].values
     
-    if algo == 'RandomForest':
-        rf_params = parameters['RandomForest']
+    if algo=='RandomForest':
+        rf_params=parameters['RandomForest']
         model = RandomForestRegressor(**rf_params)
         model.fit(X_train, y_train)
         
-    elif algo == 'ExtraTrees':
-        et_params = parameters['ExtraTrees']
+    elif algo=='ExtraTrees':
+        et_params=parameters['ExtraTrees']
         model = ExtraTreesRegressor(**et_params)
         model.fit(X_train, y_train)
         
-    elif algo == 'GBR':
-        gbr_params = parameters['GBR']
+    elif algo=='GBR':
+        gbr_params=parameters['GBR']
         model = GradientBoostingRegressor(**gbr_params)
         model.fit(X_train, y_train)
         
-    elif algo == 'KNN':
-        knn_params = parameters['KNN']
+    elif algo=='KNN':
+        knn_params=parameters['KNN']
         model = KNeighborsRegressor(**knn_params)
         model.fit(X_train, y_train)
         
-    elif algo == 'XGBoost':
-        xg_params = parameters['XGBoost']
+    elif algo=='XGBoost':
+        xg_params=parameters['XGBoost']
         model = xgboost.XGBRegressor(**xg_params)
         model.fit(X_train, y_train)
     
-    elif algo == "Catboost":
-        cb_params = parameters['Catboost']
+    elif algo=="Catboost":
+        cb_params=parameters['Catboost']
         model = cb.CatBoostRegressor(**cb_params)
         model.fit(X_train, y_train)
         
-    elif algo == "Lightgbm":
-        lb_params = parameters['Lightgbm']
+    elif algo=="Lightgbm":
+        lb_params=parameters['Lightgbm']
         train_data = lgb.Dataset(X_train, label=y_train)
         model = lgb.train(lb_params, train_data, num_boost_round=100)
         
     else:
         raise ValueError('Invalid model')
    
     return model
 
-def missing_report(X : pd.DataFrame):
+def missing_report(dataset:pd.DataFrame):
     """
-    This function generates a report of missing values in a given X.
+    This function generates a report of missing values in a given dataset.
     
     Parameters:
-    X (pd.DataFrame): The input data to be analyzed for missing values
+    dataset (pd.DataFrame): The input data to be analyzed for missing values
     
     Returns:
-    X_md (pd.DataFrame): A dataframe containing the count and percentage of missing values 
-    for each numerical column in the input X. 
+    df_md (pd.DataFrame): A dataframe containing the count and percentage of missing values 
+    for each numerical column in the input dataset. 
     Sorted by the percentage of missing values in ascending order. <-***********
     """
     
-    X_ = X.copy()
+    df=dataset.copy()
+    
+    num_cols=df.select_dtypes(include=['int','float']).columns.tolist()
+    df_md = pd.DataFrame(df[num_cols].isna().sum().loc[df[num_cols].isna().sum() > 0], columns=['null_count'])
+    df_md['null_percentage'] = df_md['null_count'] / len(df)
+    df_md = df_md.sort_values(by='null_percentage', ascending=True)
+    df_md['columns']=df_md.index
+    df_md=df_md.reset_index(drop=True)
     
-    num_cols = X_.select_dtypes(include=['int','float']).columns.tolist()
-    X_md = pd.DataFrame(X_[num_cols].isna().sum().loc[X_[num_cols].isna().sum() > 0], columns = ['null_count'])
-    X_md['null_percentage'] = X_md['null_count'] / len(X_)
-    X_md = X_md.sort_values(by = 'null_percentage', ascending=True)
-    X_md['columns'] = X_md.index
-    X_md = X_md.reset_index(drop = True)
-    
-    return X_md
-
-def cross_validation(X : pd.DataFrame, 
-                     target : str, 
-                     test_size : float = 0.2, 
-                     n_splits : int = 5,
-                     models : list = []):
+    return df_md
+
+def cross_validation(dataset:pd.DataFrame, target:str, test_size:float=0.2, n_splits:int=5,models:list=[]):
     """
-    This function performs cross-validation on the given X. The X is divided into training and test sets, 
+    This function performs cross-validation on the given dataset. The dataset is divided into training and test sets, 
     and then each model from the list is fit and evaluated on the test set. The performance of each model on the test
     set is recorded in the form of various metrics, such as accuracy, precision, recall, F1-score, etc. (depending on
     whether the target variable is a continuous variable or a categorical variable). The final result of the function
     is a leaderboard containing the metrics of each model for each fold of the cross-validation.
     
     Parameters:
     -----------
-    X: pd.DataFrame
-        The input X to be evaluated.
+    dataset: pd.DataFrame
+        The input dataset to be evaluated.
     target: str
         The name of the target column.
     test_size: float, optional (default=0.2)
-        The size of the test set, specified as a fraction of the input X.
+        The size of the test set, specified as a fraction of the input dataset.
     n_splits: int, optional (default=5)
         The number of folds for cross-validation.
     models: list, optional (default=[])
         A list of models to be evaluated.
         
     Returns:
     --------
     leaderboard: pd.DataFrame
         A dataframe containing the performance metrics of each model for each fold of the cross-validation.
     """
     
-    y ,list_metrics = X[target], []
-    sv_pred ,_ = Analysis(target=target).target_type(X = X)
+    y,list_metrics=dataset[target],[]
+    sv_pred=atl.target_type(dataset, target)[0]
     for i in range(n_splits):
-        X_train, X_test, y_train, y_test = train_test_split(X, y, test_size = test_size)
-        print(f"Fold {i + 1} :")
+        X_train, X_test, y_train, y_test = train_test_split(dataset, y, test_size=test_size)
+        print(f"Fold number: {i + 1}")
 
-        X_train,X_test = X_train.drop([target], axis = 1),X_test.drop([target], axis=1)
+        X_train,X_test=X_train.drop([target], axis=1),X_test.drop([target], axis=1)
         for model in models:
             print(f"Fitting {model.__class__.__name__} model")
             model.fit(X_train, y_train)
             y_pred = model.predict(X_test)
             score = model.score(X_test, y_test)
             print(f"{model.__class__.__name__} model score: {score}")
-            if sv_pred == 'Class':
-                metrics = pd.DataFrame(Evaluation.metrics_classification(y_test,y_pred),index = [0])
-            elif sv_pred == 'Reg':
-                metrics = pd.DataFrame(Evaluation.metrics_regression(y_test,y_pred),index = [0])
-            metrics["model"] = model.__class__.__name__
-            metrics["n_splits"] = i+1
-            metrics = metrics.reset_index(drop = True)
+            if sv_pred=='Class':
+                metrics=pd.DataFrame(atl.metrics_classification(y_test,y_pred),index=[0])
+            elif sv_pred=='Reg':
+                metrics = pd.DataFrame(atl.metrics_regression(y_test,y_pred),index=[0])
+            metrics["model"]=model.__class__.__name__
+            metrics["n_splits"]=i+1
+            metrics=metrics.reset_index(drop=True)
             list_metrics.append(metrics)
 
-    leaderboard = pd.concat(list_metrics)
-    
-    leaderboard = leaderboard.reset_index(drop = True)
-    
-    return leaderboard
+    leaderboard= pd.concat(list_metrics)
+    leaderboard=leaderboard.reset_index(drop=True)
+    return leaderboard
```

## Comparing `mlimputer/parameters.py` & `mlimputer/mli_parameters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 def imputer_parameters():
-    
     parameters ={'RandomForest':{'n_estimators':50,'random_state':42,'criterion':"squared_error",
                                  'max_depth':None},
                  'ExtraTrees':{'n_estimators':50,'random_state':42,'criterion':"squared_error",
                                'max_depth':None}, 
-                 'GBR':{'n_estimators':50,'learning_rate':0.01,'criterion':"friedman_mse",
-                        'max_depth':3,'min_samples_split':5,'loss':'squared_error'},
-                 'KNN':{'n_neighbors': 3,'weights':"uniform",'algorithm':"auto",
-                        'metric_params':None},
-                 'XGBoost':{'objective':'reg:squarederror','n_estimators':100,'nthread':24},
+                 'GBR':{'n_estimators':50,'learning_rate':0.1,'criterion':"friedman_mse",
+                        'max_depth':3,'min_samples_split':5,'learning_rate':0.01,'loss':'squared_error'},
+                 'KNN':{'n_neighbors': 3,'weights':"uniform",
+                        'algorithm':"auto",'metric_params':None},
+                 'XGBoost':{'objective':'reg:squarederror','n_estimators':1000,'nthread':24},
                  "Lightgbm": {'boosting_type': 'gbdt','objective':'regression','metric': 'mse',
                               'num_leaves': 31,'learning_rate': 0.05,'feature_fraction': 0.9,
-                              'bagging_fraction': 0.8,'bagging_freq': 5}, 
+                              'bagging_fraction': 0.8,'bagging_freq': 5,'reg_alpha': 0.1,
+                              'reg_lambda': 0.1,'verbose': 0, 'force_col_wise':True}, 
                  'Catboost':{'iterations': 100, 'depth': 5, 'learning_rate': 0.1, 'loss_function': 'RMSE', 
                              'l2_leaf_reg': 3, 'random_seed': 42, 'verbose': False }
                  }
     return parameters
```

## Comparing `mlimputer-1.0.55.dist-info/LICENSE` & `mlimputer-1.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mlimputer-1.0.55.dist-info/METADATA` & `mlimputer-1.0.6.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 Metadata-Version: 2.1
 Name: mlimputer
-Version: 1.0.55
+Version: 1.0.6
 Summary: MLimputer - Null Imputation Framework for Supervised Machine Learning
 Home-page: https://github.com/TsLu1s/MLimputer
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
-Keywords: data science,machine learning,data preprecessing,null imputation,missing data imputation,predictive null imputation,multiple null imputation,automated machine learning
+Keywords: data science,machine learning,data preprecessing,null imputation,predictive null imputation,multiple null imputation,automated machine learning
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scikit-learn (>=1.0.2)
-Requires-Dist: atlantic (>=1.1.25)
+Requires-Dist: atlantic (>=1.0.50)
 Requires-Dist: catboost (>=1.1.1)
 Requires-Dist: xgboost (>=1.7.3)
 Requires-Dist: lightgbm (>=3.3.5)
 
 <br>
 <p align="center">
   <h2 align="center"> MLimputer - Null Imputation Framework for Supervised Machine Learning
   <br>
   
 ## Framework Contextualization <a name = "ta"></a>
 
 The `MLimputer` project constitutes an complete and integrated pipeline to automate the handling of missing values in datasets through regression prediction and aims at reducing bias and increase the precision of imputation results when compared to more classic imputation methods.
-This package provides multiple algorithm options to impute your data, in which every observed data column with existing missing values is fitted with a robust preprocessing approach and subsequently predicted.
+This package provides multiple algorithm options to impute your data (shown bellow), in which every observed data column with existing missing values is fitted with a robust preprocessing approach and subsequently predicted.
 
-The architecture design includes three main sections, these being: missing data analysis, data preprocessing and supervised model imputation which are organized in a customizable pipeline structure.
+The architecture design includes three main sections, these being: missing data analysis, data preprocessing and predictive model imputation which are organized in a customizable pipeline structure.
 
 This project aims at providing the following application capabilities:
 
 * General applicability on tabular datasets: The developed imputation procedures are applicable on any data table associated with any Supervised ML scopes, based on missing data columns to be imputed.
     
 * Robustness and improvement of predictive results: The application of the MLimputer preprocessing aims at improve the predictive performance through customization and optimization of existing missing values imputation in the dataset input columns. 
    
@@ -67,91 +65,88 @@
 
 ```
 pip install mlimputer
 ```
 
 # Usage Examples
     
-The first needed step after importing the package is to load a dataset (split it) and define your choosen imputation model.
+The first needed step after importing the package is to load a dataset (split it) and define your choosen imputation model in`fit_imput` function.
 The imputation model options for handling the missing data in your dataset are the following:
 * `RandomForest`
 * `ExtraTrees`
 * `GBR`
 * `KNN`
 * `XGBoost`
 * `Lightgbm`
 * `Catboost`
 
-After creating a `MLimputer` object with your imputation selected model, you can then fit the missing data through the `fit_imput` method. From there you can impute the future datasets with `transform_imput` (validate, test ...) with the same data properties. Note, as it shows in the example bellow, you can also customize your model imputer parameters by changing it's configurations and then, implementing them in the `imputer_configs` parameter.
+After fitting your imputation model, you can load the `imputer` variable into `fit_configs` parameter in the `transform_imput` function. From there you can impute the future datasets (validate, test ...) with the same data properties. Note, as it shows in the example bellow, you can also customize your model imputer parameters by changing it's configurations and then, implementing them in the `imputer_configs` function parameter.
 
 Through the `cross_validation` function you can also compare the predictive performance evalution of multiple imputations, allowing you to validate which imputation model fits better your future predictions.
 
 Importante Notes:
 
 * The actual version of this package does not incorporate the imputing of categorical values, just the automatic handling of numeric missing values is implemented.
 
 ```py
 
-from mlimputer.imputation import MLimputer
-import mlimputer.model_selection as ms
-from mlimputer.parameters import imputer_parameters
+import mlimputer as mli
 import pandas as pd
 import numpy as np
 from sklearn.model_selection import train_test_split
 import warnings
 warnings.filterwarnings("ignore", category=Warning) #-> For a clean console
 
 data = pd.read_csv('csv_directory_path') # Dataframe Loading Example
 
-train,test = train_test_split(data, train_size=0.8)
-train,test = train.reset_index(drop=True), test.reset_index(drop=True) # <- Required
+train, test= train_test_split(data, train_size=0.8)
+train,test=train.reset_index(drop=True), test.reset_index(drop=True) # <- Required
 
 # All model imputation options ->  "RandomForest","ExtraTrees","GBR","KNN","XGBoost","Lightgbm","Catboost"
 
-# Customizing Hyperparameters Example
+# Model Imputer Customization
+hparameters=mli.imputer_parameters()
 
-hparameters = params.imputer_parameters()
+# Customizing parameters settings
+hparameters["RandomForest"]["n_estimators"]=40
+hparameters["KNN"]["n_neighbors"]=5
 print(hparameters)
-hparameters["KNN"]["n_neighbors"] = 5
-hparameters["RandomForest"]["n_estimators"] = 30
     
-# Imputation Example 1 : KNN
+# Imputation Example 1 : RandomForest
 
-mli_knn = MLimputer(imput_model = "KNN", imputer_configs = hparameters)
-mli_knn.fit_imput(X = train)
-train_knn = mli_knn.transform_imput(X = train)
-test_knn = mli_knn.transform_imput(X = test)
-
-# Imputation Example 2 : RandomForest
-
-mli_rf = MLimputer(imput_model = "RandomForest", imputer_configs = hparameters)
-mli_rf.fit_imput(X = train)
-train_rf = mli_rf.transform_imput(X = train)
-test_rf = mli_rf.transform_imput(X = test)
+imputer_rf=mli.fit_imput(dataset=train,imput_model="RandomForest",imputer_configs=hparameters)
+train_rf=mli.transform_imput(dataset=train,fit_configs=imputer_rf)
+test_rf=mli.transform_imput(dataset=test,fit_configs=imputer_rf)
+
+# Imputation Example 2 : KNN
+
+imputer_knn=mli.fit_imput(dataset=train,imput_model="KNN",imputer_configs=hparameters)
+train_knn=mli.transform_imput(dataset=train,fit_configs=imputer_knn)
+test_knn=mli.transform_imput(dataset=test,fit_configs=imputer_knn)
     
 #(...)
     
-## Performance Evaluation Regression - Imputation CrossValidation Example
+## Performance Evaluation Example - Imputation CrossValidation
 
 from sklearn.linear_model import LinearRegression
 from sklearn.ensemble import RandomForestRegressor
 from catboost import CatBoostRegressor
         
-leaderboard_rf_imp=ms.cross_validation(X = train_rf,
-                                       target = "Target_Name_Col", 
-                                       test_size = 0.2,
-                                       n_splits = 3,
-                                       models = [LinearRegression(), RandomForestRegressor(), CatBoostRegressor()])
+leaderboard_knn_imp=mli.cross_validation(dataset=train_knn,
+                                         target="Target_Name_Col", 
+                                         test_size=0.2,
+                                         n_splits=3,
+                                         models=[LinearRegression(), RandomForestRegressor(), CatBoostRegressor()])
 
 ## Export Imputation Metadata
 
-# Imputation Metadata
+# KNN Imputation Metadata
 import pickle 
-output = open("imputer_rf.pkl", 'wb')
-pickle.dump(mli_rf, output)
+output = open("imputer_knn.pkl", 'wb')
+pickle.dump(imputer_knn, output)
 
 ```  
     
 ## License
 
 Distributed under the MIT License. See [LICENSE](https://github.com/TsLu1s/TSForecasting/blob/main/LICENSE) for more information.
```

