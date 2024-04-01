# Comparing `tmp/aiolyric-1.1.1.tar.gz` & `tmp/aiolyric-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiolyric-1.1.1.tar", last modified: Mon Dec  4 09:12:13 2023, max compression
+gzip compressed data, was "aiolyric-2.0.0.tar", last modified: Mon Apr  1 13:38:37 2024, max compression
```

## Comparing `aiolyric-1.1.1.tar` & `aiolyric-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 09:12:13.540837 aiolyric-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-12-04 09:12:04.000000 aiolyric-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-12-04 09:12:13.540837 aiolyric-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2023-12-04 09:12:04.000000 aiolyric-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 09:12:13.536837 aiolyric-1.1.1/aiolyric/
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2023-12-04 09:12:04.000000 aiolyric-1.1.1/aiolyric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 09:12:13.540837 aiolyric-1.1.1/aiolyric/client/
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2023-12-04 09:12:04.000000 aiolyric-1.1.1/aiolyric/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-12-04 09:12:04.000000 aiolyric-1.1.1/aiolyric/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-12-04 09:12:04.000000 aiolyric-1.1.1/aiolyric/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 09:12:13.540837 aiolyric-1.1.1/aiolyric/objects/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-04 09:12:04.000000 aiolyric-1.1.1/aiolyric/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-12-04 09:12:04.000000 aiolyric-1.1.1/aiolyric/objects/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7737 2023-12-04 09:12:04.000000 aiolyric-1.1.1/aiolyric/objects/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2023-12-04 09:12:04.000000 aiolyric-1.1.1/aiolyric/objects/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2023-12-04 09:12:04.000000 aiolyric-1.1.1/aiolyric/objects/priority.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 09:12:13.540837 aiolyric-1.1.1/aiolyric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-12-04 09:12:13.000000 aiolyric-1.1.1/aiolyric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-12-04 09:12:13.000000 aiolyric-1.1.1/aiolyric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 09:12:13.000000 aiolyric-1.1.1/aiolyric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-04 09:12:13.000000 aiolyric-1.1.1/aiolyric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-04 09:12:13.000000 aiolyric-1.1.1/aiolyric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-04 09:12:13.540837 aiolyric-1.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      565 2023-12-04 09:12:04.000000 aiolyric-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:38:37.892058 aiolyric-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 13:38:16.000000 aiolyric-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-01 13:38:37.892058 aiolyric-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-01 13:38:16.000000 aiolyric-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:38:37.888058 aiolyric-2.0.0/aiolyric/
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:38:37.888058 aiolyric-2.0.0/aiolyric/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/objects/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/objects/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/objects/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-01 13:38:16.000000 aiolyric-2.0.0/aiolyric/objects/priority.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:38:37.892058 aiolyric-2.0.0/aiolyric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-01 13:38:37.000000 aiolyric-2.0.0/aiolyric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-01 13:38:37.000000 aiolyric-2.0.0/aiolyric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:38:37.000000 aiolyric-2.0.0/aiolyric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-01 13:38:37.000000 aiolyric-2.0.0/aiolyric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 13:38:37.000000 aiolyric-2.0.0/aiolyric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-04-01 13:38:16.000000 aiolyric-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:38:37.892058 aiolyric-2.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1011 2024-04-01 13:38:16.000000 aiolyric-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:38:37.888058 aiolyric-2.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:38:37.892058 aiolyric-2.0.0/tests/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-01 13:38:16.000000 aiolyric-2.0.0/tests/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-01 13:38:16.000000 aiolyric-2.0.0/tests/objects/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11160 2024-04-01 13:38:16.000000 aiolyric-2.0.0/tests/objects/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-01 13:38:16.000000 aiolyric-2.0.0/tests/objects/test_priority.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-01 13:38:16.000000 aiolyric-2.0.0/tests/test__version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-01 13:38:16.000000 aiolyric-2.0.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-01 13:38:16.000000 aiolyric-2.0.0/tests/test_init.py
```

### Comparing `aiolyric-1.1.1/PKG-INFO` & `aiolyric-2.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: aiolyric
-Version: 1.1.1
-Summary: AIO package for the Honeywell Lyric Platform.
+Version: 2.0.0
+Summary: Python package for the Honeywell Lyric Platform
 Home-page: https://github.com/timmo001/aiolyric
 Author: Aidan Timson (Timmo)
-Author-email: contact@timmo.xyz
-License: MIT
-Keywords: honeywell lyric thermostat
+Author-email: aidan@timmo.dev
+License: Apache-2.0
+Keywords: aiolyric,api,async,asyncio,honeywell lyric,honeywell,lyric,integration
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp>=3.7.3
+Requires-Dist: aiohttp>=3.9.0b0; python_version >= "3.12"
+Requires-Dist: aiohttp>=3.8.5; python_version < "3.12"
+Requires-Dist: incremental>=22.10.0
 
