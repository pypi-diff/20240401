# Comparing `tmp/libre_linkup_py-0.2.1.tar.gz` & `tmp/libre_linkup_py-0.2.2.tar.gz`

## Comparing `libre_linkup_py-0.2.1.tar` & `libre_linkup_py-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/requirements-dev.lock
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/requirements.lock
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/.github/workflows/format.yml
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/.github/workflows/mypy.yml
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/examples/generate_interactive_glucose_graph.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/examples/generate_interactive_logbook_graph.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/examples/latest_glucose_reading.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/src/libre_link_up/__init__.py
--rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/src/libre_link_up/client.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/src/libre_link_up/types.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/tests/test_client.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/LICENSE
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/requirements-dev.lock
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/requirements.lock
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/.github/workflows/format.yml
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/.github/workflows/mypy.yml
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/examples/generate_interactive_glucose_graph.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/examples/generate_interactive_logbook_graph.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/examples/latest_glucose_reading.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/src/libre_link_up/__init__.py
+-rw-r--r--   0        0        0     8943 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/src/libre_link_up/client.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/src/libre_link_up/custom_types.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/tests/test_client.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/README.md
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 libre_linkup_py-0.2.2/PKG-INFO
```

### Comparing `libre_linkup_py-0.2.1/requirements-dev.lock` & `libre_linkup_py-0.2.2/requirements-dev.lock`

 * *Files 16% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 pydantic-core==2.16.3
     # via pydantic
 pytest==8.0.2
     # via pytest-dependency
 pytest-dependency==0.6.0
 python-dotenv==1.0.1
     # via libre-linkup-py
+pytz==2024.1
+    # via libre-linkup-py
 requests==2.31.0
     # via libre-linkup-py
 setuptools==69.1.1
     # via pytest-dependency
 tenacity==8.2.3
     # via plotly
 typing-extensions==4.10.0
```

### Comparing `libre_linkup_py-0.2.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `libre_linkup_py-0.2.2/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `libre_linkup_py-0.2.1/.github/ISSUE_TEMPLATE/feature_request.yml` & `libre_linkup_py-0.2.2/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `libre_linkup_py-0.2.1/examples/generate_interactive_glucose_graph.py` & `libre_linkup_py-0.2.2/examples/generate_interactive_glucose_graph.py`

 * *Files identical despite different names*

### Comparing `libre_linkup_py-0.2.1/examples/generate_interactive_logbook_graph.py` & `libre_linkup_py-0.2.2/examples/generate_interactive_logbook_graph.py`

 * *Files identical despite different names*

### Comparing `libre_linkup_py-0.2.1/examples/latest_glucose_reading.py` & `libre_linkup_py-0.2.2/examples/latest_glucose_reading.py`

 * *Files identical despite different names*

### Comparing `libre_linkup_py-0.2.1/src/libre_link_up/client.py` & `libre_linkup_py-0.2.2/src/libre_link_up/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 from datetime import datetime
 from typing import Any, Optional
