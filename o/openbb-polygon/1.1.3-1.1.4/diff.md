# Comparing `tmp/openbb_polygon-1.1.3.tar.gz` & `tmp/openbb_polygon-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_polygon-1.1.3.tar", max compression
+gzip compressed data, was "openbb_polygon-1.1.4.tar", max compression
```

## Comparing `openbb_polygon-1.1.3.tar` & `openbb_polygon-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      430 2024-01-17 14:26:16.781125 openbb_polygon-1.1.3/README.md
--rw-r--r--   0        0        0     2100 2024-03-11 10:41:33.412394 openbb_polygon-1.1.3/openbb_polygon/__init__.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.781318 openbb_polygon-1.1.3/openbb_polygon/models/__init__.py
--rw-r--r--   0        0        0     9313 2024-01-17 14:26:16.781421 openbb_polygon-1.1.3/openbb_polygon/models/balance_sheet.py
--rw-r--r--   0        0        0     6961 2024-01-17 14:26:16.781486 openbb_polygon-1.1.3/openbb_polygon/models/cash_flow.py
--rw-r--r--   0        0        0     4600 2024-02-26 09:52:50.865351 openbb_polygon-1.1.3/openbb_polygon/models/company_news.py
--rw-r--r--   0        0        0     6130 2024-03-11 10:41:33.412584 openbb_polygon-1.1.3/openbb_polygon/models/crypto_historical.py
--rw-r--r--   0        0        0     6054 2024-03-11 10:41:33.412739 openbb_polygon-1.1.3/openbb_polygon/models/currency_historical.py
--rw-r--r--   0        0        0     6125 2024-03-11 10:41:33.413054 openbb_polygon-1.1.3/openbb_polygon/models/currency_pairs.py
--rw-r--r--   0        0        0     7020 2024-03-11 10:41:33.413185 openbb_polygon-1.1.3/openbb_polygon/models/equity_historical.py
--rw-r--r--   0        0        0     8211 2024-02-28 09:43:45.471820 openbb_polygon-1.1.3/openbb_polygon/models/equity_nbbo.py
--rw-r--r--   0        0        0    13663 2024-02-06 11:54:53.240184 openbb_polygon-1.1.3/openbb_polygon/models/income_statement.py
--rw-r--r--   0        0        0     5973 2024-03-11 10:41:33.413316 openbb_polygon-1.1.3/openbb_polygon/models/index_historical.py
--rw-r--r--   0        0        0     3618 2024-01-29 13:09:03.823442 openbb_polygon-1.1.3/openbb_polygon/models/market_indices.py
--rw-r--r--   0        0        0     6126 2024-02-06 11:54:53.240441 openbb_polygon-1.1.3/openbb_polygon/models/market_snapshots.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.782434 openbb_polygon-1.1.3/openbb_polygon/py.typed
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.782500 openbb_polygon-1.1.3/openbb_polygon/utils/__init__.py
--rw-r--r--   0        0        0     3690 2024-02-28 12:51:01.931137 openbb_polygon-1.1.3/openbb_polygon/utils/helpers.py
--rw-r--r--   0        0        0      457 2024-03-11 19:59:03.404412 openbb_polygon-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 openbb_polygon-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      430 2024-02-29 11:03:36.885809 openbb_polygon-1.1.4/README.md
+-rw-r--r--   0        0        0     2100 2024-03-21 17:38:35.652390 openbb_polygon-1.1.4/openbb_polygon/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.885969 openbb_polygon-1.1.4/openbb_polygon/models/__init__.py
+-rw-r--r--   0        0        0     9313 2024-03-21 17:38:35.652575 openbb_polygon-1.1.4/openbb_polygon/models/balance_sheet.py
+-rw-r--r--   0        0        0     6961 2024-03-21 17:38:35.652696 openbb_polygon-1.1.4/openbb_polygon/models/cash_flow.py
+-rw-r--r--   0        0        0     4600 2024-03-13 16:36:51.767779 openbb_polygon-1.1.4/openbb_polygon/models/company_news.py
+-rw-r--r--   0        0        0     6130 2024-03-13 16:36:51.767909 openbb_polygon-1.1.4/openbb_polygon/models/crypto_historical.py
+-rw-r--r--   0        0        0     6054 2024-03-13 16:36:51.768003 openbb_polygon-1.1.4/openbb_polygon/models/currency_historical.py
+-rw-r--r--   0        0        0     6125 2024-03-21 17:38:35.652826 openbb_polygon-1.1.4/openbb_polygon/models/currency_pairs.py
+-rw-r--r--   0        0        0     7020 2024-03-13 16:36:51.768639 openbb_polygon-1.1.4/openbb_polygon/models/equity_historical.py
+-rw-r--r--   0        0        0     8240 2024-03-21 17:38:35.652992 openbb_polygon-1.1.4/openbb_polygon/models/equity_nbbo.py
+-rw-r--r--   0        0        0    13663 2024-03-21 17:38:35.653155 openbb_polygon-1.1.4/openbb_polygon/models/income_statement.py
+-rw-r--r--   0        0        0     5973 2024-03-13 16:36:51.768957 openbb_polygon-1.1.4/openbb_polygon/models/index_historical.py
+-rw-r--r--   0        0        0     3618 2024-03-21 17:38:35.653278 openbb_polygon-1.1.4/openbb_polygon/models/market_indices.py
+-rw-r--r--   0        0        0     6126 2024-03-21 17:38:35.653455 openbb_polygon-1.1.4/openbb_polygon/models/market_snapshots.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.887235 openbb_polygon-1.1.4/openbb_polygon/py.typed
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.887288 openbb_polygon-1.1.4/openbb_polygon/utils/__init__.py
+-rw-r--r--   0        0        0     3690 2024-03-13 16:36:51.769344 openbb_polygon-1.1.4/openbb_polygon/utils/helpers.py
+-rw-r--r--   0        0        0      457 2024-04-01 14:20:16.520095 openbb_polygon-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 openbb_polygon-1.1.4/PKG-INFO
```

### Comparing `openbb_polygon-1.1.3/openbb_polygon/__init__.py` & `openbb_polygon-1.1.4/openbb_polygon/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.3/openbb_polygon/models/balance_sheet.py` & `openbb_polygon-1.1.4/openbb_polygon/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.3/openbb_polygon/models/cash_flow.py` & `openbb_polygon-1.1.4/openbb_polygon/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.3/openbb_polygon/models/company_news.py` & `openbb_polygon-1.1.4/openbb_polygon/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.3/openbb_polygon/models/crypto_historical.py` & `openbb_polygon-1.1.4/openbb_polygon/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.3/openbb_polygon/models/currency_historical.py` & `openbb_polygon-1.1.4/openbb_polygon/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.3/openbb_polygon/models/currency_pairs.py` & `openbb_polygon-1.1.4/openbb_polygon/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.3/openbb_polygon/models/equity_historical.py` & `openbb_polygon-1.1.4/openbb_polygon/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.3/openbb_polygon/models/equity_nbbo.py` & `openbb_polygon-1.1.4/openbb_polygon/models/equity_nbbo.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,41 +41,41 @@
             QUERY_DESCRIPTIONS.get("date", "")
             + " Use bracketed the timestamp parameters to specify exact time ranges."
         ),
         alias="timestamp",
     )
     timestamp_lt: Optional[Union[datetime, str]] = Field(
         default=None,
-        description="""
-            Query by datetime, less than. Either a date with the format YYYY-MM-DD or a TZ-aware timestamp string,
-            YYYY-MM-DDTH:M:S.000000000-04:00". Include all nanoseconds and the 'T' between the day and hour.
-        """,
+        description=(
+            "Query by datetime, less than. Either a date with the format 'YYYY-MM-DD' or a TZ-aware timestamp string, "
+            "'YYYY-MM-DDTH:M:S.000000000-04:00'. Include all nanoseconds and the 'T' between the day and hour."
+        ),
     )
     timestamp_gt: Optional[Union[datetime, str]] = Field(
         default=None,
-        description="""
-            Query by datetime, greater than. Either a date with the format YYYY-MM-DD or a TZ-aware timestamp string,
-            YYYY-MM-DDTH:M:S.000000000-04:00". Include all nanoseconds and the 'T' between the day and hour.
-        """,
+        description=(
+            "Query by datetime, greater than. Either a date with the format 'YYYY-MM-DD' or a TZ-aware timestamp string, "
+            "'YYYY-MM-DDTH:M:S.000000000-04:00'. Include all nanoseconds and the 'T' between the day and hour."
+        ),
     )
     timestamp_lte: Optional[Union[datetime, str]] = Field(
         default=None,
-        description="""
-            Query by datetime, less than or equal to.
-            Either a date with the format YYYY-MM-DD or a TZ-aware timestamp string,
-            YYYY-MM-DDTH:M:S.000000000-04:00". Include all nanoseconds and the 'T' between the day and hour.
-        """,
+        description=(
+            "Query by datetime, less than or equal to. Either a date with the format 'YYYY-MM-DD' or a TZ-aware "
+            "timestamp string, 'YYYY-MM-DDTH:M:S.000000000-04:00'. Include all nanoseconds and the 'T' between the "
+            "day and hour."
+        ),
     )
     timestamp_gte: Optional[Union[datetime, str]] = Field(
         default=None,
-        description="""
-            Query by datetime, greater than or equal to.
-            Either a date with the format YYYY-MM-DD or a TZ-aware timestamp string,
-            YYYY-MM-DDTH:M:S.000000000-04:00". Include all nanoseconds and the 'T' between the day and hour.
-        """,
+        description=(
+            "Query by datetime, greater than or equal to. Either a date with the format 'YYYY-MM-DD' or a TZ-aware "
+            "timestamp string, 'YYYY-MM-DDTH:M:S.000000000-04:00'. Include all nanoseconds and the 'T' between the "
+            "day and hour."
+        ),
     )
 
     @field_validator("limit", mode="before", check_fields=False)
     @classmethod
     def capping_limit(cls, v):
         """Caps the number of records to 10 million."""
         return 10000000 if v > 10000000 else v
