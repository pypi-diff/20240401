# Comparing `tmp/tsclassification-1.0.1.tar.gz` & `tmp/tsclassification-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsclassification-1.0.1.tar", last modified: Mon Jun 19 21:11:17 2023, max compression
+gzip compressed data, was "tsclassification-1.1.1.tar", last modified: Mon Apr  1 21:43:12 2024, max compression
```

## Comparing `tsclassification-1.0.1.tar` & `tsclassification-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-19 21:11:17.315554 tsclassification-1.0.1/
--rw-r--r--   0 grant      (501) staff       (20)     1068 2023-06-19 19:37:09.000000 tsclassification-1.0.1/LICENSE
--rw-r--r--   0 grant      (501) staff       (20)      905 2023-06-19 21:11:17.315684 tsclassification-1.0.1/PKG-INFO
--rw-r--r--   0 grant      (501) staff       (20)     1950 2023-06-19 21:01:52.000000 tsclassification-1.0.1/README.md
--rw-r--r--   0 grant      (501) staff       (20)       79 2023-06-19 21:11:17.316117 tsclassification-1.0.1/setup.cfg
--rw-r--r--   0 grant      (501) staff       (20)     1029 2023-06-19 20:11:35.000000 tsclassification-1.0.1/setup.py
-drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-19 21:11:17.313416 tsclassification-1.0.1/tsclassification/
--rw-r--r--   0 grant      (501) staff       (20)       58 2023-06-19 21:07:17.000000 tsclassification-1.0.1/tsclassification/__init__.py
--rw-r--r--   0 grant      (501) staff       (20)     4600 2023-06-19 21:00:32.000000 tsclassification-1.0.1/tsclassification/classifier.py
--rw-r--r--   0 grant      (501) staff       (20)     2213 2023-06-19 18:59:54.000000 tsclassification-1.0.1/tsclassification/sample_methods.py
-drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-19 21:11:17.315337 tsclassification-1.0.1/tsclassification.egg-info/
--rw-r--r--   0 grant      (501) staff       (20)      905 2023-06-19 21:11:17.000000 tsclassification-1.0.1/tsclassification.egg-info/PKG-INFO
--rw-r--r--   0 grant      (501) staff       (20)      330 2023-06-19 21:11:17.000000 tsclassification-1.0.1/tsclassification.egg-info/SOURCES.txt
--rw-r--r--   0 grant      (501) staff       (20)        1 2023-06-19 21:11:17.000000 tsclassification-1.0.1/tsclassification.egg-info/dependency_links.txt
--rw-r--r--   0 grant      (501) staff       (20)       25 2023-06-19 21:11:17.000000 tsclassification-1.0.1/tsclassification.egg-info/requires.txt
--rw-r--r--   0 grant      (501) staff       (20)       17 2023-06-19 21:11:17.000000 tsclassification-1.0.1/tsclassification.egg-info/top_level.txt
+drwxr-xr-x   0 grant      (501) staff       (20)        0 2024-04-01 21:43:12.384106 tsclassification-1.1.1/
+-rw-r--r--   0 grant      (501) staff       (20)     1068 2024-02-14 17:21:36.000000 tsclassification-1.1.1/LICENSE
+-rw-r--r--   0 grant      (501) staff       (20)      755 2024-04-01 21:43:12.384157 tsclassification-1.1.1/PKG-INFO
+-rw-r--r--   0 grant      (501) staff       (20)     5396 2024-04-01 21:28:25.000000 tsclassification-1.1.1/README.md
+-rw-r--r--   0 grant      (501) staff       (20)       79 2024-04-01 21:43:12.384312 tsclassification-1.1.1/setup.cfg
+-rw-r--r--   0 grant      (501) staff       (20)      934 2024-04-01 21:42:10.000000 tsclassification-1.1.1/setup.py
+drwxr-xr-x   0 grant      (501) staff       (20)        0 2024-04-01 21:43:12.383597 tsclassification-1.1.1/tsclassification/
+-rw-r--r--   0 grant      (501) staff       (20)       42 2024-02-17 20:53:07.000000 tsclassification-1.1.1/tsclassification/__init__.py
+-rw-r--r--   0 grant      (501) staff       (20)     9887 2024-04-01 18:08:17.000000 tsclassification-1.1.1/tsclassification/classifier.py
+-rw-r--r--   0 grant      (501) staff       (20)     2564 2024-03-05 04:39:34.000000 tsclassification-1.1.1/tsclassification/sample_methods.py
+drwxr-xr-x   0 grant      (501) staff       (20)        0 2024-04-01 21:43:12.384031 tsclassification-1.1.1/tsclassification.egg-info/
+-rw-r--r--   0 grant      (501) staff       (20)      755 2024-04-01 21:43:12.000000 tsclassification-1.1.1/tsclassification.egg-info/PKG-INFO
+-rw-r--r--   0 grant      (501) staff       (20)      330 2024-04-01 21:43:12.000000 tsclassification-1.1.1/tsclassification.egg-info/SOURCES.txt
+-rw-r--r--   0 grant      (501) staff       (20)        1 2024-04-01 21:43:12.000000 tsclassification-1.1.1/tsclassification.egg-info/dependency_links.txt
+-rw-r--r--   0 grant      (501) staff       (20)       25 2024-04-01 21:43:12.000000 tsclassification-1.1.1/tsclassification.egg-info/requires.txt
+-rw-r--r--   0 grant      (501) staff       (20)       17 2024-04-01 21:43:12.000000 tsclassification-1.1.1/tsclassification.egg-info/top_level.txt
```

### Comparing `tsclassification-1.0.1/LICENSE` & `tsclassification-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsclassification-1.0.1/PKG-INFO` & `tsclassification-1.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 Metadata-Version: 2.1
 Name: tsclassification
