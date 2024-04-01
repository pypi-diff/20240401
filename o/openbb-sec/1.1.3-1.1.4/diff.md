# Comparing `tmp/openbb_sec-1.1.3.tar.gz` & `tmp/openbb_sec-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_sec-1.1.3.tar", max compression
+gzip compressed data, was "openbb_sec-1.1.4.tar", max compression
```

## Comparing `openbb_sec-1.1.3.tar` & `openbb_sec-1.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      424 2024-01-17 14:26:16.793233 openbb_sec-1.1.3/README.md
--rw-r--r--   0        0        0     1562 2024-03-11 10:41:33.413904 openbb_sec-1.1.3/openbb_sec/__init__.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.793419 openbb_sec-1.1.3/openbb_sec/models/__init__.py
--rw-r--r--   0        0        0     1454 2024-02-26 21:17:23.742087 openbb_sec-1.1.3/openbb_sec/models/cik_map.py
--rw-r--r--   0        0        0     8257 2024-01-17 14:26:16.793580 openbb_sec-1.1.3/openbb_sec/models/company_filings.py
--rw-r--r--   0        0        0     2617 2024-01-17 14:26:16.793651 openbb_sec-1.1.3/openbb_sec/models/equity_ftd.py
--rw-r--r--   0        0        0     2720 2024-02-07 09:55:40.834170 openbb_sec-1.1.3/openbb_sec/models/equity_search.py
--rw-r--r--   0        0        0    32406 2024-02-29 11:47:32.351999 openbb_sec-1.1.3/openbb_sec/models/etf_holdings.py
--rw-r--r--   0        0        0     2754 2024-03-11 10:41:33.414172 openbb_sec-1.1.3/openbb_sec/models/form_13FHR.py
--rw-r--r--   0        0        0     2079 2024-02-06 11:54:53.241494 openbb_sec-1.1.3/openbb_sec/models/institutions_search.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.793873 openbb_sec-1.1.3/openbb_sec/models/py.typed
--rw-r--r--   0        0        0     2790 2024-01-17 14:26:16.793948 openbb_sec-1.1.3/openbb_sec/models/rss_litigation.py
--rw-r--r--   0        0        0     1945 2024-02-28 09:43:45.471929 openbb_sec-1.1.3/openbb_sec/models/schema_files.py
--rw-r--r--   0        0        0     3009 2024-02-06 11:54:53.241594 openbb_sec-1.1.3/openbb_sec/models/sic_search.py
--rw-r--r--   0        0        0     1714 2024-03-11 10:41:33.414306 openbb_sec-1.1.3/openbb_sec/models/symbol_map.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.794237 openbb_sec-1.1.3/openbb_sec/py.typed
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.794316 openbb_sec-1.1.3/openbb_sec/utils/__init__.py
--rw-r--r--   0        0        0     5511 2024-01-17 14:26:16.794406 openbb_sec-1.1.3/openbb_sec/utils/definitions.py
--rw-r--r--   0        0        0    13814 2024-01-17 14:26:16.794556 openbb_sec-1.1.3/openbb_sec/utils/helpers.py
--rw-r--r--   0        0        0     7410 2024-03-11 10:41:33.414416 openbb_sec-1.1.3/openbb_sec/utils/parse_13f.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.794597 openbb_sec-1.1.3/openbb_sec/utils/py.typed
--rw-r--r--   0        0        0      516 2024-03-11 19:58:44.392876 openbb_sec-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 openbb_sec-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      424 2024-02-29 11:03:36.896002 openbb_sec-1.1.4/README.md
+-rw-r--r--   0        0        0     1562 2024-03-21 17:38:35.653641 openbb_sec-1.1.4/openbb_sec/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.896154 openbb_sec-1.1.4/openbb_sec/models/__init__.py
+-rw-r--r--   0        0        0     1454 2024-03-21 17:38:35.653808 openbb_sec-1.1.4/openbb_sec/models/cik_map.py
+-rw-r--r--   0        0        0     8277 2024-03-21 17:38:35.653936 openbb_sec-1.1.4/openbb_sec/models/company_filings.py
+-rw-r--r--   0        0        0     2617 2024-03-21 17:38:35.654048 openbb_sec-1.1.4/openbb_sec/models/equity_ftd.py
+-rw-r--r--   0        0        0     2720 2024-03-21 17:38:35.654140 openbb_sec-1.1.4/openbb_sec/models/equity_search.py
+-rw-r--r--   0        0        0    32406 2024-03-21 17:38:35.654328 openbb_sec-1.1.4/openbb_sec/models/etf_holdings.py
+-rw-r--r--   0        0        0     2754 2024-03-21 17:38:35.654598 openbb_sec-1.1.4/openbb_sec/models/form_13FHR.py
+-rw-r--r--   0        0        0     2079 2024-03-21 17:38:35.654754 openbb_sec-1.1.4/openbb_sec/models/institutions_search.py
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.779245 openbb_sec-1.1.4/openbb_sec/models/py.typed
+-rw-r--r--   0        0        0     2790 2024-03-21 17:38:35.654871 openbb_sec-1.1.4/openbb_sec/models/rss_litigation.py
+-rw-r--r--   0        0        0     1945 2024-03-21 17:38:35.655006 openbb_sec-1.1.4/openbb_sec/models/schema_files.py
+-rw-r--r--   0        0        0     3009 2024-03-21 17:38:35.655140 openbb_sec-1.1.4/openbb_sec/models/sic_search.py
+-rw-r--r--   0        0        0     1714 2024-03-21 17:38:35.655251 openbb_sec-1.1.4/openbb_sec/models/symbol_map.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.896831 openbb_sec-1.1.4/openbb_sec/py.typed
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.896870 openbb_sec-1.1.4/openbb_sec/utils/__init__.py
+-rw-r--r--   0        0        0     5511 2024-02-29 11:03:36.896953 openbb_sec-1.1.4/openbb_sec/utils/definitions.py
+-rw-r--r--   0        0        0    13834 2024-03-21 17:38:35.655553 openbb_sec-1.1.4/openbb_sec/utils/helpers.py
+-rw-r--r--   0        0        0     7410 2024-03-21 17:38:35.655723 openbb_sec-1.1.4/openbb_sec/utils/parse_13f.py
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.780521 openbb_sec-1.1.4/openbb_sec/utils/py.typed
+-rw-r--r--   0        0        0      516 2024-04-01 14:20:00.173560 openbb_sec-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 openbb_sec-1.1.4/PKG-INFO
```

### Comparing `openbb_sec-1.1.3/openbb_sec/__init__.py` & `openbb_sec-1.1.4/openbb_sec/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.3/openbb_sec/models/cik_map.py` & `openbb_sec-1.1.4/openbb_sec/models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.3/openbb_sec/models/company_filings.py` & `openbb_sec-1.1.4/openbb_sec/models/company_filings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """SEC Company Filings Model."""
 
