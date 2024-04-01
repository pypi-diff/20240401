# Comparing `tmp/aioecopanel-0.0.8.tar.gz` & `tmp/aioecopanel-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioecopanel-0.0.8.tar", last modified: Sat Mar 23 17:49:32 2024, max compression
+gzip compressed data, was "aioecopanel-0.0.9.tar", last modified: Mon Apr  1 18:06:43 2024, max compression
```

## Comparing `aioecopanel-0.0.8.tar` & `aioecopanel-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-23 17:49:32.953660 aioecopanel-0.0.8/
--rw-rw-rw-   0        0        0    11558 2022-12-30 12:25:35.000000 aioecopanel-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      849 2024-03-23 17:49:32.952662 aioecopanel-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-03-17 09:24:05.000000 aioecopanel-0.0.8/README.md
--rw-rw-rw-   0        0        0      690 2024-03-23 17:46:53.000000 aioecopanel-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-23 17:49:32.954659 aioecopanel-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-23 17:49:32.911723 aioecopanel-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-03-23 17:49:32.931668 aioecopanel-0.0.8/src/aioecopanel/
--rw-rw-rw-   0        0        0      471 2024-03-17 09:28:07.000000 aioecopanel-0.0.8/src/aioecopanel/__init__.py
--rw-rw-rw-   0        0        0     9243 2024-03-23 17:40:19.000000 aioecopanel-0.0.8/src/aioecopanel/aioecopanel.py
--rw-rw-rw-   0        0        0    12973 2024-03-17 09:23:55.000000 aioecopanel-0.0.8/src/aioecopanel/const.py
--rw-rw-rw-   0        0        0      803 2024-03-17 09:29:25.000000 aioecopanel-0.0.8/src/aioecopanel/exceptions.py
--rw-rw-rw-   0        0        0     3741 2024-03-23 17:48:29.000000 aioecopanel-0.0.8/src/aioecopanel/models.py
-drwxrwxrwx   0        0        0        0 2024-03-23 17:49:32.950660 aioecopanel-0.0.8/src/aioecopanel.egg-info/
--rw-rw-rw-   0        0        0      849 2024-03-23 17:49:32.000000 aioecopanel-0.0.8/src/aioecopanel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2024-03-23 17:49:32.000000 aioecopanel-0.0.8/src/aioecopanel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-23 17:49:32.000000 aioecopanel-0.0.8/src/aioecopanel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-03-23 17:49:32.000000 aioecopanel-0.0.8/src/aioecopanel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 18:06:43.539318 aioecopanel-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2022-12-30 12:25:35.000000 aioecopanel-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      849 2024-04-01 18:06:43.537231 aioecopanel-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-03-17 09:24:05.000000 aioecopanel-0.0.9/README.md
+-rw-rw-rw-   0        0        0      690 2024-04-01 18:04:42.000000 aioecopanel-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 18:06:43.540229 aioecopanel-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 18:06:43.491231 aioecopanel-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 18:06:43.516228 aioecopanel-0.0.9/src/aioecopanel/
+-rw-rw-rw-   0        0        0      471 2024-03-17 09:28:07.000000 aioecopanel-0.0.9/src/aioecopanel/__init__.py
+-rw-rw-rw-   0        0        0     9243 2024-03-23 19:59:16.000000 aioecopanel-0.0.9/src/aioecopanel/aioecopanel.py
+-rw-rw-rw-   0        0        0    13030 2024-04-01 18:04:42.000000 aioecopanel-0.0.9/src/aioecopanel/const.py
+-rw-rw-rw-   0        0        0      807 2024-04-01 18:05:33.000000 aioecopanel-0.0.9/src/aioecopanel/exceptions.py
+-rw-rw-rw-   0        0        0     3904 2024-04-01 18:06:21.000000 aioecopanel-0.0.9/src/aioecopanel/models.py
+drwxrwxrwx   0        0        0        0 2024-04-01 18:06:43.535230 aioecopanel-0.0.9/src/aioecopanel.egg-info/
+-rw-rw-rw-   0        0        0      849 2024-04-01 18:06:43.000000 aioecopanel-0.0.9/src/aioecopanel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2024-04-01 18:06:43.000000 aioecopanel-0.0.9/src/aioecopanel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 18:06:43.000000 aioecopanel-0.0.9/src/aioecopanel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-01 18:06:43.000000 aioecopanel-0.0.9/src/aioecopanel.egg-info/top_level.txt
```

### Comparing `aioecopanel-0.0.8/LICENSE.txt` & `aioecopanel-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aioecopanel-0.0.8/PKG-INFO` & `aioecopanel-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioecopanel
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package to be used for the Home Assistant Bepacom Integration for displaying BACnet devices.
 Author-email: Luuk Geertsema <s1136643@windesheim.nl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aioecopanel-0.0.8/pyproject.toml` & `aioecopanel-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "aiohttp", "yarl"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aioecopanel"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Luuk Geertsema", email="s1136643@windesheim.nl" },
 ]
 description = "A package to be used for the Home Assistant Bepacom Integration for displaying BACnet devices."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aioecopanel-0.0.8/src/aioecopanel/aioecopanel.py` & `aioecopanel-0.0.9/src/aioecopanel/aioecopanel.py`

 * *Files identical despite different names*

### Comparing `aioecopanel-0.0.8/src/aioecopanel/const.py` & `aioecopanel-0.0.9/src/aioecopanel/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from dataclasses import dataclass
 from enum import Enum
