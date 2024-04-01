# Comparing `tmp/wolta-0.1.1.tar.gz` & `tmp/wolta-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolta-0.1.1.tar", last modified: Sun Mar 31 16:15:14 2024, max compression
+gzip compressed data, was "wolta-0.1.2.tar", last modified: Mon Apr  1 16:20:19 2024, max compression
```

## Comparing `wolta-0.1.1.tar` & `wolta-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 16:15:14.180696 wolta-0.1.1/
--rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0    12623 2024-03-31 16:15:14.179603 wolta-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    11496 2024-03-31 10:19:37.000000 wolta-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-03-31 16:15:14.180696 wolta-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1185 2024-03-31 11:58:39.000000 wolta-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:15:14.133602 wolta-0.1.1/wolta/
--rw-rw-rw-   0        0        0      113 2024-03-31 11:58:39.000000 wolta-0.1.1/wolta/__init__.py
--rw-rw-rw-   0        0        0     7506 2024-03-31 09:38:42.000000 wolta-0.1.1/wolta/data_tools.py
--rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.1.1/wolta/feature_tools.py
--rw-rw-rw-   0        0        0     4332 2024-03-30 23:38:39.000000 wolta-0.1.1/wolta/model_tools.py
--rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.1.1/wolta/progressive_tools.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:15:14.178599 wolta-0.1.1/wolta.egg-info/
--rw-rw-rw-   0        0        0    12623 2024-03-31 16:15:14.000000 wolta-0.1.1/wolta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-03-31 16:15:14.000000 wolta-0.1.1/wolta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 16:15:14.000000 wolta-0.1.1/wolta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-03-31 16:15:14.000000 wolta-0.1.1/wolta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       61 2024-03-31 16:15:14.000000 wolta-0.1.1/wolta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 16:20:19.097100 wolta-0.1.2/
+-rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    13850 2024-04-01 16:20:19.096029 wolta-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    12695 2024-04-01 16:18:46.000000 wolta-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-01 16:20:19.097100 wolta-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1185 2024-04-01 16:19:12.000000 wolta-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:20:19.057578 wolta-0.1.2/wolta/
+-rw-rw-rw-   0        0        0      113 2024-03-31 11:58:39.000000 wolta-0.1.2/wolta/__init__.py
+-rw-rw-rw-   0        0        0     7562 2024-04-01 16:18:15.000000 wolta-0.1.2/wolta/data_tools.py
+-rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.1.2/wolta/feature_tools.py
+-rw-rw-rw-   0        0        0     4332 2024-03-30 23:38:39.000000 wolta-0.1.2/wolta/model_tools.py
+-rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.1.2/wolta/progressive_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:20:19.094949 wolta-0.1.2/wolta.egg-info/
+-rw-rw-rw-   0        0        0    13850 2024-04-01 16:20:18.000000 wolta-0.1.2/wolta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-01 16:20:18.000000 wolta-0.1.2/wolta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 16:20:18.000000 wolta-0.1.2/wolta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-01 16:20:18.000000 wolta-0.1.2/wolta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       61 2024-04-01 16:20:18.000000 wolta-0.1.2/wolta.egg-info/top_level.txt
```

### Comparing `wolta-0.1.1/LICENSE.txt` & `wolta-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wolta-0.1.1/PKG-INFO` & `wolta-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.1.1
+Version: 0.1.2
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 Requires-Dist: hyperopt
 
 
 # WOLTA DOCUMENTATION
 
 Wolta is designed for making simplify the frequently used processes which includes Pandas, Numpy and Scikit-Learn in Machine Learning.
 <br><br>
-Currently there are three modules inside the library, which are 'data_tools', 'model_tools' and 'progressive_tools'
+Currently there are four modules inside the library, which are 'data_tools', 'model_tools', 'progressive_tools' and 'feature_tools'
 
 ## Installation
 
 ```
 pip install wolta
 ```
 
@@ -42,14 +42,15 @@
 **Parameters**:
 <br>
 * paths, _python list_
 * strategy, {'default', 'efficient'}, by default, 'default'
 * deleted_columns, _python string list_, by default, None
 * print_description, _boolean_, by default, False
 * shuffle, _boolean_ , by default, False
