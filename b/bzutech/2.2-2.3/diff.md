# Comparing `tmp/bzutech-2.2.tar.gz` & `tmp/bzutech-2.3.tar.gz`

## Comparing `bzutech-2.2.tar` & `bzutech-2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 bzutech-2.2/setup.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 bzutech-2.2/test.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bzutech-2.2/build/lib/bzutech/__init__.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bzutech-2.2/bzutech/__init__.py
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 bzutech-2.2/bzutech/bzutechapi/BzuTechAPI.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 bzutech-2.2/bzutech/bzutechapi/__init__.py
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 bzutech-2.2/bzutech/device/Device.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bzutech-2.2/bzutech/device/__init__.py
--rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 bzutech-2.2/bzutech/sensor/Sensor.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bzutech-2.2/bzutech/sensor/__init__.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 bzutech-2.2/bzutech.egg-info/PKG-INFO
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 bzutech-2.2/bzutech.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 bzutech-2.2/bzutech.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bzutech-2.2/bzutech.egg-info/requires.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bzutech-2.2/bzutech.egg-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bzutech-2.2/tests/main.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 bzutech-2.2/README.md
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 bzutech-2.2/pyproject.toml
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 bzutech-2.2/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 bzutech-2.3/setup.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 bzutech-2.3/test.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bzutech-2.3/build/lib/bzutech/__init__.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech/__init__.py
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech/bzutechapi/BzuTechAPI.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech/bzutechapi/__init__.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech/device/Device.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech/device/__init__.py
+-rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech/sensor/Sensor.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech/sensor/__init__.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech.egg-info/requires.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech.egg-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bzutech-2.3/tests/main.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 bzutech-2.3/README.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 bzutech-2.3/pyproject.toml
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 bzutech-2.3/PKG-INFO
```

### Comparing `bzutech-2.2/bzutech/bzutechapi/BzuTechAPI.py` & `bzutech-2.3/bzutech/bzutechapi/BzuTechAPI.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from aiohttp import ClientSession
-import paho.mqtt.client as mqtt
 import json
 from ..device import Device
 class BzuTech:
     def __init__(self, email: str, password: str) -> None:
         self.email = email
         self.password = password
         self._token = None
@@ -77,18 +76,29 @@
         return list(self.dispositivos.keys())
 
     def get_sensors(self, chipid: str) -> list:
         if chipid in self.get_device_names():
             return list(self.dispositivos[chipid].get_sensor_names())
         return ["-1"]
     
+    def get_sensors_on(self, chipid: str, port: int) -> list:
+        if chipid in self.get_device_names():
+            list = self.dispositivos[chipid].get_sensor_names_on(port)
+            return list
+        return ["-1"]
+    
+    def get_endpoint_on(self, chipid: str, port: int) -> str:
+        if(chipid in self.get_device_names()):
+            return self.dispositivos[chipid].get_ep_on(port)
+        return "-1"
+
+    
     def get_reading(self, chipid: str, sensorname:str):
         return self.dispositivos[chipid].get_readings(sensorname.upper())
 
-
     async def send_reading(self, sensoref:str, DeviceID: str, reading: float, date: str):
         url = "https://back-dev.bzutech.com.br/logs/home_assistence/"
         data = '{"bci":"'+DeviceID+'", "date":"'+ date +'", "data":\"[{\'ref\':\''+ sensoref +'\',\'med\':'+ str(reading) +'}]\"}'
         data = json.loads(data)
         client = ClientSession()
         async with client.post(url, json=data, headers = self.httpheaders) as resp:
             await client.close()
```

### Comparing `bzutech-2.2/bzutech/device/Device.py` & `bzutech-2.3/bzutech/device/Device.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,13 +45,28 @@
 
     def get_sensor_names_on(self, port: str):
         sensores = []
         for sensor in self.get_sensor_names():
             if sensor[-1] == port:
                 sensores.append(sensor)
         return sensores
+    
+    def get_ep_on(self, port:int):
+        sensors = self.get_sensor_names_on(str(port))
+        for sensor in sensors:
+            if "ADS7878" in sensor:
+                return "EP400"
+            if "RTZSBZ" in sensor:
+                return "EP300"
+            if "SGP30" in sensor:
+                return "EP200"
+            if "DOOR" in sensor:
+                return "EP121"
+            if "SHT30" in sensor:
+                return "EP111"
+        
 
     async def get_readings(self, nome_sensor):
         return await self.sensores[nome_sensor].get_leitura()
 
     def get_chipid(self):
         return self.chipid
```

### Comparing `bzutech-2.2/bzutech/sensor/Sensor.py` & `bzutech-2.3/bzutech/sensor/Sensor.py`

 * *Files identical despite different names*

### Comparing `bzutech-2.2/bzutech.egg-info/PKG-INFO` & `bzutech-2.3/bzutech.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `bzutech-2.2/pyproject.toml` & `bzutech-2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["bzutech"]
 
 [project]
 name = "bzutech"
-version = "2.2"
+version = "2.3"
 dependencies = [
     "aiohttp",
     "paho-mqtt"
 ]  
 authors = [
   { name="Ênio Ferreira", email="e.nioferreira@hotmail.com" },
 ]
```

### Comparing `bzutech-2.2/PKG-INFO` & `bzutech-2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bzutech
-Version: 2.2
+Version: 2.3
 Summary: Integration package for bzutech services
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Author-email: Ênio Ferreira <e.nioferreira@hotmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