-# AIOLyric
+# aiolyric
 
 Python package for the Honeywell Lyric Platform.
 
 ## Attributions / Contributions
 
 - [@bramkragten](https://github.com/bramkragten) for the original implementation. Referenced his [package](https://github.com/bramkragten/python-lyric) quite a bit whilst writing this one.
 - [@ludeeus](https://github.com/ludeeus) for his generator class. Made reading json into objects super simple. :tada:
```

### Comparing `aiolyric-1.1.1/aiolyric/__init__.py` & `aiolyric-2.0.0/aiolyric/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,67 @@
-"""Lyric: Init"""
-from typing import List
+"""Lyric."""
+
+import logging
 
 from aiohttp import ClientResponse
 
+from .client import LyricClient
 from .const import BASE_URL
-from .objects.base import LyricBase
 from .objects.device import LyricDevice
 from .objects.location import LyricLocation
 from .objects.priority import LyricPriority, LyricRoom
 
 
-class Lyric(LyricBase):
+class Lyric:
     """Handles authentication refresh tokens."""
 
+    logger = logging.getLogger(__name__)
+
     def __init__(
         self,
-        client: "LyricClient",
+        client: LyricClient,
         client_id: str,
     ) -> None:
         """Initialize the token manager class."""
         self._client = client
         self._client_id = client_id
-        self._devices: List[LyricDevice] = []
+        self._devices: list[LyricDevice] = []
         self._devices_dict: dict = {}
-        self._locations: List[LyricLocation] = []
+        self._locations: list[LyricLocation] = []
         self._locations_dict: dict = {}
-        self._rooms_dict: dict = {}    
+        self._rooms_dict: dict = {}
 
     @property
     def client_id(self) -> str:
+        """Return the client id."""
         return self._client_id
 
     @property
-    def devices(self) -> List[LyricDevice]:
+    def devices(self) -> list[LyricDevice]:
+        """Return the devices."""
         return self._devices
 
     @property
     def devices_dict(self) -> dict:
+        """Return the devices dict."""
         return self._devices_dict
 
     @property
-    def locations(self) -> List[LyricLocation]:
+    def locations(self) -> list[LyricLocation]:
+        """Return the locations."""
         return self._locations
 
     @property
     def locations_dict(self) -> dict:
+        """Return the locations dict."""
         return self._locations_dict
 
     @property
     def rooms_dict(self) -> dict[str, dict[str, LyricRoom]]:
+        """Return the rooms dict."""
         return self._rooms_dict
 
     async def get_devices(
         self,
         location_id: int,
     ) -> None:
         """Get Devices."""
@@ -60,128 +69,126 @@
             f"{BASE_URL}/devices?apikey={self.client_id}&locationId={location_id}"
         )
         json = await response.json()
         self.logger.debug(json)
         self._devices = [LyricDevice(self._client, device) for device in json or []]
         self._devices_dict: dict = {}
         for device in self._devices:
-            self._devices_dict[device.macID] = device
+            self._devices_dict[device.mac_id] = device
 
     async def get_locations(self) -> None:
         """Get Locations."""
         response: ClientResponse = await self._client.get(
             f"{BASE_URL}/locations?apikey={self.client_id}"
         )
         json = await response.json()
         self.logger.debug(json)
         self._locations = [
             LyricLocation(self._client, location) for location in json or []
         ]
         self._locations_dict: dict = {}
         for location in self._locations:
-            self._locations_dict[location.locationID] = location
+            self._locations_dict[location.location_id] = location
 
     async def get_thermostat_rooms(
-            self,
-            location_id: int,
-            device_id: str
-        ) -> None:
+        self,
+        location_id: int,
+        device_id: str,
+    ) -> None:
         """Get Priority, which contains accessory information."""
         response: ClientResponse = await self._client.get(
             f"{BASE_URL}/devices/thermostats/{device_id}/priority?apikey={self.client_id}&locationId={location_id}"
         )
         json = await response.json()
         self.logger.debug(json)
-        
+
         priority = LyricPriority(json)
 
-        macId = priority.deviceId   # device id in the priority payload refers to the mac address of the device
-        self._rooms_dict[macId]: dict = {}
-        
+        # device id in the priority payload refers to the mac address of the device
+        mac_id = priority.device_id
+        self._rooms_dict[mac_id] = {}
+
         # add each room to the room dictionary. Rooms contain motion, temp, and humidity averages for all accessories in a room