+* encoding, _string_, by default, 'utf-8'
 
 1. _paths_ holds the locations of data files.
 <br>
 2. If _strategy_ is 'default', then the datatypes of columns are assigned with maximum bytes (64).
 <br>
 3. If _strategy_ is 'efficient', then the each column is examined and the min-max values are detected. According to the info, least required byte amount is assigned to each column.
 <br>
@@ -470,8 +471,35 @@
 
 X_test = np.load('x_test.npy')
 y_test = np.load('x_test.npy')
 
 paths = glob.glob('path/to/dir/*.csv')
 
 percentage_log, metrics_log = path_chain(paths, RandomForestClassifier, X_test, y_test, 'output')
-```
+```
+
+***
+
+## Feature Tools
+
+This module is about to manipulating features in datasets.
+
+### quest_selection
+
+Prints out suggestions about what feature(s) can be deleted with less loss or maximum gain.
+
+The algorithm works with two steps: Firstly, It removes one feature for each time and compares accuracies between current situation and whole-features case. If new accuracy is the better than whole-feature one or their difference less-equal than flag_one_tol, it passes to the second step.
+<br>
+The next process 'trials' times creates combinations with random amounts of passed features and they are removed at same time. If new accuracy is the better than whole-feature one or their difference less-equal than fin_tol, it becomes a suggestion.
+
+**Parameters**:
+* model_class
+* X_train
+* y_train
+* X_test
+* y_test
+* features, list of string, holds column names for X.
+* flag_one_tol, float
+* fin_tol, float
+* params, dictionary, if model has parameters, they initialize it here, default by, None
+* normal_acc, float, default by, None. If it is None then it is calculated first of all
+* trials, int, default by, 100
```

### Comparing `wolta-0.1.1/README.md` & `wolta-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # WOLTA DOCUMENTATION
 
 Wolta is designed for making simplify the frequently used processes which includes Pandas, Numpy and Scikit-Learn in Machine Learning.
 <br><br>
-Currently there are three modules inside the library, which are 'data_tools', 'model_tools' and 'progressive_tools'
+Currently there are four modules inside the library, which are 'data_tools', 'model_tools', 'progressive_tools' and 'feature_tools'
 
 ## Installation
 
 ```
 pip install wolta
 ```
 
@@ -21,14 +21,15 @@
 **Parameters**:
 <br>
 * paths, _python list_
 * strategy, {'default', 'efficient'}, by default, 'default'
 * deleted_columns, _python string list_, by default, None
 * print_description, _boolean_, by default, False
 * shuffle, _boolean_ , by default, False
+* encoding, _string_, by default, 'utf-8'
 
 1. _paths_ holds the locations of data files.
 <br>
 2. If _strategy_ is 'default', then the datatypes of columns are assigned with maximum bytes (64).
 <br>
 3. If _strategy_ is 'efficient', then the each column is examined and the min-max values are detected. According to the info, least required byte amount is assigned to each column.
 <br>
@@ -449,8 +450,35 @@
 
 X_test = np.load('x_test.npy')
 y_test = np.load('x_test.npy')
 
 paths = glob.glob('path/to/dir/*.csv')
 
 percentage_log, metrics_log = path_chain(paths, RandomForestClassifier, X_test, y_test, 'output')
