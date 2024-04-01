# Comparing `tmp/pysma-plus-0.1.0.tar.gz` & `tmp/pysma-plus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysma-plus-0.1.0.tar", last modified: Sun Mar 31 14:49:20 2024, max compression
+gzip compressed data, was "pysma-plus-0.1.1.tar", last modified: Mon Apr  1 14:09:32 2024, max compression
```

## Comparing `pysma-plus-0.1.0.tar` & `pysma-plus-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-03-31 14:49:20.204411 pysma-plus-0.1.0/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1075 2024-03-27 10:30:58.000000 pysma-plus-0.1.0/LICENSE
--rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-03-30 19:14:11.000000 pysma-plus-0.1.0/MANIFEST.in
--rw-r--r--   0 sven      (1001) sven      (1001)     2669 2024-03-31 14:49:20.204411 pysma-plus-0.1.0/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)      642 2024-03-30 18:43:59.000000 pysma-plus-0.1.0/README.md
--rw-rw-r--   0 sven      (1001) sven      (1001)      895 2024-03-31 14:49:14.000000 pysma-plus-0.1.0/pyproject.toml
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-03-31 14:49:20.204411 pysma-plus-0.1.0/pysma_plus.egg-info/
--rw-r--r--   0 sven      (1001) sven      (1001)     2669 2024-03-31 14:49:20.000000 pysma-plus-0.1.0/pysma_plus.egg-info/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)      597 2024-03-31 14:49:20.000000 pysma-plus-0.1.0/pysma_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-03-31 14:49:20.000000 pysma-plus-0.1.0/pysma_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       35 2024-03-31 14:49:20.000000 pysma-plus-0.1.0/pysma_plus.egg-info/requires.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-03-31 14:49:20.000000 pysma-plus-0.1.0/pysma_plus.egg-info/top_level.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-03-30 19:16:34.000000 pysma-plus-0.1.0/pysma_plus.egg-info/zip-safe
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-03-31 14:49:20.203411 pysma-plus-0.1.0/pysmaplus/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1920 2024-03-29 07:19:41.000000 pysma-plus-0.1.0/pysmaplus/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     6668 2024-03-31 12:59:54.000000 pysma-plus-0.1.0/pysmaplus/const.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    21131 2024-03-28 08:57:32.000000 pysma-plus-0.1.0/pysmaplus/definitions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      507 2024-03-27 12:21:42.000000 pysma-plus-0.1.0/pysmaplus/device.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-03-27 10:31:31.000000 pysma-plus-0.1.0/pysmaplus/exceptions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-03-27 10:31:31.000000 pysma-plus-0.1.0/pysmaplus/helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     6237 2024-03-31 12:44:16.000000 pysma-plus-0.1.0/pysmaplus/sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    13856 2024-03-31 13:01:52.000000 pysma-plus-0.1.0/pysmaplus/smaennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     8552 2024-03-31 12:43:42.000000 pysma-plus-0.1.0/pysmaplus/smaspeedwireem.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    16136 2024-03-27 12:04:04.000000 pysma-plus-0.1.0/pysmaplus/smawebconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-03-31 14:49:20.204411 pysma-plus-0.1.0/setup.cfg
--rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-03-31 14:49:14.000000 pysma-plus-0.1.0/setup.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-03-31 14:49:20.204411 pysma-plus-0.1.0/tests/
--rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-03-27 10:30:58.000000 pysma-plus-0.1.0/tests/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      883 2024-03-27 10:30:58.000000 pysma-plus-0.1.0/tests/test_definitions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-03-27 10:30:58.000000 pysma-plus-0.1.0/tests/test_helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    17280 2024-03-27 10:30:58.000000 pysma-plus-0.1.0/tests/test_init.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     4785 2024-03-27 10:30:58.000000 pysma-plus-0.1.0/tests/test_sensor.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-01 14:09:32.810427 pysma-plus-0.1.1/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1075 2024-03-27 10:30:58.000000 pysma-plus-0.1.1/LICENSE
+-rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-03-30 19:14:11.000000 pysma-plus-0.1.1/MANIFEST.in
+-rw-r--r--   0 sven      (1001) sven      (1001)     2669 2024-04-01 14:09:32.810427 pysma-plus-0.1.1/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)      642 2024-03-30 18:43:59.000000 pysma-plus-0.1.1/README.md
+-rw-rw-r--   0 sven      (1001) sven      (1001)      895 2024-04-01 14:09:25.000000 pysma-plus-0.1.1/pyproject.toml
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-01 14:09:32.810427 pysma-plus-0.1.1/pysma_plus.egg-info/
+-rw-r--r--   0 sven      (1001) sven      (1001)     2669 2024-04-01 14:09:32.000000 pysma-plus-0.1.1/pysma_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)      597 2024-04-01 14:09:32.000000 pysma-plus-0.1.1/pysma_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-04-01 14:09:32.000000 pysma-plus-0.1.1/pysma_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       35 2024-04-01 14:09:32.000000 pysma-plus-0.1.1/pysma_plus.egg-info/requires.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-04-01 14:09:32.000000 pysma-plus-0.1.1/pysma_plus.egg-info/top_level.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-03-30 19:16:34.000000 pysma-plus-0.1.1/pysma_plus.egg-info/zip-safe
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-01 14:09:32.810427 pysma-plus-0.1.1/pysmaplus/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1920 2024-03-29 07:19:41.000000 pysma-plus-0.1.1/pysmaplus/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6668 2024-03-31 12:59:54.000000 pysma-plus-0.1.1/pysmaplus/const.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    21131 2024-03-28 08:57:32.000000 pysma-plus-0.1.1/pysmaplus/definitions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      507 2024-03-27 12:21:42.000000 pysma-plus-0.1.1/pysmaplus/device.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-03-27 10:31:31.000000 pysma-plus-0.1.1/pysmaplus/exceptions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-03-27 10:31:31.000000 pysma-plus-0.1.1/pysmaplus/helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6237 2024-03-31 12:44:16.000000 pysma-plus-0.1.1/pysmaplus/sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    13827 2024-03-31 17:59:40.000000 pysma-plus-0.1.1/pysmaplus/smaennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     9378 2024-04-01 14:05:43.000000 pysma-plus-0.1.1/pysmaplus/smaspeedwireem.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    16136 2024-03-27 12:04:04.000000 pysma-plus-0.1.1/pysmaplus/smawebconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-04-01 14:09:32.811427 pysma-plus-0.1.1/setup.cfg
+-rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-04-01 14:09:25.000000 pysma-plus-0.1.1/setup.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-01 14:09:32.810427 pysma-plus-0.1.1/tests/
+-rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-03-27 10:30:58.000000 pysma-plus-0.1.1/tests/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      883 2024-03-27 10:30:58.000000 pysma-plus-0.1.1/tests/test_definitions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-03-27 10:30:58.000000 pysma-plus-0.1.1/tests/test_helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    17280 2024-03-27 10:30:58.000000 pysma-plus-0.1.1/tests/test_init.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     4785 2024-03-27 10:30:58.000000 pysma-plus-0.1.1/tests/test_sensor.py
```

### Comparing `pysma-plus-0.1.0/LICENSE` & `pysma-plus-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.0/PKG-INFO` & `pysma-plus-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.0
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.1
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 kellerza
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysma-plus-0.1.0/README.md` & `pysma-plus-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.0/pyproject.toml` & `pysma-plus-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysma-plus"
-version = "0.1.0"
+version = "0.1.1"
 description = "Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices"
 readme = "README.md"
 authors = [{ name = "Sven Bursch-Osewold", email = "sb_pysma@bursch.com" },{ name = "Johann Kellerman" , email ="kellerza@gmail.com"} ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pysma-plus-0.1.0/pysma_plus.egg-info/PKG-INFO` & `pysma-plus-0.1.1/pysma_plus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.0
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.1
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 kellerza
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysma-plus-0.1.0/pysma_plus.egg-info/SOURCES.txt` & `pysma-plus-0.1.1/pysma_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.0/pysmaplus/__init__.py` & `pysma-plus-0.1.1/pysmaplus/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.0/pysmaplus/const.py` & `pysma-plus-0.1.1/pysmaplus/const.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.0/pysmaplus/definitions.py` & `pysma-plus-0.1.1/pysmaplus/definitions.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.0/pysmaplus/helpers.py` & `pysma-plus-0.1.1/pysmaplus/helpers.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.0/pysmaplus/sensor.py` & `pysma-plus-0.1.1/pysmaplus/sensor.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.0/pysmaplus/smaennexos.py` & `pysma-plus-0.1.1/pysmaplus/smaennexos.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     SmaReadException,
 )
 from .sensor import Sensors
 from .device import Device
 from .const import Identifier
 
 
