# Comparing `tmp/quasi_utils-0.1.8.tar.gz` & `tmp/quasi_utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quasi_utils-0.1.8.tar", last modified: Sat Jan 27 14:02:33 2024, max compression
+gzip compressed data, was "quasi_utils-0.1.9.tar", last modified: Sat Jan 27 14:17:33 2024, max compression
```

## Comparing `quasi_utils-0.1.8.tar` & `quasi_utils-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-01-27 14:02:33.162353 quasi_utils-0.1.8/
--rw-rw-rw-   0        0        0     1092 2023-08-11 19:08:23.000000 quasi_utils-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       16 2023-08-11 19:08:23.000000 quasi_utils-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1952 2024-01-27 14:02:33.162353 quasi_utils-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-08-11 19:08:23.000000 quasi_utils-0.1.8/README.md
--rw-rw-rw-   0        0        0      784 2024-01-27 14:02:23.000000 quasi_utils-0.1.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-01-27 14:02:33.159354 quasi_utils-0.1.8/quasi_utils/
--rw-rw-rw-   0        0        0      391 2024-01-27 14:01:37.000000 quasi_utils-0.1.8/quasi_utils/auth_utils.py
--rw-rw-rw-   0        0        0      858 2024-01-26 21:04:27.000000 quasi_utils-0.1.8/quasi_utils/aws_utils.py
--rw-rw-rw-   0        0        0      839 2024-01-26 21:04:27.000000 quasi_utils-0.1.8/quasi_utils/generic_utils.py
--rw-rw-rw-   0        0        0     8481 2024-01-26 23:42:03.000000 quasi_utils-0.1.8/quasi_utils/oms.py
--rw-rw-rw-   0        0        0     3236 2024-01-26 21:04:27.000000 quasi_utils-0.1.8/quasi_utils/oms_utils.py
-drwxrwxrwx   0        0        0        0 2024-01-27 14:02:33.162353 quasi_utils-0.1.8/quasi_utils.egg-info/
--rw-rw-rw-   0        0        0     1952 2024-01-27 14:02:33.000000 quasi_utils-0.1.8/quasi_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2024-01-27 14:02:33.000000 quasi_utils-0.1.8/quasi_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-27 14:02:33.000000 quasi_utils-0.1.8/quasi_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-01-27 14:02:33.000000 quasi_utils-0.1.8/quasi_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-01-27 14:02:33.000000 quasi_utils-0.1.8/quasi_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-27 14:02:33.162353 quasi_utils-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-08-11 19:08:23.000000 quasi_utils-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-27 14:17:33.486238 quasi_utils-0.1.9/
+-rw-rw-rw-   0        0        0     1092 2023-08-11 19:08:23.000000 quasi_utils-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-08-11 19:08:23.000000 quasi_utils-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1952 2024-01-27 14:17:33.485238 quasi_utils-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-08-11 19:08:23.000000 quasi_utils-0.1.9/README.md
+-rw-rw-rw-   0        0        0      784 2024-01-27 14:17:25.000000 quasi_utils-0.1.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-01-27 14:17:33.483239 quasi_utils-0.1.9/quasi_utils/
+-rw-rw-rw-   0        0        0      391 2024-01-27 14:17:24.000000 quasi_utils-0.1.9/quasi_utils/auth_utils.py
+-rw-rw-rw-   0        0        0      858 2024-01-26 21:04:27.000000 quasi_utils-0.1.9/quasi_utils/aws_utils.py
+-rw-rw-rw-   0        0        0      839 2024-01-26 21:04:27.000000 quasi_utils-0.1.9/quasi_utils/generic_utils.py
+-rw-rw-rw-   0        0        0     8481 2024-01-26 23:42:03.000000 quasi_utils-0.1.9/quasi_utils/oms.py
+-rw-rw-rw-   0        0        0     3236 2024-01-26 21:04:27.000000 quasi_utils-0.1.9/quasi_utils/oms_utils.py
+drwxrwxrwx   0        0        0        0 2024-01-27 14:17:33.485238 quasi_utils-0.1.9/quasi_utils.egg-info/
+-rw-rw-rw-   0        0        0     1952 2024-01-27 14:17:33.000000 quasi_utils-0.1.9/quasi_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2024-01-27 14:17:33.000000 quasi_utils-0.1.9/quasi_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-27 14:17:33.000000 quasi_utils-0.1.9/quasi_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-01-27 14:17:33.000000 quasi_utils-0.1.9/quasi_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-01-27 14:17:33.000000 quasi_utils-0.1.9/quasi_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-01-27 14:17:33.486238 quasi_utils-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-08-11 19:08:23.000000 quasi_utils-0.1.9/setup.py
```

### Comparing `quasi_utils-0.1.8/LICENSE` & `quasi_utils-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quasi_utils-0.1.8/PKG-INFO` & `quasi_utils-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quasi_utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: Utilities for OMS
 Author-email: Kaustubh Dixit <hi.stockemy@gmail.com>
 License: Copyright (c) 2022 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `quasi_utils-0.1.8/pyproject.toml` & `quasi_utils-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ['setuptools>=68.2.2', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'quasi_utils'
-version = '0.1.8'
+version = '0.1.9'
 description = 'Utilities for OMS'
 readme = 'README.md'
 authors = [{name = 'Kaustubh Dixit', email = 'hi.stockemy@gmail.com'}]
 license = {file = 'LICENSE'}
 classifiers = ['License :: OSI Approved :: MIT License', 'Programming Language :: Python',
                'Programming Language :: Python :: 3', ]
 keywords = ['trading', 'algorithm', 'nifty']
 dependencies = ['requests==2.31.0', 'pyjwt==2.8.0']
 requires-python = '>=3.10'
 
 [bumpver]
-current_version = '0.1.8'
+current_version = '0.1.9'
 version_pattern = 'MAJOR.MINOR.PATCH'
 
 [bumpver.file_patterns]
 'pyproject.toml' = ["version = '{version}'"]
 'deploy.py' = ["quasi-utils=={version}"]
```

### Comparing `quasi_utils-0.1.8/quasi_utils/aws_utils.py` & `quasi_utils-0.1.9/quasi_utils/aws_utils.py`

 * *Files identical despite different names*

### Comparing `quasi_utils-0.1.8/quasi_utils/generic_utils.py` & `quasi_utils-0.1.9/quasi_utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `quasi_utils-0.1.8/quasi_utils/oms.py` & `quasi_utils-0.1.9/quasi_utils/oms.py`

 * *Files identical despite different names*

### Comparing `quasi_utils-0.1.8/quasi_utils/oms_utils.py` & `quasi_utils-0.1.9/quasi_utils/oms_utils.py`

 * *Files identical despite different names*

### Comparing `quasi_utils-0.1.8/quasi_utils.egg-info/PKG-INFO` & `quasi_utils-0.1.9/quasi_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quasi_utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: Utilities for OMS
 Author-email: Kaustubh Dixit <hi.stockemy@gmail.com>
 License: Copyright (c) 2022 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

