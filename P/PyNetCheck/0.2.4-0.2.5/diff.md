# Comparing `tmp/pynetcheck-0.2.4.tar.gz` & `tmp/pynetcheck-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynetcheck-0.2.4.tar", max compression
+gzip compressed data, was "pynetcheck-0.2.5.tar", max compression
```

## Comparing `pynetcheck-0.2.4.tar` & `pynetcheck-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1094 2023-10-17 17:21:13.864484 pynetcheck-0.2.4/LICENSE
--rw-r--r--   0        0        0      207 2023-12-15 17:15:33.098831 pynetcheck-0.2.4/pynetcheck/__init__.py
--rw-r--r--   0        0        0        0 2023-12-14 17:09:53.760561 pynetcheck-0.2.4/pynetcheck/models/__init__.py
--rw-r--r--   0        0        0     2187 2023-12-15 17:15:33.112987 pynetcheck-0.2.4/pynetcheck/models/device.py
--rw-r--r--   0        0        0      522 2023-12-15 17:15:33.094330 pynetcheck-0.2.4/pynetcheck/models/shared.py
--rw-r--r--   0        0        0      191 2023-12-15 17:32:52.528437 pynetcheck-0.2.4/pynetcheck/pytest.ini
--rw-r--r--   0        0        0        0 2023-10-17 17:16:48.410387 pynetcheck-0.2.4/pynetcheck/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-12-14 16:44:32.386339 pynetcheck-0.2.4/pynetcheck/tests/cisco/__init__.py
--rw-r--r--   0        0        0      797 2023-12-15 15:13:21.441564 pynetcheck-0.2.4/pynetcheck/tests/cisco/conftest.py
--rw-r--r--   0        0        0     2824 2023-12-15 17:17:31.291109 pynetcheck-0.2.4/pynetcheck/tests/cisco/test_servers.py
--rw-r--r--   0        0        0     1461 2023-12-15 17:15:33.104369 pynetcheck-0.2.4/pynetcheck/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-12-14 18:28:19.306024 pynetcheck-0.2.4/pynetcheck/tests/cve/__init__.py
--rw-r--r--   0        0        0        0 2023-12-14 18:28:19.315998 pynetcheck-0.2.4/pynetcheck/tests/cve/cisco/__init__.py
--rw-r--r--   0        0        0     5195 2023-12-15 17:15:33.087865 pynetcheck-0.2.4/pynetcheck/tests/cve/cisco/test_cve_2023_20198_ios_xe.py
--rw-r--r--   0        0        0     1322 2023-12-15 17:32:32.825845 pynetcheck-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     8670 2023-12-15 17:28:57.176545 pynetcheck-0.2.4/README.md
--rw-r--r--   0        0        0     9710 1970-01-01 00:00:00.000000 pynetcheck-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-10-17 17:21:13.864484 pynetcheck-0.2.5/LICENSE
+-rw-r--r--   0        0        0      207 2024-04-01 17:38:30.516449 pynetcheck-0.2.5/pynetcheck/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 17:38:30.517432 pynetcheck-0.2.5/pynetcheck/models/__init__.py
+-rw-r--r--   0        0        0     2179 2024-04-01 17:38:30.517432 pynetcheck-0.2.5/pynetcheck/models/device.py
+-rw-r--r--   0        0        0      965 2024-04-01 17:38:30.518492 pynetcheck-0.2.5/pynetcheck/models/shared.py
+-rw-r--r--   0        0        0      191 2024-04-01 17:38:30.518492 pynetcheck-0.2.5/pynetcheck/pytest.ini
+-rw-r--r--   0        0        0        0 2024-04-01 17:38:30.519511 pynetcheck-0.2.5/pynetcheck/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 17:38:30.519511 pynetcheck-0.2.5/pynetcheck/tests/cisco/__init__.py
+-rw-r--r--   0        0        0      819 2024-04-01 17:38:30.519511 pynetcheck-0.2.5/pynetcheck/tests/cisco/conftest.py
+-rw-r--r--   0        0        0     2824 2024-04-01 17:38:30.520511 pynetcheck-0.2.5/pynetcheck/tests/cisco/test_servers.py
+-rw-r--r--   0        0        0     1520 2024-04-01 17:38:30.520511 pynetcheck-0.2.5/pynetcheck/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-01 17:38:30.520511 pynetcheck-0.2.5/pynetcheck/tests/cve/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 17:38:30.521511 pynetcheck-0.2.5/pynetcheck/tests/cve/cisco/__init__.py
+-rw-r--r--   0        0        0     5195 2024-04-01 17:38:30.522515 pynetcheck-0.2.5/pynetcheck/tests/cve/cisco/test_cve_2023_20198_ios_xe.py
+-rw-r--r--   0        0        0     1989 2024-04-01 17:38:30.522515 pynetcheck-0.2.5/pynetcheck/tests/cve/cisco/test_cve_2024_20278.py
+-rw-r--r--   0        0        0     1321 2024-04-01 17:38:30.523511 pynetcheck-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     8670 2024-04-01 17:38:30.513432 pynetcheck-0.2.5/README.md
+-rw-r--r--   0        0        0     9709 1970-01-01 00:00:00.000000 pynetcheck-0.2.5/PKG-INFO
```

### Comparing `pynetcheck-0.2.4/LICENSE` & `pynetcheck-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pynetcheck-0.2.4/pynetcheck/models/device.py` & `pynetcheck-0.2.5/pynetcheck/models/device.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,10 +63,10 @@
             if self.config.start
             else None
         )
         if self.config.current:
             self.parsed_config = ParsedConfig(current, startup)
 
     def get_config(self):