-Version: 1.0.1
+Version: 1.1.1
 Summary: A shapelet classifier for time series data.
 Home-page: https://github.com/gellison321/tsclassification
+Download-URL: https://github.com/gellison321/tsclassification/releases/tag/1.1.1.tar.gz
 Author: Grant Ellison
 Author-email: gellison321@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/gellison321/tsclassification/archive/refs/tags/1.0.1.tar.gz
 Keywords: timeseries,data science,data analysis,classificaiton,machine learning
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `tsclassification-1.0.1/setup.py` & `tsclassification-1.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
   name = 'tsclassification',
   packages = find_packages(),
-  version = '1.0.1',
+  version = '1.1.1',
   license='',
   description = 'A shapelet classifier for time series data.',
   author = 'Grant Ellison',
   author_email = 'gellison321@gmail.com',
   url = 'https://github.com/gellison321/tsclassification',
-  download_url = 'https://github.com/gellison321/tsclassification/archive/refs/tags/1.0.1.tar.gz',
+  download_url = 'https://github.com/gellison321/tsclassification/releases/tag/1.1.1.tar.gz',
   keywords = ['timeseries', 'data science','data analysis', 'classificaiton', 'machine learning'],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Topic :: Software Development :: Build Tools',
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
   ],
   install_requires=['numpy', 'sklearn', 'tsshapelet'],
 )
```

### Comparing `tsclassification-1.0.1/tsclassification/sample_methods.py` & `tsclassification-1.1.1/tsclassification/sample_methods.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,78 @@
 import numpy as np
+from numpy.lib.stride_tricks import as_strided
 
 # Bootstrapped subsequence sampling from a stepped sliding window, with a random initialization
-def sample_slide_comile(X, Y, window, step = 1, sample = 100):
+def bootstrapped(X, Y, window = 100, step = 1, qty = 1000):
+
     data = []
     labels = []
     for label in np.unique(Y):
         x = X[np.where(Y == label)[0]]
         y = Y[np.where(Y == label)[0]]
         temp_data = []
         temp_labels = []
         if len(x)>0:
             a = 0
-            while len(temp_data)<sample:
+            while len(temp_data)<qty:
                 rano = np.random.randint(0, len(x)) if a != 0 else a
                 a += 1
                 for i in range(rano, len(x) - window, step):
-                    if len(temp_data)>=sample:
+                    if len(temp_data)>=qty:
                         break
                     temp_labels.append(y[i])
                     temp_data.append(np.array(x[i:i+window]))
-            data.extend(temp_data[:sample])
-            labels.extend(temp_labels[:sample])
+            data.extend(temp_data[:qty])
+            labels.extend(temp_labels[:qty])
+
     return data, labels
 
 # Simple stepped sliding window for subsequence extraction
-def slide_compile(X, Y, window, step = 1, sample = 100):
+def slide(X, Y, window = 100, step = 1, qty = 1000):
+
     data = []
     labels = []
     for label in np.unique(Y):
         x = X[np.where(Y == label)[0]]
         y = Y[np.where(Y == label)[0]]
         temp_data = []
         temp_labels = []
         for i in range(0, len(x) - window, step):
-            if len(temp_data) >= sample:
+            if len(temp_data) >= qty:
                 break
-            temp_labels.append(y)
             temp_data.append(np.array(x[i:i+window]))
-        data.extend(temp_data[:sample])
-        labels.extend(temp_labels[:sample])
+            temp_labels.append(y[i])
+        data.extend(temp_data[:qty])
+        labels.extend(temp_labels[:qty])
+
     return data, labels
 
 # Extracts randomly positioned subsequences
-def random_compile(X, Y, window, sample = 300, step = 1):
+def random(X, Y, window = 100, qty = 1000):
+    
     data = []
     labels = []
     for label in np.unique(Y):
         x = X[np.where(Y == label)[0]]
         y = Y[np.where(Y == label)[0]]
         if len(x) > window:
-            for n in range(sample):
+            for n in range(qty):
                 indexer = np.random.randint(window//2, len(x) - window//2)
                 series = x[indexer-window//2:indexer+window//2]
                 data.append(np.array(series))
                 labels.append(y[indexer])
 
     return data, labels
 
-compilers = {'random' : random_compile,
-             'slide' : slide_compile,
-             'sample_slide' : sample_slide_comile,
-            }
+def compiler(X, y, method = 'slide', window = 100, step = 1, qty = 1000):
+
+    if method == 'slide':
+        return slide(X, y, window = window, step = step, qty = qty)
+    
+    elif method == 'random':
+        return random(X, y, window = window, qty = qty)
+    
+    elif method == 'bootstrapped':
+        return bootstrapped(X, y, window = window, step = step, qty = qty)
+        
+    else:
+        raise ValueError('Only slide, random and bootstrapped methods are supported')
```

### Comparing `tsclassification-1.0.1/tsclassification.egg-info/PKG-INFO` & `tsclassification-1.1.1/tsclassification.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 Metadata-Version: 2.1
 Name: tsclassification
-Version: 1.0.1
+Version: 1.1.1
 Summary: A shapelet classifier for time series data.
 Home-page: https://github.com/gellison321/tsclassification
+Download-URL: https://github.com/gellison321/tsclassification/releases/tag/1.1.1.tar.gz
 Author: Grant Ellison
 Author-email: gellison321@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/gellison321/tsclassification/archive/refs/tags/1.0.1.tar.gz
 Keywords: timeseries,data science,data analysis,classificaiton,machine learning
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
-
-UNKNOWN
-
```