-from libre_link_up.types import (
+from libre_link_up.custom_types import (
     GlucoseSensorReading,
     LibreLinkUpUrl,
     Connection,
     ReadingSource,
 )
 import requests
+from datetime import datetime
+from typing import Any, Optional
+from pytz import timezone
+import requests
 
 
-def _convert_timestamp_string_to_datetime(timestamp: str) -> float:
+def _convert_timestamp_string_to_datetime(
+    timestamp: str, country: Optional[str]
+) -> float:
+    print(timestamp)
     # "8/16/2023 10:16:34 AM"
-    return datetime.strptime(timestamp, "%m/%d/%Y %I:%M:%S %p").timestamp()
+    dt = datetime.strptime(timestamp, "%m/%d/%Y %I:%M:%S %p")
+    if country is not None:
+        tz = timezone(country)
+        dt = tz.localize(dt)
+    print(dt.timestamp())
+    return dt.timestamp()
 
 
 class LibreLinkUpClient:
     def __init__(
         self,
         username: str,
         password: str,
@@ -42,27 +54,29 @@
             "accept-encoding": "gzip",
             "cache-control": "no-cache",
             "connection": "Keep-Alive",
             "content-type": "application/json",
             "user-agent": "Mozilla/5.0 (Linux; Android 10; Pixel 3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.181 Mobile Safari/537.36",
         }
         self.jwt_token: Optional[str] = None
+        self.country: Optional[str] = None
 
     def login(self) -> None:
         """
         Log in to the LibreLinkUp API and set the JWT token
         """
         response = requests.post(
             f"{self.url}/llu/auth/login",
             headers=self.headers,
             json={"email": self.username, "password": self.password},
         )
         response.raise_for_status()
         data = response.json()
         self.jwt_token = data["data"]["authTicket"]["token"]
+        self.country = data["data"]["user"]["country"]
         self.headers["Authorization"] = f"Bearer {self.jwt_token}"
 
     @property
     def connection(self) -> Connection:
         if not hasattr(self, "_connection"):
             self._connection = self.get_connection()
         return self._connection
@@ -146,15 +160,16 @@
         raw_graph_data = self.get_raw_graph_readings()
         graph_data = raw_graph_data["data"]["graphData"]
         glucose_readings = []
         for reading in graph_data:
             glucose_readings.append(
                 GlucoseSensorReading(
                     unix_timestamp=_convert_timestamp_string_to_datetime(
-                        reading["Timestamp"]
+                        reading["Timestamp"],
+                        self.country,
                     ),
                     value=reading["Value"],
                     value_in_mg_per_dl=reading["ValueInMgPerDl"],
                     source=ReadingSource.GRAPH,
                 )
             )
         return glucose_readings
@@ -193,15 +208,16 @@
         """
         response = self.get_raw_logbook_readings()
         logbook_data = []
         for logbook_entry in response["data"]:
             logbook_data.append(
                 GlucoseSensorReading(
                     unix_timestamp=_convert_timestamp_string_to_datetime(
-                        logbook_entry["Timestamp"]
+                        logbook_entry["Timestamp"],
+                        self.country,
                     ),
                     value=logbook_entry["Value"],
                     value_in_mg_per_dl=logbook_entry["ValueInMgPerDl"],
                     source=ReadingSource.LOGBOOK,
                 )
             )
         return logbook_data
@@ -219,14 +235,31 @@
                     source="latest_reading",
                 )
         """
         resp = self.get_raw_graph_readings()
         raw_reading = resp["data"]["connection"]["glucoseMeasurement"]
         latest_reading = GlucoseSensorReading(
             unix_timestamp=_convert_timestamp_string_to_datetime(
-                raw_reading["Timestamp"]
+                raw_reading["Timestamp"],
+                self.country,
             ),
             value=raw_reading["Value"],
             value_in_mg_per_dl=raw_reading["ValueInMgPerDl"],
             source=ReadingSource.LATEST_READING,
         )
         return latest_reading
+
+
+if __name__ == "__main__":
+    import os
+    import dotenv
+
+    dotenv.load_dotenv()
+
+    client = LibreLinkUpClient(
+        username=os.environ["LIBRE_LINK_UP_USERNAME"],
+        password=os.environ["LIBRE_LINK_UP_PASSWORD"],
+        url=os.environ["LIBRE_LINK_UP_URL"],
+        version=os.getenv("LIBRE_LINK_UP_VERSION", "4.7.0"),
+    )
+    client.login()
+    print(client.get_latest_reading())
```

### Comparing `libre_linkup_py-0.2.1/src/libre_link_up/types.py` & `libre_linkup_py-0.2.2/src/libre_link_up/custom_types.py`

 * *Files identical despite different names*

### Comparing `libre_linkup_py-0.2.1/tests/test_client.py` & `libre_linkup_py-0.2.2/tests/test_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+from datetime import datetime
 import pytest
-from libre_link_up.client import LibreLinkUpClient
-from libre_link_up.types import ReadingSource
+import pytz
+from libre_link_up.client import (
+    LibreLinkUpClient,
+    _convert_timestamp_string_to_datetime,
+)
+from libre_link_up.custom_types import ReadingSource
 
 
 @pytest.mark.dependency()
 def test_login(client: LibreLinkUpClient) -> None:
     client.login()
     assert client.jwt_token is not None
 
@@ -70,7 +75,22 @@
 @pytest.mark.dependency(depends=["test_login"])
 def test_get_glucose_data(client: LibreLinkUpClient) -> None:
     glucose_data = client.get_latest_reading()
     assert glucose_data.unix_timestamp is not None
     assert glucose_data.value is not None
     assert glucose_data.value_in_mg_per_dl is not None
     assert glucose_data.source == ReadingSource.LATEST_READING
+
+
+def test_without_timezone():
+    timestamp = "4/1/2024 4:36:19 PM"
+    expected = datetime.strptime(timestamp, "%m/%d/%Y %I:%M:%S %p").timestamp()
+    result = _convert_timestamp_string_to_datetime(timestamp, None)
+    assert result == 1711989379.0
+
+
+def test_with_timezone():
+    timestamp = "4/1/2024 4:36:19 PM"
+    country = "GB"
+    dt = datetime.strptime(timestamp, "%m/%d/%Y %I:%M:%S %p")
+    result = _convert_timestamp_string_to_datetime(timestamp, country)
+    assert result == 1711985779.0
```

### Comparing `libre_linkup_py-0.2.1/LICENSE` & `libre_linkup_py-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libre_linkup_py-0.2.1/README.md` & `libre_linkup_py-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `libre_linkup_py-0.2.1/pyproject.toml` & `libre_linkup_py-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "libre-linkup-py"
-version = "0.2.1"
+version = "0.2.2"
 description = "Unofficial libre linkup python client"
 authors = [{ name = "Sam Purkis", email = "sam.purkis@hotmail.co.uk" }]
-dependencies = ["python-dotenv>=1.0.1", "requests>=2.31.0"]
+dependencies = ["python-dotenv>=1.0.1", "requests>=2.31.0", "pytz>=2024.1"]
 readme = "README.md"
 requires-python = ">= 3.9"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `libre_linkup_py-0.2.1/PKG-INFO` & `libre_linkup_py-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.3
 Name: libre-linkup-py
-Version: 0.2.1
+Version: 0.2.2
 Summary: Unofficial libre linkup python client
 Author-email: Sam Purkis <sam.purkis@hotmail.co.uk>
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: python-dotenv>=1.0.1
+Requires-Dist: pytz>=2024.1
 Requires-Dist: requests>=2.31.0
 Description-Content-Type: text/markdown
 
 # Libre-linkup-py
 
 ## TL;DR
```