-        self.config = self.inventory.get_config(self.ipf)
+        self.config = self.inventory.get_config()
         if self.config and self.inventory.vendor == "cisco":
             self._cisco_config()
```

### Comparing `pynetcheck-0.2.4/pynetcheck/tests/cisco/test_servers.py` & `pynetcheck-0.2.5/pynetcheck/tests/cisco/test_servers.py`

 * *Files identical despite different names*

### Comparing `pynetcheck-0.2.4/pynetcheck/tests/conftest.py` & `pynetcheck-0.2.5/pynetcheck/tests/conftest.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import os
-from pathlib import Path
-from typing import Optional, Any
-
-from ipfabric import IPFClient
-from pydantic import BaseModel
-
-IPF, CONFIGS = None, []
-
-
-class ConfigFile(BaseModel):
-    file: Path
-    parsed: Optional[Any] = None
-
-
-def check_ipfabric(ipf):
-    """Check IP Fabric Settings if Configs Exists."""
-    settings = []
-    try:
-        settings = [
-            d["taskId"]
-            for d in ipf.get(f"snapshots/{ipf.snapshot_id}/settings").json()[
-                "discoveryTasks"
-            ]
-        ]
-    except:
-        print("Could not get Snapshot please check the token policies/roles.")
-
-    if "tasks/deviceConfig/configSaved" in settings:
-        raise NotImplementedError(
-            "Saved Config Consistency Discovery Task Not Enabled."
-        )
-
-
-def pytest_addoption(parser):
-    parser.addoption(
-        "--config-dir",
-        help="Path to directory with configurations.",
-        action="store",
-        type=Path,
-    )
-    parser.addoption(
-        "--snapshot",
-        help="IP Fabric Snapshot ID.",
-        action="store",
-        default="$last",
-        type=str,
-    )
-
-
-def pytest_configure(config):
-    global IPF, CONFIGS
-
-    if config.getoption("--config-dir"):
-        cfg_dir = config.getoption("--config-dir").resolve()
-        CONFIGS = [ConfigFile(file=cfg_dir / f) for f in os.listdir(cfg_dir)]
-    else:
-        IPF = IPFClient(snapshot_id=config.getoption("--snapshot"))
-        check_ipfabric(IPF)
+import os
+from pathlib import Path
+from typing import Optional, Any
+
+from ipfabric import IPFClient
+from pydantic import BaseModel
+
+IPF, CONFIGS = None, []
+
+
+class ConfigFile(BaseModel):
+    file: Path
+    parsed: Optional[Any] = None
+
+
+def check_ipfabric(ipf):
+    """Check IP Fabric Settings if Configs Exists."""
+    settings = []
+    try:
+        settings = [
+            d["taskId"]
+            for d in ipf.get(f"snapshots/{ipf.snapshot_id}/settings").json()[
+                "discoveryTasks"
+            ]
+        ]
+    except:
+        print("Could not get Snapshot please check the token policies/roles.")
+
+    if "tasks/deviceConfig/configSaved" in settings:
+        raise NotImplementedError(
+            "Saved Config Consistency Discovery Task Not Enabled."
+        )
+
+
+def pytest_addoption(parser):
+    parser.addoption(
+        "--config-dir",
+        help="Path to directory with configurations.",
+        action="store",
+        type=Path,
+    )
+    parser.addoption(
+        "--snapshot",
+        help="IP Fabric Snapshot ID.",
+        action="store",
+        default="$last",
+        type=str,
+    )
+
+
+def pytest_configure(config):
+    global IPF, CONFIGS
+
+    if config.getoption("--config-dir"):
+        cfg_dir = config.getoption("--config-dir").resolve()
+        CONFIGS = [ConfigFile(file=cfg_dir / f) for f in os.listdir(cfg_dir)]
+    else:
+        IPF = IPFClient(snapshot_id=config.getoption("--snapshot"))
+        check_ipfabric(IPF)
```

### Comparing `pynetcheck-0.2.4/pynetcheck/tests/cve/cisco/test_cve_2023_20198_ios_xe.py` & `pynetcheck-0.2.5/pynetcheck/tests/cve/cisco/test_cve_2023_20198_ios_xe.py`

 * *Files identical despite different names*

### Comparing `pynetcheck-0.2.4/pyproject.toml` & `pynetcheck-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyNetCheck"
-version = "0.2.4"
+version = "0.2.5"
 license = "MIT"
 description = "Python Network device checker using Pytest and IP Fabric."
 authors = [
     "Solution Architecture <solution.architecture@ipfabric.io>",
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
 ]
 readme = "README.md"