-```
+```
+
+***
+
+## Feature Tools
+
+This module is about to manipulating features in datasets.
+
+### quest_selection
+
+Prints out suggestions about what feature(s) can be deleted with less loss or maximum gain.
+
+The algorithm works with two steps: Firstly, It removes one feature for each time and compares accuracies between current situation and whole-features case. If new accuracy is the better than whole-feature one or their difference less-equal than flag_one_tol, it passes to the second step.
+<br>
+The next process 'trials' times creates combinations with random amounts of passed features and they are removed at same time. If new accuracy is the better than whole-feature one or their difference less-equal than fin_tol, it becomes a suggestion.
+
+**Parameters**:
+* model_class
+* X_train
+* y_train
+* X_test
+* y_test
+* features, list of string, holds column names for X.
+* flag_one_tol, float
+* fin_tol, float
+* params, dictionary, if model has parameters, they initialize it here, default by, None
+* normal_acc, float, default by, None. If it is None then it is calculated first of all
+* trials, int, default by, 100
```

### Comparing `wolta-0.1.1/setup.py` & `wolta-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'Data Science Library'
 LONG_DESCRIPTION = 'A package for data science'
 
 setup(
     name="wolta",
     version=VERSION,
     author="iamalreadynoob",
```

### Comparing `wolta-0.1.1/wolta/data_tools.py` & `wolta-0.1.2/wolta/data_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,22 +156,22 @@
 
             if sub_min < min_val[i]:
                 min_val[i] = sub_min
 
     return columns, types, max_val, min_val
 
 
-def load_by_parts(paths, strategy='default', deleted_columns=None, print_description=False, shuffle=False):
+def load_by_parts(paths, strategy='default', deleted_columns=None, print_description=False, shuffle=False, encoding='utf-8'):
     import pandas as pd
 
     if strategy == 'default':
         dfs = []
         loc = 0
         for path in paths:
-            df = pd.read_csv(path)
+            df = pd.read_csv(path, encoding=encoding)
 
             if deleted_columns is not None:
                 for col in deleted_columns:
                     del df[col]
 
             if shuffle:
                 df = df.sample(frac=1).reset_index(drop=True)
@@ -213,15 +213,15 @@
 
         del numeric_columns, max_val, min_val, types
 
         dfs = []
         loc = 0
 
         for path in paths:
-            df = pd.read_csv(path, dtype=dtype)
+            df = pd.read_csv(path, dtype=dtype, encoding=encoding)
 
             if deleted_columns is not None:
                 for col in deleted_columns:
                     del df[col]
 
             if shuffle:
                 df = df.sample(frac=1).reset_index(drop=True)
```

### Comparing `wolta-0.1.1/wolta/feature_tools.py` & `wolta-0.1.2/wolta/feature_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.1/wolta/model_tools.py` & `wolta-0.1.2/wolta/model_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.1/wolta/progressive_tools.py` & `wolta-0.1.2/wolta/progressive_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.1/wolta.egg-info/PKG-INFO` & `wolta-0.1.2/wolta.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.1.1
+Version: 0.1.2
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 Requires-Dist: hyperopt
 
 
 # WOLTA DOCUMENTATION
 
 Wolta is designed for making simplify the frequently used processes which includes Pandas, Numpy and Scikit-Learn in Machine Learning.
 <br><br>
-Currently there are three modules inside the library, which are 'data_tools', 'model_tools' and 'progressive_tools'
+Currently there are four modules inside the library, which are 'data_tools', 'model_tools', 'progressive_tools' and 'feature_tools'
 
 ## Installation
 
 ```
 pip install wolta
 ```
 
@@ -42,14 +42,15 @@
 **Parameters**:
 <br>
 * paths, _python list_
 * strategy, {'default', 'efficient'}, by default, 'default'
 * deleted_columns, _python string list_, by default, None
 * print_description, _boolean_, by default, False
 * shuffle, _boolean_ , by default, False
+* encoding, _string_, by default, 'utf-8'
 
 1. _paths_ holds the locations of data files.
 <br>
 2. If _strategy_ is 'default', then the datatypes of columns are assigned with maximum bytes (64).
 <br>
 3. If _strategy_ is 'efficient', then the each column is examined and the min-max values are detected. According to the info, least required byte amount is assigned to each column.
 <br>
@@ -470,8 +471,35 @@
 
 X_test = np.load('x_test.npy')
 y_test = np.load('x_test.npy')
 
 paths = glob.glob('path/to/dir/*.csv')
 
 percentage_log, metrics_log = path_chain(paths, RandomForestClassifier, X_test, y_test, 'output')
-```
+```
+
+***
+
+## Feature Tools
+
+This module is about to manipulating features in datasets.
+
+### quest_selection
+
+Prints out suggestions about what feature(s) can be deleted with less loss or maximum gain.
+
+The algorithm works with two steps: Firstly, It removes one feature for each time and compares accuracies between current situation and whole-features case. If new accuracy is the better than whole-feature one or their difference less-equal than flag_one_tol, it passes to the second step.
+<br>
+The next process 'trials' times creates combinations with random amounts of passed features and they are removed at same time. If new accuracy is the better than whole-feature one or their difference less-equal than fin_tol, it becomes a suggestion.
+
+**Parameters**:
+* model_class
+* X_train
+* y_train
+* X_test
+* y_test
+* features, list of string, holds column names for X.
+* flag_one_tol, float
+* fin_tol, float
+* params, dictionary, if model has parameters, they initialize it here, default by, None
+* normal_acc, float, default by, None. If it is None then it is calculated first of all
+* trials, int, default by, 100
```