@@ -93,41 +93,41 @@
         default=None, description="A list of condition codes.", alias="conditions"
     )
     indicators: Optional[List[int]] = Field(
         default=None, description="A list of indicator codes.", alias="indicators"
     )
     sequence_num: Optional[int] = Field(
         default=None,
-        description="""
-            The sequence number represents the sequence in which message events happened.
-            These are increasing and unique per ticker symbol, but will not always be sequential
-            (e.g., 1, 2, 6, 9, 10, 11)
-        """,
+        description=(
+            "The sequence number represents the sequence in which message events happened. "
+            "These are increasing and unique per ticker symbol, but will not always be sequential "
+            "(e.g., 1, 2, 6, 9, 10, 11)"
+        ),
         alias="sequence_number",
     )
     participant_timestamp: Optional[datetime] = Field(
         default=None,
-        description="""
-            The nanosecond accuracy Participant/Exchange Unix Timestamp.
-            This is the timestamp of when the quote was actually generated at the exchange.
-        """,
+        description=(
+            "The nanosecond accuracy Participant/Exchange Unix Timestamp. "
+            "This is the timestamp of when the quote was actually generated at the exchange."
+        ),
     )
     sip_timestamp: Optional[datetime] = Field(
         default=None,
-        description="""
-            The nanosecond accuracy SIP Unix Timestamp.
-            This is the timestamp of when the SIP received this quote from the exchange which produced it.
-        """,
+        description=(
+            "The nanosecond accuracy SIP Unix Timestamp. "
+            "This is the timestamp of when the SIP received this quote from the exchange which produced it."
+        ),
     )
     trf_timestamp: Optional[datetime] = Field(
         default=None,
-        description="""
-            The nanosecond accuracy TRF (Trade Reporting Facility) Unix Timestamp.
-            This is the timestamp of when the trade reporting facility received this quote.
-        """,
+        description=(
+            "The nanosecond accuracy TRF (Trade Reporting Facility) Unix Timestamp. "
+            "This is the timestamp of when the trade reporting facility received this quote."
+        ),
     )
 
     @field_validator(
         "sip_timestamp",
         "participant_timestamp",
         "trf_timestamp",
         mode="before",
```

### Comparing `openbb_polygon-1.1.3/openbb_polygon/models/income_statement.py` & `openbb_polygon-1.1.4/openbb_polygon/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.3/openbb_polygon/models/index_historical.py` & `openbb_polygon-1.1.4/openbb_polygon/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.3/openbb_polygon/models/market_indices.py` & `openbb_polygon-1.1.4/openbb_polygon/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.3/openbb_polygon/models/market_snapshots.py` & `openbb_polygon-1.1.4/openbb_polygon/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.3/openbb_polygon/utils/helpers.py` & `openbb_polygon-1.1.4/openbb_polygon/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.3/PKG-INFO` & `openbb_polygon-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-polygon
-Version: 1.1.3
+Version: 1.1.4
 Summary: Polygon extension for OpenBB
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
 Description-Content-Type: text/markdown
 
 # OpenBB Polygon Provider
 
 This extension integrates the [Polygon](https://polygon.io/) data provider into the OpenBB Platform.
 
 ## Installation
```