@@ -16,17 +16,17 @@
 
 [tool.poetry.urls]
 "IP Fabric" = "https://ipfabric.io/"
 "Changelog" = "https://gitlab.com/ip-fabric/integrations/pynetcheck/-/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-ipfabric = "^6.5.0"
-ciscoconfparse = "^1.7.24"
-pytest = "^7.4.2"
+ipfabric = "^6.7.0"
+ciscoconfparse = "^1.9.0"
+pytest = "^8.0.0"
 pytest-html-reporter = "^0.2.9"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.12.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `pynetcheck-0.2.4/README.md` & `pynetcheck-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pynetcheck-0.2.4/PKG-INFO` & `pynetcheck-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: PyNetCheck
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python Network device checker using Pytest and IP Fabric.
 Home-page: https://gitlab.com/ip-fabric/integrations/pynetcheck
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Solution Architecture
 Author-email: solution.architecture@ipfabric.io
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ciscoconfparse (>=1.7.24,<2.0.0)
-Requires-Dist: ipfabric (>=6.5.0,<7.0.0)
-Requires-Dist: pytest (>=7.4.2,<8.0.0)
+Requires-Dist: ciscoconfparse (>=1.9.0,<2.0.0)
+Requires-Dist: ipfabric (>=6.7.0,<7.0.0)
+Requires-Dist: pytest (>=8.0.0,<9.0.0)
 Requires-Dist: pytest-html-reporter (>=0.2.9,<0.3.0)
 Project-URL: Changelog, https://gitlab.com/ip-fabric/integrations/pynetcheck/-/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://gitlab.com/ip-fabric/integrations/pynetcheck
 Project-URL: IP Fabric, https://ipfabric.io/
 Project-URL: Repository, https://gitlab.com/ip-fabric/integrations/pynetcheck
 Description-Content-Type: text/markdown
```