-# TODO Identifier.voltage_l1
 ennexosSensors = [
 
     Sensor("Coolsys.Inverter.TmpVal.1", Identifier.temp_a, factor=1, unit="°C"),
     Sensor("Coolsys.Inverter.TmpVal.2", Identifier.temp_b, factor=1, unit="°C"),
     Sensor("Coolsys.Inverter.TmpVal.3", Identifier.temp_c, factor=1, unit="°C"),
     Sensor("DcMs.Amp.1", Identifier.pv_current_a, factor=1, unit="A"),
     Sensor("DcMs.Amp.2", Identifier.pv_current_b, factor=1, unit="A"),
```

### Comparing `pysma-plus-0.1.0/pysmaplus/smaspeedwireem.py` & `pysma-plus-0.1.1/pysmaplus/smaspeedwireem.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import socket
 import struct
 import asyncio
 import copy
 import logging
 import binascii
 from typing import Any, Dict, Optional
+import datetime
 
 # https://www.unifox.at/software/sma-em-daemon/
 # https://cdn.sma.de/fileadmin/content/www.developer.sma.de/docs/EMETER-Protokoll-TI-en-10.pdf?v=1699276024
 
 
 from .sensor import Sensor
 from .const import Identifier
@@ -108,14 +109,20 @@
             group (str, optional): Username to use during login. 
 
         """
         pass
 
 
 
+    async def run(self):
+        while True:
+            await watch(self._q._connection)
+            msg = self._q.receive()
+            print(msg)
+
     async def new_session(self) -> bool:
         """Establish a new session.
 
         Returns:
             bool: authentication successful
         """
         MCAST_GRP = '239.12.255.254'
@@ -154,30 +161,51 @@
 
     async def close_session(self) -> None:
         """Close the session login."""
         # TODO
         pass
 
 
+    def getData(self):
+        """
+
+        Hack:
+            If the function is called less frequently than the device supplies data,
+            the UDP packets will be stored in the buffer.
+            If the read instruction (sock.recv) takes only milliseconds, I assume that
+            the data came from the buffer and discard it. Otherwise outdated values would
+            be used.
+            One of my most ugly hacks.
+
+        """
+        data = None
+        tries = 4
+        while tries > 0:
+            a = datetime.datetime.now()
+            data=self._decode(self._sock.recv(608))
+            b = datetime.datetime.now()
+            if data and (b-a).total_seconds() < 0.1:
+                continue
+            if data:
+                break
+            tries -= 1
+        return data
+        # TODO raise SmaConnectionException or SmaReadException if no connection after 4 tries
 
     async def read(self, sensors: Sensors) -> bool:
         """Read a set of keys.
 
         Args:
             sensors (Sensors): Sensors object containing Sensor objects to read
 
         Returns:
             bool: reading was successful
         """
         notfound = []
-        for i in range(0,4):
-            data=self._decode(self._sock.recv(608))
-            if data:
-                break
-        # TODO raise SmaConnectionException or SmaReadException if no connection after 4 tries
+        data = self.getData()
             
         for sensor in sensors:
           if (sensor.key in data):
               value = data[sensor.key]
               if (sensor.factor):
                   value /= sensor.factor
               sensor.value = value
@@ -195,18 +223,17 @@
 
     async def device_info(self) -> dict:
         """Read device info and return the results.
 
         Returns:
             dict: dict containing serial, name, type, manufacturer and sw_version
         """
-        for i in range(0,4):
-            data=self._decode(self._sock.recv(608))
-            if data:
-                break
+        notfound = []
+        data = self.getData()
+
         device_info = {
             "serial": data["serial"],
             "name": data["device"],
             "type": data["susyid"],
             "manufacturer": "SMA",
             "sw_version": data["sw_version"],
         }
@@ -220,15 +247,16 @@
 
         Returns:
             dict: Dict with all the decoded information
         """
         if p[0:4] != b"SMA\0":
             return None
         protocolID = int.from_bytes(p[16:18], byteorder="big")
-        if (protocolID != 0x6069):
+        
+        if (protocolID not in [0x6069, 0x6081]):
             _LOGGER.debug("Unknown protocoll " + str(protocolID))
             return None
         
         data = {}
         data["protocolID"] = protocolID
         data["susyid"] = int.from_bytes(p[18:20], byteorder="big")
         data["device"] = self._susyid.get(data["susyid"], "unknown")
```

### Comparing `pysma-plus-0.1.0/pysmaplus/smawebconnect.py` & `pysma-plus-0.1.1/pysmaplus/smawebconnect.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.0/setup.py` & `pysma-plus-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 """pysma library setup."""
 from pathlib import Path
 
 from setuptools import setup
 
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 URL = "https://github.com/littleyoda/pysma"
 
 setup(
     name="pysma-plus",
     version=VERSION,
     description="Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices",
     long_description=Path("README.md").read_text(),
```

### Comparing `pysma-plus-0.1.0/tests/__init__.py` & `pysma-plus-0.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.0/tests/test_definitions.py` & `pysma-plus-0.1.1/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.0/tests/test_init.py` & `pysma-plus-0.1.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.0/tests/test_sensor.py` & `pysma-plus-0.1.1/tests/test_sensor.py`

 * *Files identical despite different names*

