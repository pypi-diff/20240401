# Comparing `tmp/openbb_ecb-1.1.3.tar.gz` & `tmp/openbb_ecb-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_ecb-1.1.3.tar", max compression
+gzip compressed data, was "openbb_ecb-1.1.4.tar", max compression
```

## Comparing `openbb_ecb-1.1.3.tar` & `openbb_ecb-1.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      426 2024-01-17 14:26:16.668136 openbb_ecb-1.1.3/README.md
--rw-r--r--   0        0        0      895 2024-01-17 14:26:16.668305 openbb_ecb-1.1.3/openbb_ecb/__init__.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.668379 openbb_ecb-1.1.3/openbb_ecb/models/__init__.py
--rw-r--r--   0        0        0     3305 2024-01-17 14:26:16.668459 openbb_ecb-1.1.3/openbb_ecb/models/balance_of_payments.py
--rw-r--r--   0        0        0     2263 2024-01-17 14:26:16.668528 openbb_ecb-1.1.3/openbb_ecb/models/currency_reference_rates.py
--rw-r--r--   0        0        0     4199 2024-02-23 17:14:57.424185 openbb_ecb-1.1.3/openbb_ecb/models/eu_yield_curve.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.668703 openbb_ecb-1.1.3/openbb_ecb/utils/__init__.py
--rw-r--r--   0        0        0    16135 2024-01-17 14:26:16.668885 openbb_ecb-1.1.3/openbb_ecb/utils/bps_series.py
--rw-r--r--   0        0        0     1374 2024-01-17 14:26:16.668966 openbb_ecb-1.1.3/openbb_ecb/utils/ecb_helpers.py
--rw-r--r--   0        0        0     4867 2024-02-23 17:14:57.424259 openbb_ecb-1.1.3/openbb_ecb/utils/yield_curve_series.py
--rw-r--r--   0        0        0      455 2024-03-11 20:00:29.187602 openbb_ecb-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 openbb_ecb-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      426 2024-02-29 11:03:36.766673 openbb_ecb-1.1.4/README.md
+-rw-r--r--   0        0        0      895 2024-03-21 17:38:35.638562 openbb_ecb-1.1.4/openbb_ecb/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.766855 openbb_ecb-1.1.4/openbb_ecb/models/__init__.py
+-rw-r--r--   0        0        0     3305 2024-03-21 17:38:35.638719 openbb_ecb-1.1.4/openbb_ecb/models/balance_of_payments.py
+-rw-r--r--   0        0        0     2263 2024-02-29 11:03:36.767005 openbb_ecb-1.1.4/openbb_ecb/models/currency_reference_rates.py
+-rw-r--r--   0        0        0     4199 2024-03-21 17:38:35.638863 openbb_ecb-1.1.4/openbb_ecb/models/eu_yield_curve.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.767115 openbb_ecb-1.1.4/openbb_ecb/utils/__init__.py
+-rw-r--r--   0        0        0    16135 2024-02-29 11:03:36.767215 openbb_ecb-1.1.4/openbb_ecb/utils/bps_series.py
+-rw-r--r--   0        0        0     1374 2024-02-29 11:03:36.767284 openbb_ecb-1.1.4/openbb_ecb/utils/ecb_helpers.py
+-rw-r--r--   0        0        0     4867 2024-03-13 16:36:51.648056 openbb_ecb-1.1.4/openbb_ecb/utils/yield_curve_series.py
+-rw-r--r--   0        0        0      455 2024-04-01 14:21:31.087177 openbb_ecb-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 openbb_ecb-1.1.4/PKG-INFO
```

### Comparing `openbb_ecb-1.1.3/openbb_ecb/__init__.py` & `openbb_ecb-1.1.4/openbb_ecb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_ecb-1.1.3/openbb_ecb/models/balance_of_payments.py` & `openbb_ecb-1.1.4/openbb_ecb/models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_ecb-1.1.3/openbb_ecb/models/currency_reference_rates.py` & `openbb_ecb-1.1.4/openbb_ecb/models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_ecb-1.1.3/openbb_ecb/models/eu_yield_curve.py` & `openbb_ecb-1.1.4/openbb_ecb/models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_ecb-1.1.3/openbb_ecb/utils/bps_series.py` & `openbb_ecb-1.1.4/openbb_ecb/utils/bps_series.py`

 * *Files identical despite different names*

### Comparing `openbb_ecb-1.1.3/openbb_ecb/utils/ecb_helpers.py` & `openbb_ecb-1.1.4/openbb_ecb/utils/ecb_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_ecb-1.1.3/openbb_ecb/utils/yield_curve_series.py` & `openbb_ecb-1.1.4/openbb_ecb/utils/yield_curve_series.py`

 * *Files identical despite different names*

### Comparing `openbb_ecb-1.1.3/PKG-INFO` & `openbb_ecb-1.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-ecb
-Version: 1.1.3
+Version: 1.1.4
 Summary: ECB extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: openbb-core (>=1.1.3,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
 # OpenBB ECB Provider
 
 This extension integrates the [ECB](https://data.ecb.europa.eu/) data provider into the OpenBB Platform.
```

