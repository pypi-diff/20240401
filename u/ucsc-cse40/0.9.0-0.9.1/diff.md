# Comparing `tmp/ucsc-cse40-0.9.0.tar.gz` & `tmp/ucsc-cse40-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucsc-cse40-0.9.0.tar", last modified: Tue Jan  2 13:58:35 2024, max compression
+gzip compressed data, was "ucsc-cse40-0.9.1.tar", last modified: Mon Apr  1 20:07:11 2024, max compression
```

## Comparing `ucsc-cse40-0.9.0.tar` & `ucsc-cse40-0.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-01-02 13:58:35.646673 ucsc-cse40-0.9.0/
--rw-r--r--   0 eriq      (1000) eriq      (1000)     1590 2024-01-02 13:58:35.646673 ucsc-cse40-0.9.0/PKG-INFO
--rw-rw----   0 eriq      (1000) eriq      (1000)      851 2024-01-02 12:58:26.000000 ucsc-cse40-0.9.0/README.md
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-01-02 13:58:35.643340 ucsc-cse40-0.9.0/cse40/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2023-05-17 17:36:49.000000 ucsc-cse40-0.9.0/cse40/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)       38 2024-01-02 13:58:35.646673 ucsc-cse40-0.9.0/setup.cfg
--rw-rw----   0 eriq      (1000) eriq      (1000)     1362 2024-01-02 12:58:11.000000 ucsc-cse40-0.9.0/setup.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-01-02 13:58:35.646673 ucsc-cse40-0.9.0/ucsc_cse40.egg-info/
--rw-r--r--   0 eriq      (1000) eriq      (1000)     1590 2024-01-02 13:58:35.000000 ucsc-cse40-0.9.0/ucsc_cse40.egg-info/PKG-INFO
--rw-rw----   0 eriq      (1000) eriq      (1000)      250 2024-01-02 13:58:35.000000 ucsc-cse40-0.9.0/ucsc_cse40.egg-info/SOURCES.txt
--rw-rw----   0 eriq      (1000) eriq      (1000)        1 2024-01-02 13:58:35.000000 ucsc-cse40-0.9.0/ucsc_cse40.egg-info/dependency_links.txt
--rw-rw----   0 eriq      (1000) eriq      (1000)      105 2024-01-02 13:58:35.000000 ucsc-cse40-0.9.0/ucsc_cse40.egg-info/requires.txt
--rw-rw----   0 eriq      (1000) eriq      (1000)        6 2024-01-02 13:58:35.000000 ucsc-cse40-0.9.0/ucsc_cse40.egg-info/top_level.txt
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-01 20:07:11.304915 ucsc-cse40-0.9.1/
+-rw-r--r--   0 eriq      (1000) eriq      (1000)     1590 2024-04-01 20:07:11.304915 ucsc-cse40-0.9.1/PKG-INFO
+-rw-rw----   0 eriq      (1000) eriq      (1000)      851 2024-01-02 12:58:26.000000 ucsc-cse40-0.9.1/README.md
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-01 20:07:11.304915 ucsc-cse40-0.9.1/cse40/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2023-05-17 17:36:49.000000 ucsc-cse40-0.9.1/cse40/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)       38 2024-04-01 20:07:11.304915 ucsc-cse40-0.9.1/setup.cfg
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1362 2024-04-01 20:06:11.000000 ucsc-cse40-0.9.1/setup.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-01 20:07:11.304915 ucsc-cse40-0.9.1/ucsc_cse40.egg-info/
+-rw-r--r--   0 eriq      (1000) eriq      (1000)     1590 2024-04-01 20:07:11.000000 ucsc-cse40-0.9.1/ucsc_cse40.egg-info/PKG-INFO
+-rw-rw----   0 eriq      (1000) eriq      (1000)      250 2024-04-01 20:07:11.000000 ucsc-cse40-0.9.1/ucsc_cse40.egg-info/SOURCES.txt
+-rw-rw----   0 eriq      (1000) eriq      (1000)        1 2024-04-01 20:07:11.000000 ucsc-cse40-0.9.1/ucsc_cse40.egg-info/dependency_links.txt
+-rw-rw----   0 eriq      (1000) eriq      (1000)      105 2024-04-01 20:07:11.000000 ucsc-cse40-0.9.1/ucsc_cse40.egg-info/requires.txt
+-rw-rw----   0 eriq      (1000) eriq      (1000)        6 2024-04-01 20:07:11.000000 ucsc-cse40-0.9.1/ucsc_cse40.egg-info/top_level.txt
```

### Comparing `ucsc-cse40-0.9.0/PKG-INFO` & `ucsc-cse40-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucsc-cse40
-Version: 0.9.0
+Version: 0.9.1
 Summary: Dependencies for UCSC's CSE 40 - ML Basics: Data Analysis and Empirical Methods
 Home-page: https://github.com/ucsc-cse-40/ucsc-cse40
 Maintainer: Eriq Augustine
 Maintainer-email: eaugusti@ucsc.edu
 Keywords: grading
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: /home/eriq/code/cse40/ucsc-cse40/LICENSE.txt
 Requires-Dist: jupyterlab>=3.5.0
 Requires-Dist: matplotlib>=3.6.2
 Requires-Dist: numpy>=1.22.3
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: scikit-learn>=1.2.0
-Requires-Dist: autograder-py==0.4.*
+Requires-Dist: autograder-py>=0.4.2
 
 # UCSC CSE 40
 
 Materials for UCSC's CSE 40 course taught by Dr. Lise Getoor and managed by the [LINQS lab](https://linqs.org/).
 This package is available on PyPi at [ucsc-cse40](https://pypi.org/project/ucsc-cse40/).
 
 ## Dependencies
```

### Comparing `ucsc-cse40-0.9.0/README.md` & `ucsc-cse40-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ucsc-cse40-0.9.0/setup.py` & `ucsc-cse40-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with open(LONG_DESCRIPTION_PATH, 'r') as file:
         return file.read()
 
 setuptools.setup(
     name = 'ucsc-cse40',
     url = 'https://github.com/ucsc-cse-40/ucsc-cse40',
 
-    version = '0.9.0',
+    version = '0.9.1',
     keywords = 'grading',
 
     description = "Dependencies for UCSC's CSE 40 - ML Basics: Data Analysis and Empirical Methods",
     long_description = get_description(),
     long_description_content_type = 'text/markdown',
 
 
@@ -37,14 +37,14 @@
 
     install_requires = [
         'jupyterlab>=3.5.0',
         'matplotlib>=3.6.2',
         'numpy>=1.22.3',
         'pandas>=1.5.1',
         'scikit-learn>=1.2.0',
-        'autograder-py==0.4.*',
+        'autograder-py>=0.4.2',
     ],
 
     license_files = (LICENSE_PATH, ),
 
     python_requires = '>=3.8'
 )
```

### Comparing `ucsc-cse40-0.9.0/ucsc_cse40.egg-info/PKG-INFO` & `ucsc-cse40-0.9.1/ucsc_cse40.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucsc-cse40
-Version: 0.9.0
+Version: 0.9.1
 Summary: Dependencies for UCSC's CSE 40 - ML Basics: Data Analysis and Empirical Methods
 Home-page: https://github.com/ucsc-cse-40/ucsc-cse40
 Maintainer: Eriq Augustine
 Maintainer-email: eaugusti@ucsc.edu
 Keywords: grading
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: /home/eriq/code/cse40/ucsc-cse40/LICENSE.txt
 Requires-Dist: jupyterlab>=3.5.0
 Requires-Dist: matplotlib>=3.6.2
 Requires-Dist: numpy>=1.22.3
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: scikit-learn>=1.2.0
-Requires-Dist: autograder-py==0.4.*
+Requires-Dist: autograder-py>=0.4.2
 
 # UCSC CSE 40
 
 Materials for UCSC's CSE 40 course taught by Dr. Lise Getoor and managed by the [LINQS lab](https://linqs.org/).
 This package is available on PyPi at [ucsc-cse40](https://pypi.org/project/ucsc-cse40/).
 
 ## Dependencies
```