+import logging
 
+LOGGER = logging.getLogger(__package__)
 
 @dataclass
 class PropertyIdentifier(Enum):
     absenteeLimit = 244
     acceptedModes = 175
     accessAlarmEvents = 245
     accessDoors = 246
```

### Comparing `aioecopanel-0.0.8/src/aioecopanel/exceptions.py` & `aioecopanel-0.0.9/src/aioecopanel/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     """EcoPanel connection timeout exception."""
 
 
 class EcoPanelConnectionClosed(EcoPanelConnectionError):
     """EcoPanel connection closed."""
 
 
-class DeviceDictError(Exception):
+class DeviceDictError(EcoPanelError):
     """Generic Device dictionary exception."""
 
 
 class DeviceDictObjectEmpty(DeviceDictError):
     """Device dictionary object is empty."""
```

### Comparing `aioecopanel-0.0.8/src/aioecopanel/models.py` & `aioecopanel-0.0.9/src/aioecopanel/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """ Model for BACnet add-on data."""
 from dataclasses import dataclass
 from typing import Any, Union
 
 from .exceptions import DeviceDictEmpty, DeviceDictError, DeviceDictObjectEmpty
 
+from .const import LOGGER
+
 
 @dataclass
 class Object:
     """Represent a BACnet object."""
 
     objectIdentifier: str
     objectType: str
@@ -23,14 +25,15 @@
     vendorName: str
     modelName: str
     stateText: list
     numberOfStates: int
     notificationClass: int
     minPresValue: Union[int, float, str, bool]
     maxPresValue: Union[int, float, str, bool]
+    resolution: Union[int, float]
 
     def __post_init__(self):
         if self.objectIdentifier is None:
             raise DeviceDictObjectEmpty("objectIdentifier missing!")
 
     @property
     def id(self):
@@ -48,15 +51,15 @@
 @dataclass
 class Device:
     """Represent a BACnet Device."""
 
     objects: dict[str, Object]
 
     @staticmethod
-    def update_device(device_data: dict[str, Any]):
+    def update_device(device_name: str, device_data: dict[str, Any]):
         """Update the device from device data."""
         objects = {}
         for object_name, object_data in device_data.items():
             try:
                 object = Object(
                     object_data.get("objectIdentifier"),
                     object_data.get("objectType"),
@@ -72,18 +75,19 @@
                     object_data.get("vendorName"),
                     object_data.get("modelName"),
                     object_data.get("stateText"),
                     object_data.get("numberOfStates"),
                     object_data.get("notificationClass"),
                     object_data.get("minPresValue"),
                     object_data.get("maxPresValue"),
+                    object_data.get("resolution"),
                 )
                 objects.update({object_name: object})
             except DeviceDictObjectEmpty as err:
-                raise DeviceDictObjectEmpty(f"{object_name}, {object_data}: {err}")
+                LOGGER.warning(f"{device_name} {object_name}, {object_data}: {err}")
 
         return Device(objects)
 
     def __getattr__(self, name):
         try:
             return self.objects[name]
         except KeyError:
@@ -96,18 +100,18 @@
     devices: dict[str, Device] = {}
 
     def __init__(self, data: dict[str, Any]):
         if data is None:
             raise DeviceDictEmpty(f"Received empty data: {data}")
         self.update_from_data(data)
 
-    def update_from_data(self, data: dict[str, Device]):
+    def update_from_data(self, data: dict[str,Device | dict[str,Any]]):
         """Update the device dictionary from received data"""
         if data is None:
             raise DeviceDictEmpty(f"Received empty data: {data}")
         for device_name, device_data in data.items():
-            device = Device.update_device(device_data)
+            device = Device.update_device(device_name, device_data)
             self.devices.update({device_name: device})
         if self is not None:
             return self
         else:
             raise DeviceDictEmpty(f"Previous None checks didn't prevent this!'")
```

### Comparing `aioecopanel-0.0.8/src/aioecopanel.egg-info/PKG-INFO` & `aioecopanel-0.0.9/src/aioecopanel.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioecopanel
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package to be used for the Home Assistant Bepacom Integration for displaying BACnet devices.
 Author-email: Luuk Geertsema <s1136643@windesheim.nl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

