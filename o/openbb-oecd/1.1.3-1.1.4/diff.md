# Comparing `tmp/openbb_oecd-1.1.3.tar.gz` & `tmp/openbb_oecd-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_oecd-1.1.3.tar", max compression
+gzip compressed data, was "openbb_oecd-1.1.4.tar", max compression
```

## Comparing `openbb_oecd-1.1.3.tar` & `openbb_oecd-1.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.779799 openbb_oecd-1.1.3/README.md
--rw-r--r--   0        0        0      981 2024-01-31 18:17:26.678755 openbb_oecd-1.1.3/openbb_oecd/__init__.py
--rw-r--r--   0        0        0     4658 2024-03-11 10:41:33.409289 openbb_oecd-1.1.3/openbb_oecd/models/composite_leading_indicator.py
--rw-r--r--   0        0        0     4292 2024-03-11 10:41:33.409404 openbb_oecd-1.1.3/openbb_oecd/models/gdp_forecast.py
--rw-r--r--   0        0        0     3725 2024-03-11 10:41:33.409499 openbb_oecd-1.1.3/openbb_oecd/models/gdp_nominal.py
--rw-r--r--   0        0        0     3920 2024-03-11 10:41:33.409591 openbb_oecd-1.1.3/openbb_oecd/models/gdp_real.py
--rw-r--r--   0        0        0     4952 2024-03-11 10:41:33.409829 openbb_oecd-1.1.3/openbb_oecd/models/long_term_interest_rate.py
--rw-r--r--   0        0        0     4960 2024-03-11 10:41:33.409959 openbb_oecd-1.1.3/openbb_oecd/models/short_term_interest_rate.py
--rw-r--r--   0        0        0     6141 2024-03-11 10:41:33.410092 openbb_oecd-1.1.3/openbb_oecd/models/unemployment.py
--rw-r--r--   0        0        0    13133 2024-02-29 17:24:47.120298 openbb_oecd-1.1.3/openbb_oecd/utils/constants.py
--rw-r--r--   0        0        0     8668 2024-03-11 10:41:33.410204 openbb_oecd-1.1.3/openbb_oecd/utils/helpers.py
--rw-r--r--   0        0        0      485 2024-03-11 19:59:20.558096 openbb_oecd-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      635 1970-01-01 00:00:00.000000 openbb_oecd-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.884104 openbb_oecd-1.1.4/README.md
+-rw-r--r--   0        0        0      981 2024-03-21 17:38:35.652197 openbb_oecd-1.1.4/openbb_oecd/__init__.py
+-rw-r--r--   0        0        0     4658 2024-03-13 16:36:51.763328 openbb_oecd-1.1.4/openbb_oecd/models/composite_leading_indicator.py
+-rw-r--r--   0        0        0     4292 2024-03-13 16:36:51.763472 openbb_oecd-1.1.4/openbb_oecd/models/gdp_forecast.py
+-rw-r--r--   0        0        0     3725 2024-03-13 16:36:51.763745 openbb_oecd-1.1.4/openbb_oecd/models/gdp_nominal.py
+-rw-r--r--   0        0        0     3920 2024-03-13 16:36:51.763872 openbb_oecd-1.1.4/openbb_oecd/models/gdp_real.py
+-rw-r--r--   0        0        0     4952 2024-03-13 16:36:51.764186 openbb_oecd-1.1.4/openbb_oecd/models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     4960 2024-03-13 16:36:51.764245 openbb_oecd-1.1.4/openbb_oecd/models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     6141 2024-03-13 16:36:51.764318 openbb_oecd-1.1.4/openbb_oecd/models/unemployment.py
+-rw-r--r--   0        0        0    13133 2024-03-13 16:36:51.764590 openbb_oecd-1.1.4/openbb_oecd/utils/constants.py
+-rw-r--r--   0        0        0     8668 2024-03-13 16:36:51.764757 openbb_oecd-1.1.4/openbb_oecd/utils/helpers.py
+-rw-r--r--   0        0        0      485 2024-04-01 14:20:33.323389 openbb_oecd-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      635 1970-01-01 00:00:00.000000 openbb_oecd-1.1.4/PKG-INFO
```

### Comparing `openbb_oecd-1.1.3/openbb_oecd/__init__.py` & `openbb_oecd-1.1.4/openbb_oecd/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.3/openbb_oecd/models/composite_leading_indicator.py` & `openbb_oecd-1.1.4/openbb_oecd/models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.3/openbb_oecd/models/gdp_forecast.py` & `openbb_oecd-1.1.4/openbb_oecd/models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.3/openbb_oecd/models/gdp_nominal.py` & `openbb_oecd-1.1.4/openbb_oecd/models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.3/openbb_oecd/models/gdp_real.py` & `openbb_oecd-1.1.4/openbb_oecd/models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.3/openbb_oecd/models/long_term_interest_rate.py` & `openbb_oecd-1.1.4/openbb_oecd/models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.3/openbb_oecd/models/short_term_interest_rate.py` & `openbb_oecd-1.1.4/openbb_oecd/models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.3/openbb_oecd/models/unemployment.py` & `openbb_oecd-1.1.4/openbb_oecd/models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.3/openbb_oecd/utils/constants.py` & `openbb_oecd-1.1.4/openbb_oecd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.3/openbb_oecd/utils/helpers.py` & `openbb_oecd-1.1.4/openbb_oecd/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.1.3/PKG-INFO` & `openbb_oecd-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: openbb-oecd
-Version: 1.1.3
+Version: 1.1.4
 Summary: OECD extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: defusedxml (>=0.8.0rc2,<0.9.0)
-Requires-Dist: openbb-core (>=1.1.3,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
 Requires-Dist: urllib3 (>1.26.16)
 Description-Content-Type: text/markdown
```