+# pylint: skip-file
 from datetime import (
     date as dateType,
     datetime,
 )
 from typing import Any, Dict, List, Optional, Union
 
 import pandas as pd
```

### Comparing `openbb_sec-1.1.3/openbb_sec/models/equity_ftd.py` & `openbb_sec-1.1.4/openbb_sec/models/equity_ftd.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.3/openbb_sec/models/equity_search.py` & `openbb_sec-1.1.4/openbb_sec/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.3/openbb_sec/models/etf_holdings.py` & `openbb_sec-1.1.4/openbb_sec/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.3/openbb_sec/models/form_13FHR.py` & `openbb_sec-1.1.4/openbb_sec/models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.3/openbb_sec/models/institutions_search.py` & `openbb_sec-1.1.4/openbb_sec/models/institutions_search.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.3/openbb_sec/models/rss_litigation.py` & `openbb_sec-1.1.4/openbb_sec/models/rss_litigation.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.3/openbb_sec/models/schema_files.py` & `openbb_sec-1.1.4/openbb_sec/models/schema_files.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.3/openbb_sec/models/sic_search.py` & `openbb_sec-1.1.4/openbb_sec/models/sic_search.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.3/openbb_sec/models/symbol_map.py` & `openbb_sec-1.1.4/openbb_sec/models/symbol_map.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.3/openbb_sec/utils/definitions.py` & `openbb_sec-1.1.4/openbb_sec/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.3/openbb_sec/utils/helpers.py` & `openbb_sec-1.1.4/openbb_sec/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """SEC Helpers module"""
 
+# pylint: skip-file
 from datetime import timedelta
 from io import BytesIO
 from typing import Dict, List, Optional
 from zipfile import ZipFile
 
 import pandas as pd
 import requests
```

### Comparing `openbb_sec-1.1.3/openbb_sec/utils/parse_13f.py` & `openbb_sec-1.1.4/openbb_sec/utils/parse_13f.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.3/pyproject.toml` & `openbb_sec-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "openbb-sec"
-version = "1.1.3"
+version = "1.1.4"
 description = "SEC extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 readme = "README.md"
 packages = [{ include = "openbb_sec" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-openbb-core = "^1.1.3"
+openbb-core = "^1.1.5"
 requests-cache = "^1.1.0"
 xmltodict = "^0.13.0"
 pytest-freezegun = "^0.4.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openbb_sec-1.1.3/PKG-INFO` & `openbb_sec-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: openbb-sec
-Version: 1.1.3
+Version: 1.1.4
 Summary: SEC extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openbb-core (>=1.1.3,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
 Requires-Dist: pytest-freezegun (>=0.4.2,<0.5.0)
 Requires-Dist: requests-cache (>=1.1.0,<2.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
 # OpenBB SEC Provider
```

