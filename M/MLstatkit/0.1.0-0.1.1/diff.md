# Comparing `tmp/MLstatkit-0.1.0.tar.gz` & `tmp/MLstatkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLstatkit-0.1.0.tar", last modified: Mon Apr  1 20:46:04 2024, max compression
+gzip compressed data, was "MLstatkit-0.1.1.tar", last modified: Mon Apr  1 21:29:23 2024, max compression
```

## Comparing `MLstatkit-0.1.0.tar` & `MLstatkit-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 20:46:04.230414 MLstatkit-0.1.0/
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     1072 2024-04-01 20:44:17.000000 MLstatkit-0.1.0/LICENSE
-drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 20:46:04.229452 MLstatkit-0.1.0/MLstatkit/
--rw-r--r--   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 20:44:17.000000 MLstatkit-0.1.0/MLstatkit/__init__.py
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     6374 2024-04-01 20:44:17.000000 MLstatkit-0.1.0/MLstatkit/stats.py
-drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 20:46:04.230101 MLstatkit-0.1.0/MLstatkit.egg-info/
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     7416 2024-04-01 20:46:03.000000 MLstatkit-0.1.0/MLstatkit.egg-info/PKG-INFO
--rw-r--r--   0 brritanyhuang   (501) staff       (20)      231 2024-04-01 20:46:04.000000 MLstatkit-0.1.0/MLstatkit.egg-info/SOURCES.txt
--rw-r--r--   0 brritanyhuang   (501) staff       (20)        1 2024-04-01 20:46:03.000000 MLstatkit-0.1.0/MLstatkit.egg-info/dependency_links.txt
--rw-r--r--   0 brritanyhuang   (501) staff       (20)       32 2024-04-01 20:46:04.000000 MLstatkit-0.1.0/MLstatkit.egg-info/requires.txt
--rw-r--r--   0 brritanyhuang   (501) staff       (20)       10 2024-04-01 20:46:04.000000 MLstatkit-0.1.0/MLstatkit.egg-info/top_level.txt
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     7416 2024-04-01 20:46:04.230275 MLstatkit-0.1.0/PKG-INFO
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     6526 2024-04-01 20:45:33.000000 MLstatkit-0.1.0/README.md
--rw-r--r--   0 brritanyhuang   (501) staff       (20)       38 2024-04-01 20:46:04.230458 MLstatkit-0.1.0/setup.cfg
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     1236 2024-04-01 20:44:17.000000 MLstatkit-0.1.0/setup.py
+drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 21:29:23.069870 MLstatkit-0.1.1/
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     1072 2024-04-01 20:44:17.000000 MLstatkit-0.1.1/LICENSE
+drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 21:29:23.069036 MLstatkit-0.1.1/MLstatkit/
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 20:44:17.000000 MLstatkit-0.1.1/MLstatkit/__init__.py
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     6374 2024-04-01 20:44:17.000000 MLstatkit-0.1.1/MLstatkit/stats.py
+drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 21:29:23.069578 MLstatkit-0.1.1/MLstatkit.egg-info/
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     7426 2024-04-01 21:29:22.000000 MLstatkit-0.1.1/MLstatkit.egg-info/PKG-INFO
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)      231 2024-04-01 21:29:23.000000 MLstatkit-0.1.1/MLstatkit.egg-info/SOURCES.txt
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)        1 2024-04-01 21:29:22.000000 MLstatkit-0.1.1/MLstatkit.egg-info/dependency_links.txt
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)       32 2024-04-01 21:29:22.000000 MLstatkit-0.1.1/MLstatkit.egg-info/requires.txt
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)       10 2024-04-01 21:29:22.000000 MLstatkit-0.1.1/MLstatkit.egg-info/top_level.txt
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     7426 2024-04-01 21:29:23.069741 MLstatkit-0.1.1/PKG-INFO
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     6379 2024-04-01 21:28:23.000000 MLstatkit-0.1.1/README.md
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)       38 2024-04-01 21:29:23.069912 MLstatkit-0.1.1/setup.cfg
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     1390 2024-04-01 21:07:40.000000 MLstatkit-0.1.1/setup.py
```

### Comparing `MLstatkit-0.1.0/LICENSE` & `MLstatkit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MLstatkit-0.1.0/MLstatkit/stats.py` & `MLstatkit-0.1.1/MLstatkit/stats.py`

 * *Files identical despite different names*

### Comparing `MLstatkit-0.1.0/MLstatkit.egg-info/PKG-INFO` & `MLstatkit-0.1.1/MLstatkit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 Metadata-Version: 2.1
 Name: MLstatkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: MLstatkit is a comprehensive Python library designed to seamlessly integrate established statistical methods into machine learning projects.
 Home-page: https://github.com/Brritany/MLstatkit
 Author: Yong-Zhen Huang
 Author-email: m946111005@tmu.edu.tw
 License: UNKNOWN
 Project-URL: Tracker, https://github.com/Brritany/MLstatkit/issues
 Keywords: python,statistics,Delong test,Bootstrapping
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![PyPI - Version](https://img.shields.io/pypi/v/MLStats)
-![PyPI - License](https://img.shields.io/pypi/l/MLStats)
-![PyPI - Status](https://img.shields.io/pypi/status/MLStats)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/MLStats)
-![PyPI - Download](https://img.shields.io/pypi/dm/MLStats)
-![PyPI - Implementation](https://img.shields.io/pypi/implementation/MLStats)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/MLStats)
-[![Downloads](https://static.pepy.tech/badge/MLStats)](https://pepy.tech/project/MLStats)
+![PyPI - Version](https://img.shields.io/pypi/v/MLstatkit)
+![PyPI - License](https://img.shields.io/pypi/l/MLstatkit)
+![PyPI - Status](https://img.shields.io/pypi/status/MLstatkit)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/MLstatkit)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/MLstatkit)
 
 # MLstatkit
 
 MLstatkit is a comprehensive Python library designed to seamlessly integrate established statistical methods into machine learning projects. It encompasses a variety of tools, including **Delong's test** for comparing AUCs and **Bootstrapping** for calculating confidence intervals, among others. With its modular design, MLstatkit offers researchers and data scientists a flexible and powerful toolkit to augment their analyses and model evaluations, catering to a broad spectrum of statistical testing needs within the domain of machine learning.
 
 ## Installation
 
-Install MLstatkit directly from TestPyPI using pip:
+Install MLstatkit directly from PyPI using pip:
 
 ```bash
-pip install -i https://test.pypi.org/simple/ MLstatkit
+pip install MLstatkit
 ```
 
 ## Usage
 
 ### Delong's Test
 
 `Delong_test` function allows for statistical comparison of AUCs from two different models, providing insights into their performance differences.
@@ -154,9 +154,12 @@
 
 We welcome contributions to MLstatkit! Please see our contribution guidelines for more details.
 
 ## License
 
 MLstatkit is distributed under the MIT License. For more information, see the LICENSE file in the GitHub repository.
 
+### Update log
 
+- `0.1.1`  Update `README.md`, `setup.py`. Add `CONTRIBUTING.md`.
+- `0.1.0`  First edition
```

### Comparing `MLstatkit-0.1.0/PKG-INFO` & `MLstatkit-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 Metadata-Version: 2.1
 Name: MLstatkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: MLstatkit is a comprehensive Python library designed to seamlessly integrate established statistical methods into machine learning projects.
 Home-page: https://github.com/Brritany/MLstatkit
 Author: Yong-Zhen Huang
 Author-email: m946111005@tmu.edu.tw
 License: UNKNOWN
 Project-URL: Tracker, https://github.com/Brritany/MLstatkit/issues
 Keywords: python,statistics,Delong test,Bootstrapping
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![PyPI - Version](https://img.shields.io/pypi/v/MLStats)
-![PyPI - License](https://img.shields.io/pypi/l/MLStats)
-![PyPI - Status](https://img.shields.io/pypi/status/MLStats)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/MLStats)
-![PyPI - Download](https://img.shields.io/pypi/dm/MLStats)
-![PyPI - Implementation](https://img.shields.io/pypi/implementation/MLStats)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/MLStats)
-[![Downloads](https://static.pepy.tech/badge/MLStats)](https://pepy.tech/project/MLStats)
+![PyPI - Version](https://img.shields.io/pypi/v/MLstatkit)
+![PyPI - License](https://img.shields.io/pypi/l/MLstatkit)
+![PyPI - Status](https://img.shields.io/pypi/status/MLstatkit)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/MLstatkit)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/MLstatkit)
 
 # MLstatkit
 
 MLstatkit is a comprehensive Python library designed to seamlessly integrate established statistical methods into machine learning projects. It encompasses a variety of tools, including **Delong's test** for comparing AUCs and **Bootstrapping** for calculating confidence intervals, among others. With its modular design, MLstatkit offers researchers and data scientists a flexible and powerful toolkit to augment their analyses and model evaluations, catering to a broad spectrum of statistical testing needs within the domain of machine learning.
 
 ## Installation
 
-Install MLstatkit directly from TestPyPI using pip:
+Install MLstatkit directly from PyPI using pip:
 
 ```bash
-pip install -i https://test.pypi.org/simple/ MLstatkit
+pip install MLstatkit
 ```
 
 ## Usage
 
 ### Delong's Test
 
 `Delong_test` function allows for statistical comparison of AUCs from two different models, providing insights into their performance differences.
@@ -154,9 +154,12 @@
 
 We welcome contributions to MLstatkit! Please see our contribution guidelines for more details.
 
 ## License
 
 MLstatkit is distributed under the MIT License. For more information, see the LICENSE file in the GitHub repository.
 
+### Update log
 
+- `0.1.1`  Update `README.md`, `setup.py`. Add `CONTRIBUTING.md`.
+- `0.1.0`  First edition
```

### Comparing `MLstatkit-0.1.0/README.md` & `MLstatkit-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-![PyPI - Version](https://img.shields.io/pypi/v/MLStats)
-![PyPI - License](https://img.shields.io/pypi/l/MLStats)
-![PyPI - Status](https://img.shields.io/pypi/status/MLStats)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/MLStats)
-![PyPI - Download](https://img.shields.io/pypi/dm/MLStats)
-![PyPI - Implementation](https://img.shields.io/pypi/implementation/MLStats)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/MLStats)
-[![Downloads](https://static.pepy.tech/badge/MLStats)](https://pepy.tech/project/MLStats)
+![PyPI - Version](https://img.shields.io/pypi/v/MLstatkit)
+![PyPI - License](https://img.shields.io/pypi/l/MLstatkit)
+![PyPI - Status](https://img.shields.io/pypi/status/MLstatkit)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/MLstatkit)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/MLstatkit)
 
 # MLstatkit
 
 MLstatkit is a comprehensive Python library designed to seamlessly integrate established statistical methods into machine learning projects. It encompasses a variety of tools, including **Delong's test** for comparing AUCs and **Bootstrapping** for calculating confidence intervals, among others. With its modular design, MLstatkit offers researchers and data scientists a flexible and powerful toolkit to augment their analyses and model evaluations, catering to a broad spectrum of statistical testing needs within the domain of machine learning.
 
 ## Installation
 
-Install MLstatkit directly from TestPyPI using pip:
+Install MLstatkit directly from PyPI using pip:
 
 ```bash
-pip install -i https://test.pypi.org/simple/ MLstatkit
+pip install MLstatkit
 ```
 
 ## Usage
 
 ### Delong's Test
 
 `Delong_test` function allows for statistical comparison of AUCs from two different models, providing insights into their performance differences.
@@ -133,7 +130,11 @@
 
 We welcome contributions to MLstatkit! Please see our contribution guidelines for more details.
 
 ## License
 
 MLstatkit is distributed under the MIT License. For more information, see the LICENSE file in the GitHub repository.
 
+### Update log
+
+- `0.1.1`  Update `README.md`, `setup.py`. Add `CONTRIBUTING.md`.
+- `0.1.0`  First edition
```

### Comparing `MLstatkit-0.1.0/setup.py` & `MLstatkit-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="MLstatkit",
-    version="0.1.0",
+    version="0.1.1",
     description="MLstatkit is a comprehensive Python library designed to seamlessly integrate established statistical methods into machine learning projects.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Brritany/MLstatkit',
     project_urls={
         'Tracker': 'https://github.com/Brritany/MLstatkit/issues',
     },
@@ -20,14 +20,17 @@
     install_requires=[
         "pandas", "numpy", "scipy", "scikit-learn"
     ],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
+        "Natural Language :: English",
+        "Topic :: Scientific/Engineering",
+        "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
 )
```

