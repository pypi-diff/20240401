# Comparing `tmp/i38e_utils-1.0.8.tar.gz` & `tmp/i38e_utils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i38e_utils-1.0.8.tar", max compression
+gzip compressed data, was "i38e_utils-1.0.9.tar", max compression
```

## Comparing `i38e_utils-1.0.8.tar` & `i38e_utils-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     3793 2024-03-08 17:42:55.199817 i38e_utils-1.0.8/README.md
--rw-r--r--   0        0        0      237 2024-03-11 18:06:02.323568 i38e_utils-1.0.8/i38e_utils/__init__.py
--rw-r--r--   0        0        0     6614 2024-03-11 17:38:47.290816 i38e_utils-1.0.8/i38e_utils/data_utils.py
--rw-r--r--   0        0        0    12707 2024-03-11 17:23:30.142823 i38e_utils-1.0.8/i38e_utils/date_utils.py
--rw-r--r--   0        0        0      235 2024-02-19 23:46:02.919156 i38e_utils-1.0.8/i38e_utils/df_helper/__init__.py
--rw-r--r--   0        0        0     9849 2024-03-08 16:59:27.384887 i38e_utils-1.0.8/i38e_utils/df_helper/_df_helper.py
--rw-r--r--   0        0        0     4118 2023-08-21 15:34:49.196226 i38e_utils-1.0.8/i38e_utils/df_helper/config.py
--rw-r--r--   0        0        0     5694 2023-11-06 21:12:09.421959 i38e_utils-1.0.8/i38e_utils/df_helper/io.py
--rw-r--r--   0        0        0    13411 2024-03-08 16:59:27.389781 i38e_utils-1.0.8/i38e_utils/df_helper/models.py
--rw-r--r--   0        0        0    14516 2024-02-01 17:13:09.300444 i38e_utils-1.0.8/i38e_utils/df_helper/sql_model_builder.py
--rw-r--r--   0        0        0     3736 2023-06-29 20:51:04.729632 i38e_utils-1.0.8/i38e_utils/df_helper/utils.py
--rw-r--r--   0        0        0     2888 2023-12-19 19:22:59.605330 i38e_utils-1.0.8/i38e_utils/df_utils.py
--rw-r--r--   0        0        0    10278 2024-02-27 17:42:29.083237 i38e_utils-1.0.8/i38e_utils/file_utils.py
--rw-r--r--   0        0        0        0 2023-12-19 18:33:11.737196 i38e_utils-1.0.8/i38e_utils/geopy_helper/__init__.py
--rw-r--r--   0        0        0     1636 2023-12-19 19:33:24.386926 i38e_utils-1.0.8/i38e_utils/log_utils.py
--rw-r--r--   0        0        0        0 2023-12-19 18:32:47.826452 i38e_utils-1.0.8/i38e_utils/osmnx_helper/__init__.py
--rw-r--r--   0        0        0      499 2024-03-11 18:06:36.226559 i38e_utils-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     4404 1970-01-01 00:00:00.000000 i38e_utils-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3793 2024-03-08 17:42:55.199817 i38e_utils-1.0.9/README.md
+-rw-r--r--   0        0        0      340 2024-03-11 18:21:56.103990 i38e_utils-1.0.9/i38e_utils/__init__.py
+-rw-r--r--   0        0        0     6614 2024-03-11 17:38:47.290816 i38e_utils-1.0.9/i38e_utils/data_utils.py
+-rw-r--r--   0        0        0    12707 2024-03-11 17:23:30.142823 i38e_utils-1.0.9/i38e_utils/date_utils.py
+-rw-r--r--   0        0        0      235 2024-02-19 23:46:02.919156 i38e_utils-1.0.9/i38e_utils/df_helper/__init__.py
+-rw-r--r--   0        0        0     9849 2024-03-08 16:59:27.384887 i38e_utils-1.0.9/i38e_utils/df_helper/_df_helper.py
+-rw-r--r--   0        0        0     4118 2023-08-21 15:34:49.196226 i38e_utils-1.0.9/i38e_utils/df_helper/config.py
+-rw-r--r--   0        0        0     5694 2023-11-06 21:12:09.421959 i38e_utils-1.0.9/i38e_utils/df_helper/io.py
+-rw-r--r--   0        0        0    13411 2024-03-08 16:59:27.389781 i38e_utils-1.0.9/i38e_utils/df_helper/models.py
+-rw-r--r--   0        0        0    14516 2024-02-01 17:13:09.300444 i38e_utils-1.0.9/i38e_utils/df_helper/sql_model_builder.py
+-rw-r--r--   0        0        0     3736 2023-06-29 20:51:04.729632 i38e_utils-1.0.9/i38e_utils/df_helper/utils.py
+-rw-r--r--   0        0        0     2888 2023-12-19 19:22:59.605330 i38e_utils-1.0.9/i38e_utils/df_utils.py
+-rw-r--r--   0        0        0    10278 2024-02-27 17:42:29.083237 i38e_utils-1.0.9/i38e_utils/file_utils.py
+-rw-r--r--   0        0        0        0 2023-12-19 18:33:11.737196 i38e_utils-1.0.9/i38e_utils/geopy_helper/__init__.py
+-rw-r--r--   0        0        0     1636 2023-12-19 19:33:24.386926 i38e_utils-1.0.9/i38e_utils/log_utils.py
+-rw-r--r--   0        0        0        0 2023-12-19 18:32:47.826452 i38e_utils-1.0.9/i38e_utils/osmnx_helper/__init__.py
+-rw-r--r--   0        0        0      516 2024-03-11 18:28:07.093868 i38e_utils-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4442 1970-01-01 00:00:00.000000 i38e_utils-1.0.9/PKG-INFO
```

### Comparing `i38e_utils-1.0.8/README.md` & `i38e_utils-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `i38e_utils-1.0.8/i38e_utils/data_utils.py` & `i38e_utils-1.0.9/i38e_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `i38e_utils-1.0.8/i38e_utils/date_utils.py` & `i38e_utils-1.0.9/i38e_utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `i38e_utils-1.0.8/i38e_utils/df_helper/_df_helper.py` & `i38e_utils-1.0.9/i38e_utils/df_helper/_df_helper.py`

 * *Files identical despite different names*