-        for room in priority.currentPriority.rooms:
-            self._rooms_dict[macId][room.id] = room
+        for room in priority.current_priority.rooms:
+            self._rooms_dict[mac_id][room.id] = room
 
     async def update_thermostat(
         self,
         location: LyricLocation,
         device: LyricDevice,
-        mode=None,
-        heatSetpoint=None,
-        coolSetpoint=None,
-        autoChangeoverActive=None,
-        thermostatSetpointStatus=None,
-        nextPeriodTime=None,
+        mode: str | None = None,
+        heat_setpoint: int | float | None = None,
+        cool_setpoint: int | float | None = None,
+        auto_changeover_active: bool | None = None,
+        thermostat_setpoint_status: str | None = None,
+        next_period_time: str | None = None,
     ) -> ClientResponse:
         """Update Theremostat."""
         self.logger.debug("Update Thermostat")
 
         data = {}
 
         if mode is not None:
             data["mode"] = mode
         else:
-            data["mode"] = device.changeableValues.mode
+            data["mode"] = device.changeable_values.mode
 
-        if heatSetpoint is not None:
-            data["heatSetpoint"] = heatSetpoint
+        if heat_setpoint is not None:
+            data["heatSetpoint"] = heat_setpoint
         else:
-            data["heatSetpoint"] = device.changeableValues.heatSetpoint
-        if coolSetpoint is not None:
-            data["coolSetpoint"] = coolSetpoint
+            data["heatSetpoint"] = device.changeable_values.heat_setpoint
+        if cool_setpoint is not None:
+            data["coolSetpoint"] = cool_setpoint
         else:
-            data["coolSetpoint"] = device.changeableValues.coolSetpoint
+            data["coolSetpoint"] = device.changeable_values.cool_setpoint
 
         # Only for TCC devices
-        if autoChangeoverActive is not None:
-            data["autoChangeoverActive"] = autoChangeoverActive
-        elif device.changeableValues.autoChangeoverActive is not None:
-            data["autoChangeoverActive"] = device.changeableValues.autoChangeoverActive
+        if auto_changeover_active is not None:
+            data["autoChangeoverActive"] = auto_changeover_active
+        elif device.changeable_values.auto_changeover_active is not None:
+            data["autoChangeoverActive"] = (
+                device.changeable_values.auto_changeover_active
+            )
 
         # Only for LCC devices
-        if thermostatSetpointStatus is not None:
-            data["thermostatSetpointStatus"] = thermostatSetpointStatus
-        elif device.changeableValues.thermostatSetpointStatus is not None:
-            if device.changeableValues.thermostatSetpointStatus == "NoHold":
+        if thermostat_setpoint_status is not None:
+            data["thermostatSetpointStatus"] = thermostat_setpoint_status
+        elif device.changeable_values.thermostat_setpoint_status is not None:
+            if device.changeable_values.thermostat_setpoint_status == "NoHold":
                 data["thermostatSetpointStatus"] = "TemporaryHold"
             else:
-                data[
-                    "thermostatSetpointStatus"
-                ] = device.changeableValues.thermostatSetpointStatus
+                data["thermostatSetpointStatus"] = (
+                    device.changeable_values.thermostat_setpoint_status
+                )
 
         if data.get("thermostatSetpointStatus", "") == "HoldUntil":
-            if nextPeriodTime is not None:
-                data["nextPeriodTime"] = nextPeriodTime
-            elif device.changeableValues.nextPeriodTime == "NoHold" and mode is None:
+            if next_period_time is not None:
+                data["nextPeriodTime"] = next_period_time
+            elif device.changeable_values.next_period_time == "NoHold" and mode is None:
                 data["nextPeriodTime"] = "TemporaryHold"
             else:
-                data["nextPeriodTime"] = device.changeableValues.nextPeriodTime
+                data["nextPeriodTime"] = device.changeable_values.next_period_time
 
         self.logger.debug(data)
 
         return await self._client.post(
-            f"{BASE_URL}/devices/thermostats/{device.deviceID}?apikey={self._client_id}&locationId={location.locationID}",
+            f"{BASE_URL}/devices/thermostats/{device.device_id}?apikey={self._client_id}&locationId={location.location_id}",
             json=data,
         )
 
     async def update_fan(
         self,
         location: LyricLocation,
         device: LyricDevice,
         mode: str,
     ) -> ClientResponse:
         """Update Fan."""
         self.logger.debug("Update Fan")
 
-        data = {}
-
-        if mode is not None:
-            data["mode"] = mode
-        else:
-            data["mode"] = device.fanMode
+        data = {"mode": mode}
 
         self.logger.debug(data)
 
         return await self._client.post(
-            f"{BASE_URL}/devices/thermostats/{device.deviceID}/fan?apikey={self._client_id}&locationId={location.locationID}",
+            f"{BASE_URL}/devices/thermostats/{device.device_id}/fan?apikey={self._client_id}&locationId={location.location_id}",
             json=data,
         )
```

### Comparing `aiolyric-1.1.1/aiolyric/client/__init__.py` & `aiolyric-2.0.0/aiolyric/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,69 @@
-"""Lyric: Client"""
-import async_timeout
-import logging
+"""Lyric client."""
 
 from abc import abstractmethod
-from asyncio import CancelledError, TimeoutError, get_event_loop
-from aiohttp import ClientError, ClientSession, ClientResponse
+import asyncio
+import logging
+
+from aiohttp import ClientResponse, ClientSession
 
-from ..objects.base import LyricBase
-from ..exceptions import LyricException, LyricAuthenticationException
+from .exceptions import LyricAuthenticationException, LyricException
 
 
-class LyricClient(LyricBase):
+class LyricClient:
     """Client to handle API calls."""
 
-    def __init__(self, session: ClientSession) -> None:
+    logger = logging.getLogger(__name__)
+
+    def __init__(
+        self,
+        session: ClientSession,
+    ) -> None:
         """Initialize the client."""
         self._session = session
 
     @abstractmethod
     async def async_get_access_token(self) -> str:
         """Return a valid access token."""
 
-    async def get(self, url: str, **kwargs) -> ClientResponse:
+    async def get(
+        self,
+        url: str,
+        **kwargs,
+    ) -> ClientResponse:
         """Make a GET request."""
         return await self.request("GET", url, **kwargs)
 
-    async def post(self, url: str, **kwargs) -> ClientResponse:
+    async def post(
+        self,
+        url: str,
+        **kwargs,
+    ) -> ClientResponse:
         """Make a POST request."""
-        return await self.request("POST", url, **kwargs)
+        return await self.request(
+            "POST",
+            url,
+            **kwargs,
+        )
 
     async def request(
-        self, method: str in ["GET", "POST"], url: str, **kwargs
+        self,
+        method: str,
+        url: str,
+        **kwargs,
     ) -> ClientResponse:
         """Make a request."""
-        headers = kwargs.get("headers")
-
-        if headers is None:
+        if (headers := kwargs.get("headers")) is None:
             headers = {}
-        else:
-            headers = dict(headers)
 
         access_token = await self.async_get_access_token()
         headers["Authorization"] = f"Bearer {access_token}"
         headers["Content-Type"] = "application/json"
 
-        async with async_timeout.timeout(20):
+        async with asyncio.timeout(20):
             response: ClientResponse = await self._session.request(
                 method,
                 url,
                 headers=headers,
                 **kwargs,
             )
         if response.status != 200:
@@ -61,21 +76,20 @@
                             "headers": headers,
                             **kwargs,
                         },
                         "response": await response.json(),
                         "status": response.status,
                     }
                 )
-            else:
-                raise LyricException(
-                    {
-                        "request": {
-                            "method": method,
-                            "url": url,
-                            "headers": headers,
-                            **kwargs,
-                        },
-                        "response": await response.json(),
-                        "status": response.status,
-                    }
-                )
+            raise LyricException(
+                {
+                    "request": {
+                        "method": method,
+                        "url": url,
+                        "headers": headers,
+                        **kwargs,
+                    },
+                    "response": await response.json(),
+                    "status": response.status,
+                }
+            )
         return response
```

### Comparing `aiolyric-1.1.1/aiolyric.egg-info/PKG-INFO` & `aiolyric-2.0.0/aiolyric.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: aiolyric
-Version: 1.1.1
-Summary: AIO package for the Honeywell Lyric Platform.
+Version: 2.0.0
+Summary: Python package for the Honeywell Lyric Platform
 Home-page: https://github.com/timmo001/aiolyric
 Author: Aidan Timson (Timmo)
-Author-email: contact@timmo.xyz
-License: MIT
-Keywords: honeywell lyric thermostat
+Author-email: aidan@timmo.dev
+License: Apache-2.0
+Keywords: aiolyric,api,async,asyncio,honeywell lyric,honeywell,lyric,integration
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp>=3.7.3
+Requires-Dist: aiohttp>=3.9.0b0; python_version >= "3.12"
+Requires-Dist: aiohttp>=3.8.5; python_version < "3.12"
+Requires-Dist: incremental>=22.10.0
 
-# AIOLyric
+# aiolyric
 
 Python package for the Honeywell Lyric Platform.
 
 ## Attributions / Contributions
 
 - [@bramkragten](https://github.com/bramkragten) for the original implementation. Referenced his [package](https://github.com/bramkragten/python-lyric) quite a bit whilst writing this one.
 - [@ludeeus](https://github.com/ludeeus) for his generator class. Made reading json into objects super simple. :tada:
```