### Comparing `i38e_utils-1.0.8/i38e_utils/df_helper/config.py` & `i38e_utils-1.0.9/i38e_utils/df_helper/config.py`

 * *Files identical despite different names*

### Comparing `i38e_utils-1.0.8/i38e_utils/df_helper/io.py` & `i38e_utils-1.0.9/i38e_utils/df_helper/io.py`

 * *Files identical despite different names*

### Comparing `i38e_utils-1.0.8/i38e_utils/df_helper/models.py` & `i38e_utils-1.0.9/i38e_utils/df_helper/models.py`

 * *Files identical despite different names*

### Comparing `i38e_utils-1.0.8/i38e_utils/df_helper/sql_model_builder.py` & `i38e_utils-1.0.9/i38e_utils/df_helper/sql_model_builder.py`

 * *Files identical despite different names*

### Comparing `i38e_utils-1.0.8/i38e_utils/df_helper/utils.py` & `i38e_utils-1.0.9/i38e_utils/df_helper/utils.py`

 * *Files identical despite different names*

### Comparing `i38e_utils-1.0.8/i38e_utils/df_utils.py` & `i38e_utils-1.0.9/i38e_utils/df_utils.py`

 * *Files identical despite different names*

### Comparing `i38e_utils-1.0.8/i38e_utils/file_utils.py` & `i38e_utils-1.0.9/i38e_utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `i38e_utils-1.0.8/i38e_utils/log_utils.py` & `i38e_utils-1.0.9/i38e_utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `i38e_utils-1.0.8/PKG-INFO` & `i38e_utils-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: i38e-utils
-Version: 1.0.8
+Version: 1.0.9
 Summary: Various utilities for IBIS applications in data science and engineering
 Author: Luis Valverde
 Author-email: lvalverdeb@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dask (>=2024.2.1,<2025.0.0)
 Requires-Dist: django (==4.1.13)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 ## i38e-utils
 
 i38e-utils is a collection of utility functions and classes that I use in my projects. It is a work in progress and will be updated as I add more functionality.
 
 Currently, it includes the following:
```

