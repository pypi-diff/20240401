# Comparing `tmp/openrgb-python-0.2.9.tar.gz` & `tmp/openrgb-python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openrgb-python-0.2.9.tar", last modified: Thu Jun 24 20:45:57 2021, max compression
+gzip compressed data, was "dist/openrgb-python-0.3.0.tar", last modified: Mon Apr  1 10:40:50 2024, max compression
```

## Comparing `openrgb-python-0.2.9.tar` & `openrgb-python-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 20:45:57.000000 openrgb-python-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)     3078 2021-06-24 20:45:57.000000 openrgb-python-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2056 2021-06-24 20:45:52.000000 openrgb-python-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 20:45:57.000000 openrgb-python-0.2.9/openrgb/
--rwxr-xr-x   0 runner    (1001) docker     (121)      127 2021-06-24 20:45:52.000000 openrgb-python-0.2.9/openrgb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9097 2021-06-24 20:45:52.000000 openrgb-python-0.2.9/openrgb/network.py
--rw-r--r--   0 runner    (1001) docker     (121)    20561 2021-06-24 20:45:52.000000 openrgb-python-0.2.9/openrgb/orgb.py
--rw-r--r--   0 runner    (1001) docker     (121)    20318 2021-06-24 20:45:52.000000 openrgb-python-0.2.9/openrgb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 20:45:57.000000 openrgb-python-0.2.9/openrgb_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3078 2021-06-24 20:45:57.000000 openrgb-python-0.2.9/openrgb_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      242 2021-06-24 20:45:57.000000 openrgb-python-0.2.9/openrgb_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-24 20:45:57.000000 openrgb-python-0.2.9/openrgb_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-06-24 20:45:57.000000 openrgb-python-0.2.9/openrgb_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-24 20:45:57.000000 openrgb-python-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      636 2021-06-24 20:45:52.000000 openrgb-python-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:40:50.000000 openrgb-python-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-01 10:40:50.000000 openrgb-python-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-01 10:40:44.000000 openrgb-python-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:40:50.000000 openrgb-python-0.3.0/openrgb/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      127 2024-04-01 10:40:44.000000 openrgb-python-0.3.0/openrgb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12913 2024-04-01 10:40:44.000000 openrgb-python-0.3.0/openrgb/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25466 2024-04-01 10:40:44.000000 openrgb-python-0.3.0/openrgb/orgb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:40:50.000000 openrgb-python-0.3.0/openrgb/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-01 10:40:44.000000 openrgb-python-0.3.0/openrgb/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-01 10:40:44.000000 openrgb-python-0.3.0/openrgb/plugins/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-01 10:40:44.000000 openrgb-python-0.3.0/openrgb/plugins/effects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23896 2024-04-01 10:40:44.000000 openrgb-python-0.3.0/openrgb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:40:50.000000 openrgb-python-0.3.0/openrgb_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-01 10:40:50.000000 openrgb-python-0.3.0/openrgb_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-01 10:40:50.000000 openrgb-python-0.3.0/openrgb_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 10:40:50.000000 openrgb-python-0.3.0/openrgb_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 10:40:50.000000 openrgb-python-0.3.0/openrgb_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 10:40:50.000000 openrgb-python-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-01 10:40:44.000000 openrgb-python-0.3.0/setup.py
```

### Comparing `openrgb-python-0.2.9/PKG-INFO` & `openrgb-python-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrgb-python
-Version: 0.2.9
+Version: 0.3.0
 Summary: A python client for the OpenRGB SDK
 Home-page: https://github.com/jath03/openrgb-python
 Author: jath03
 License: UNKNOWN
 Description: # OpenRGB-Python
         
         
@@ -42,16 +42,17 @@
         Arch Linux:
         `yay -S python-openrgb-git`
         
         For a more stable package:
         
         `pip3 install openrgb-python`
         
-        Arch Linux:
-        `yay -S python-openrgb`
+        ~~Arch Linux:
+        `yay -S python-openrgb`~~
+        This AUR package is out of date. Use `python-openrgb-git` instead.
         
         Thanks to @GabMus for the AUR packages
         
         # Usage
         
         ```python
         from openrgb import OpenRGBClient
```

### Comparing `openrgb-python-0.2.9/README.md` & `openrgb-python-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,17 @@
 Arch Linux:
 `yay -S python-openrgb-git`
 
 For a more stable package:
 
 `pip3 install openrgb-python`
 
-Arch Linux:
-`yay -S python-openrgb`
+~~Arch Linux:
+`yay -S python-openrgb`~~
+This AUR package is out of date. Use `python-openrgb-git` instead.
 
 Thanks to @GabMus for the AUR packages
 
 # Usage
 
 ```python
 from openrgb import OpenRGBClient
```

### Comparing `openrgb-python-0.2.9/openrgb/network.py` & `openrgb-python-0.3.0/openrgb/network.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 import platform
 import socket
 import struct
 import threading
 from openrgb import utils
-from typing import Callable
+from typing import Callable, Optional
 
-OPENRGB_PROTOCOL_VERSION = 2
+OPENRGB_PROTOCOL_VERSION = 4
 
 if platform.system() == "Linux":
-    NOSIGNAL = socket.MSG_NOSIGNAL
+    NOSIGNAL: int = socket.MSG_NOSIGNAL
 else:
     NOSIGNAL = 0
 
 
 class NetworkClient:
     '''
     A class for interfacing with the OpenRGB SDK
     '''
 
-    def __init__(self, update_callback: Callable, address: str = "127.0.0.1", port: int = 6742, name: str = "openrgb-python", protocol_version: int = None):
+    def __init__(self, update_callback: Callable, address: str = "127.0.0.1", port: int = 6742, name: str = "openrgb-python", protocol_version: Optional[int] = None):
         '''
         :param update_callback: the function to call when data is received
         :param address: the ip address of the SDK server
         :param port: the port of the SDK server
         :param name: the string that will be displayed on the OpenRGB SDK tab's list of clients
         '''
         self.lock = threading.Lock()
@@ -74,99 +74,137 @@
         '''
         Closes the active socket
         '''
         try:
             self.lock.release()
         except Exception:
             pass
-        
+
         if self.sock is not None:
             self.sock.close()
             self.sock = None
 
     def read(self):
         '''
         Reads responses from the SDK
 
-        :raises OpenRGBDisconnected: when it loses connection to the SDK
+        :raises utils.OpenRGBDisconnected: when it loses connection to the SDK
         '''
-        if self.sock is None:
+        if not self.connected:
             raise utils.OpenRGBDisconnected()
         header = bytearray(utils.HEADER_SIZE)
         try:
             self.sock.recv_into(header)
         except utils.CONNECTION_ERRORS as e:
             self.stop_connection()
             raise utils.OpenRGBDisconnected() from e
 
         if header == '\x00'*utils.HEADER_SIZE:
             self.stop_connection()
             raise utils.OpenRGBDisconnected()
         # Unpacking the contents of the raw header struct into a list
         buff = list(struct.unpack('ccccIII', header))
-        # print(buff[:4])
+
+        # Checking packet signature
         if buff[:4] == [b'O', b'R', b'G', b'B']:
             device_id, packet_type, packet_size = buff[4:]
-            # print(device_id, packet_type, packet_size)
+
+            # Parse information from each packet type
             if packet_type == utils.PacketType.REQUEST_CONTROLLER_COUNT:
                 try:
                     buff = struct.unpack("I", self.sock.recv(packet_size))
                     self.lock.release()
                     self.callback(device_id, packet_type, buff[0])
                 except utils.CONNECTION_ERRORS as e:
                     self.stop_connection()
                     raise utils.OpenRGBDisconnected() from e
                 finally:
                     try:
                         self.lock.release()
                     except RuntimeError:
                         pass
+
             elif packet_type == utils.PacketType.REQUEST_CONTROLLER_DATA:
                 try:
-                    data =  bytearray()
+                    data = bytes()
                     while len(data) < packet_size:
                         data += self.sock.recv(packet_size - len(data))
                 except utils.CONNECTION_ERRORS as e:
                     self.stop_connection()
                     raise utils.OpenRGBDisconnected() from e
                 finally:
                     self.lock.release()
-                self.callback(device_id, packet_type, utils.ControllerData.unpack(data, self._protocol_version))
+                try:
+                    self.callback(device_id, packet_type, utils.ControllerData.unpack(data, self._protocol_version))
+                except utils.PARSING_ERRORS as e:
+                    raise utils.ControllerParsingError(f"Unable to parse data from request `{packet_type}` for device #{device_id}") from e
+
             elif packet_type == utils.PacketType.DEVICE_LIST_UPDATED:
                 assert device_id == 0 and packet_size == 0
                 self.read()
                 self.callback(device_id, packet_type, 0)
+
             elif packet_type == utils.PacketType.REQUEST_PROTOCOL_VERSION:
                 try:
                     self.max_protocol_version = min(struct.unpack("I", self.sock.recv(packet_size))[0], OPENRGB_PROTOCOL_VERSION)
                     self._protocol_version = min(self.max_protocol_version, self._protocol_version)
                 except utils.CONNECTION_ERRORS as e:
                     self.stop_connection()
                     raise utils.OpenRGBDisconnected() from e
                 finally:
                     self.lock.release()
+
             elif packet_type == utils.PacketType.REQUEST_PROFILE_LIST:
                 try:
-                    data =  bytearray()
+                    data = bytes()
+                    while len(data) < packet_size:
+                        data += self.sock.recv(packet_size - len(data))
+                    idata = iter(data)
+                    for _ in range(4):
+                        next(idata)
+                except utils.CONNECTION_ERRORS as e:
+                    self.stop_connection()
+                    raise utils.OpenRGBDisconnected() from e
+                finally:
+                    self.lock.release()
+                self.callback(device_id, packet_type, utils.parse_list(utils.Profile, idata, self._protocol_version))
+            elif packet_type == utils.PacketType.REQUEST_PLUGIN_LIST:
+                try:
+                    data = bytes()
                     while len(data) < packet_size:
                         data += self.sock.recv(packet_size - len(data))
+                    idata = iter(data)
+                    for _ in range(4):
+                        next(idata)
                 except utils.CONNECTION_ERRORS as e:
                     self.stop_connection()
                     raise utils.OpenRGBDisconnected() from e
                 finally:
                     self.lock.release()
-                self.callback(device_id, packet_type, utils.parse_list(utils.Profile, data, self._protocol_version, 4)[1])
+                self.callback(device_id, packet_type, utils.parse_list(utils.Plugin, idata, self._protocol_version))
+            elif packet_type == utils.PacketType.PLUGIN_SPECIFIC:
+                try:
+                    data = bytes()
+                    while len(data) < packet_size:
+                        data += self.sock.recv(packet_size - len(data))
+                    idata = iter(data)
+                except utils.CONNECTION_ERRORS as e:
+                    self.stop_connection()
+                    raise utils.OpenRGBDisconnected() from e
+                finally:
+                    self.lock.release()
+                self.callback(device_id, packet_type, idata)
 
     def requestDeviceData(self, device: int):
         '''
         Sends the request for a device's data
 
         :param device: the id of the device to request data for
         '''
-        if self.sock is None:
+        if not self.connected:
             raise utils.OpenRGBDisconnected()
         self.send_header(device, utils.PacketType.REQUEST_CONTROLLER_DATA, struct.calcsize('I'))
         self.send_data(struct.pack("I", self._protocol_version), False)
         self.read()
 
     def requestDeviceNum(self):
         '''
@@ -178,54 +216,89 @@
     def requestProfileList(self):
         '''
         Sends the request for the available profiles
         '''
         self.send_header(0, utils.PacketType.REQUEST_PROFILE_LIST, 0)
         self.read()
 
-    def send_header(self, device_id: int, packet_type: int, packet_size: int):
+    def requestPluginList(self):
+        '''
+        Sends the request for the available plugins
+        '''
+        self.send_header(0, utils.PacketType.REQUEST_PLUGIN_LIST, 0)
+        self.read()
+
+    def send_header(self, device_id: int, packet_type: utils.PacketType, packet_size: int, release_lock: bool = True):
         '''
         Sends a header to the SDK
 
         :param device_id: The id of the device to send a header for
         :param packet_type: A utils.PacketType
         :param packet_size: The full size of the data to be sent after the header
         '''
-        if self.sock is None:
+        self.check_version(packet_type)
+        if not self.connected:
             raise utils.OpenRGBDisconnected()
 
         if not self.lock.acquire(timeout=10):
             raise utils.OpenRGBDisconnected("SDK server did not respond to previous request")
 
         try:
             data = struct.pack('ccccIII', b'O', b'R', b'G', b'B', device_id, packet_type, packet_size)
-            sent = self.sock.send(data, NOSIGNAL)
+            sent = self.sock.send(data, NOSIGNAL)  # type: ignore
             if sent != len(data):
                 self.stop_connection()
                 raise utils.OpenRGBDisconnected()
-            if packet_size == 0 and packet_type not in (utils.PacketType.REQUEST_CONTROLLER_COUNT,\
-                                                  utils.PacketType.REQUEST_CONTROLLER_DATA,\
-                                                  utils.PacketType.REQUEST_PROTOCOL_VERSION,\
-                                                  utils.PacketType.REQUEST_PROFILE_LIST):
+            if release_lock and packet_size == 0 and packet_type not in (utils.PacketType.REQUEST_CONTROLLER_COUNT,
+                                                                         utils.PacketType.REQUEST_CONTROLLER_DATA,
+                                                                         utils.PacketType.REQUEST_PROTOCOL_VERSION,
+                                                                         utils.PacketType.REQUEST_PROFILE_LIST,
+                                                                         utils.PacketType.REQUEST_PLUGIN_LIST,
+                                                                         utils.PacketType.PLUGIN_SPECIFIC):
                 self.lock.release()
         except utils.CONNECTION_ERRORS as e:
             self.stop_connection()
             raise utils.OpenRGBDisconnected() from e
 
     def send_data(self, data: bytes, release_lock: bool = True):
         '''
         Sends data to the SDK
 
         :param data: The data to send
         '''
-        if self.sock is None:
+        if not self.connected:
             raise utils.OpenRGBDisconnected()
         try:
-            sent = self.sock.send(data, NOSIGNAL)
+            sent = self.sock.send(data, NOSIGNAL)  # type: ignore
             if sent != len(data):
                 self.stop_connection()
                 raise utils.OpenRGBDisconnected()
             if release_lock:
                 self.lock.release()
         except utils.CONNECTION_ERRORS as e:
             self.stop_connection()
             raise utils.OpenRGBDisconnected() from e
+
+    def check_version(self, packet_type: utils.PacketType):
+        '''
+        Verifies that the packet type is supported on the version we are using.
+
+        :param packet_type: What kind of packet is going to be sent
+        :raises utils.SDKVersionError: When a packet is unsupported
+        '''
+        if self._protocol_version < 2 and packet_type in (utils.PacketType.REQUEST_PROFILE_LIST,
+                                                          utils.PacketType.REQUEST_SAVE_PROFILE,
+                                                          utils.PacketType.REQUEST_LOAD_PROFILE,
+                                                          utils.PacketType.REQUEST_DELETE_PROFILE):
+            raise utils.SDKVersionError("Profile controls not supported on protocol versions < 2.  You probably need to update OpenRGB")
+        elif self._protocol_version < 3 and packet_type == utils.PacketType.RGBCONTROLLER_SAVEMODE:
+            raise utils.SDKVersionError("Saving modes not supported on protocol versions < 3.  You probably need to update OpenRGB")
+        elif self._protocol_version < 4 and packet_type in (utils.PacketType.REQUEST_PLUGIN_LIST,
+                                                            utils.PacketType.PLUGIN_SPECIFIC):
+            raise utils.SDKVersionError("Plugin controls not supported on protocol versions < 4.  You probably need to update OpenRGB")
+
+    @property
+    def connected(self) -> bool:
+        '''
+        Returns whether the current instance is currently connected to a server
+        '''
+        return self.sock is not None
```

### Comparing `openrgb-python-0.2.9/openrgb/orgb.py` & `openrgb-python-0.3.0/openrgb/orgb.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 import struct
 import platform
 from openrgb import utils
-from typing import Union, Optional
+from typing import Union, Any, Optional
 from openrgb.network import NetworkClient
-# from dataclasses import dataclass
+from openrgb.plugins import create_plugin, ORGBPlugin
 from time import sleep
 from os import environ
 
 
 class LED(utils.RGBObject):
     '''
     A class to represent individual LEDs
@@ -39,83 +39,115 @@
         )
         buff = struct.pack("i", self.id) + color.pack()
         self.comms.send_data(buff)
         if not fast:
             self.update()
 
 
+class Segment(utils.RGBContainer):
+    '''
+    A class to represent a segment
+    '''
+
+    def __init__(self, data: utils.SegmentData, id: int, parent: Zone):
+        self.leds = [None for _ in range(data.leds_count)]
+        self.id = id
+        self.parent_zone = parent
+        self._update(data)
+
+    def _update(self, data: utils.SegmentData):
+        self.name = data.name
+        self.type = data.segment_type
+        self.start_idx = data.start_idx
+        self.leds_count = data.leds_count
+        self.leds = self.parent_zone.leds[data.start_idx:data.start_idx + data.leds_count]
+
+    def set_color(self, color: utils.RGBColor, fast: bool = False):
+        self.set_colors([color] * self.leds_count, fast)
+
+    def set_colors(self, colors: list[utils.RGBColor], fast: bool = False):
+        new_colors = self.parent_zone.colors[:self.start_idx] + colors + self.parent_zone.colors[self.start_idx + self.leds_count:]
+        self.parent_zone.set_colors(new_colors, fast)
+
+
 class Zone(utils.RGBContainer):
     '''
     A class to represent a zone
     '''
 
     def __init__(self, data: utils.ZoneData, zone_id: int, device_id: int, network_client: NetworkClient):
         self.leds = [None for led in data.leds]
+        try:
+            self.segments: Optional[list[Segment]] = [None for _ in data.segments]  # type: ignore
+        except TypeError:
+            self.segments = None
         self.device_id = device_id
         self.comms = network_client
         self.id = zone_id
         self._update(data)
 
     def _update(self, data: utils.ZoneData):
         self.name = data.name
         self.type = data.zone_type
         if len(self.leds) != len(data.leds):
             self.leds = [None for led in data.leds]
         for x in range(len(data.leds)):
             if self.leds[x] is None:
-                self.leds[x] = LED(data.leds[x], data.colors[x], x, self.device_id, self.comms)
+                self.leds[x] = LED(data.leds[x], data.colors[x],
+                                   data.start_idx + x, self.device_id, self.comms)
             else:
                 self.leds[x]._update(data.leds[x], data.colors[x])
+        if self.segments:
+            for x in range(len(data.segments)):  # type: ignore
+                if self.segments[x] is None:
+                    self.segments[x] = Segment(data.segments[x], x, self)  # type: ignore
+                else:
+                    self.segments[x]._update(data.segments[x])  # type: ignore
         self.mat_width = data.mat_width
         self.mat_height = data.mat_height
         self.matrix_map = data.matrix_map
         self.colors = data.colors
         self._colors = self.colors[:]
 
-    def set_color(self, color: utils.RGBColor, start: int = 0, end: int = 0, fast: bool = False):
+    def set_color(self, color: utils.RGBColor, fast: bool = False):
         '''
-        Sets the LEDs' color in the zone between start and end
+        Sets the zone's color
 
         :param color: the color to set the LEDs to
-        :param start: the first LED to change
-        :param end: the first unchanged LED
         :param fast: If you care more about quickly setting colors than having correct internal state data, then set :code:`fast` to :code:`True`
         '''
-        if end == 0:
-            end = len(self.leds)
         self.comms.send_header(
             self.device_id,
             utils.PacketType.RGBCONTROLLER_UPDATEZONELEDS,
-            struct.calcsize(f"IiH{3*(end)}b{(end)}x")
+            struct.calcsize(f"iIH{3*(len(self.leds))}b{len(self.leds)}x")
         )
-        buff = struct.pack("iH", self.id, end) + b''.join((color.pack() for color in self._colors[:start])) + (color.pack())*(end - start)
+        buff = struct.pack("iH", self.id, len(self.leds)) + \
+            (color.pack())*len(self.leds)
         buff = struct.pack("I", len(buff)) + buff
         self.comms.send_data(buff)
         if not fast:
             self.update()
 
-    def set_colors(self, colors: list[utils.RGBColor], start: int = 0, end: int = 0, fast: bool = False):
+    def set_colors(self, colors: list[utils.RGBColor], fast: bool = False):
         '''
-        Sets the LEDs' colors in the zone between start and end
+        Sets the LEDs' colors in the zone
 
         :param colors: the list of colors, one per LED
-        :param start: the first LED to change
-        :param end: the first unchanged LED
         :param fast: If you care more about quickly setting colors than having correct internal state data, then set :code:`fast` to :code:`True`
         '''
-        if end == 0:
-            end = len(self.leds)
-        if len(colors) != (end - start):
-            raise IndexError("Number of colors doesn't match number of LEDs")
+        if len(colors) != len(self.leds):
+            raise IndexError(
+                "Number of colors doesn't match number of LEDs in the zone")
         self.comms.send_header(
             self.device_id,
             utils.PacketType.RGBCONTROLLER_UPDATEZONELEDS,
-            struct.calcsize(f"IIH{3*(end)}b{(end)}x")
+            struct.calcsize(f"iIH{3*(len(self.leds))}b{len(self.leds)}x")
         )
-        buff = struct.pack("IH", self.id, end) + b''.join((color.pack() for color in self._colors[:start])) + b''.join((color.pack() for color in colors))
+        buff = struct.pack("iH", self.id, len(self.leds)) + \
+            b''.join((color.pack() for color in colors))
         buff = struct.pack("I", len(buff)) + buff
         self.comms.send_data(buff)
         if not fast:
             self.update()
 
     def resize(self, size: int):
         '''
@@ -134,170 +166,259 @@
 
 class Device(utils.RGBContainer):
     '''
     A class to represent an RGB Device
     '''
 
     def __init__(self, data: utils.ControllerData, device_id: int, network_client: NetworkClient):
-        self.leds = [None for i in data.leds]
-        self.zones = [None for i in data.zones]
+        self.leds: list[LED] = [None for i in data.leds]  # type: ignore
+        self.zones: list[Zone] = [None for i in data.zones]  # type: ignore
         self.id = device_id
         self.device_id = device_id
         self.comms = network_client
         self._update(data)
 
     def _update(self, data: utils.ControllerData):
         self.name = data.name
         self.metadata = data.metadata
         self.type = data.device_type
         if len(self.leds) != len(data.leds):
-            self.leds = [None for i in data.leds]
+            self.leds = [None for i in data.leds]  # type: ignore
         for x in range(len(data.leds)):
             if self.leds[x] is None:
-                self.leds[x] = LED(data.leds[x], data.colors[x], x, self.device_id, self.comms)
+                self.leds[x] = LED(data.leds[x], data.colors[x],
+                                   x, self.device_id, self.comms)
             else:
                 self.leds[x]._update(data.leds[x], data.colors[x])
         for x in range(len(data.zones)):
             if self.zones[x] is None:
-                self.zones[x] = Zone(data.zones[x], x, self.device_id, self.comms)
+                self.zones[x] = Zone(
+                    data.zones[x], x, self.device_id, self.comms)
             else:
-                self.zones[x]._update(data.zones[x])
+                self.zones[x]._update(data.zones[x])  # type: ignore
         self.modes = data.modes
         self.colors = data.colors
         self._colors = self.colors[:]
         self.active_mode = data.active_mode
         self.data = data
 
-    def set_color(self, color: utils.RGBColor, start: int = 0, end: int = 0, fast: bool = False):
+    def _set_device_color(self, color: utils.RGBColor, fast: bool = False):
         '''
-        Sets the LEDs' color between start and end
+        Sets the device's color
 
         :param color: the color to set the LED(s) to
-        :param start: the first LED to change
-        :param end: the first unchanged LED
         :param fast: If you care more about quickly setting colors than having correct internal state data, then set :code:`fast` to :code:`True`
         '''
-        if end == 0:
-            end = len(self.leds)
         self.comms.send_header(
             self.id,
             utils.PacketType.RGBCONTROLLER_UPDATELEDS,
-            struct.calcsize(f"IH{3*(end)}b{(end)}x")
+            struct.calcsize(f"IH{3*(len(self.leds))}b{len(self.leds)}x")
         )
-        buff = struct.pack("H", end) + b''.join((color.pack() for color in self._colors[:start])) + (color.pack())*(end - start)
+        buff = struct.pack("H", len(self.leds)) + (color.pack())*len(self.leds)
         buff = struct.pack("I", len(buff)) + buff
         self.comms.send_data(buff)
         if not fast:
             self.update()
 
-    def set_colors(self, colors: list[utils.RGBColor], start: int = 0, end: int = 0, fast: bool = False):
+    def _set_device_colors(self, colors: list[utils.RGBColor], fast: bool = False):
         '''
-        Sets the LEDs' colors between start and end
+        Sets the devices LEDs' colors
 
         :param colors: the list of colors, one per LED
-        :param start: the first LED to change
-        :param end: the first unchanged LED
         :param fast: If you care more about quickly setting colors than having correct internal state data, then set :code:`fast` to :code:`True`
         '''
-        if end == 0:
-            end = len(self.leds)
-        if len(colors) != (end - start):
+        if len(colors) != len(self.leds):
             raise IndexError("Number of colors doesn't match number of LEDs")
         self.comms.send_header(
             self.id,
             utils.PacketType.RGBCONTROLLER_UPDATELEDS,
-            struct.calcsize(f"IH{3*(end)}b{(end)}x")
+            struct.calcsize(f"IH{3*(len(self.leds))}b{len(self.leds)}x")
         )
-        buff = struct.pack("H", end) + b''.join((color.pack() for color in self._colors[:start])) + b''.join((color.pack() for color in colors))
+        buff = struct.pack("H", len(self.leds)) + \
+            b''.join((color.pack() for color in colors))
         buff = struct.pack("I", len(buff)) + buff
         self.comms.send_data(buff)
         if not fast:
             self.update()
 
-    def set_mode(self, mode: Union[int, str, utils.ModeData]):
+    def _set_mode_color(self, color: utils.RGBColor):
+        '''
+        Sets the mode-specific color, if possible
+
+        :param color: the color to set the LED(s) to
+        '''
+        active_mode = self.modes[self.active_mode]
+        assert active_mode.color_mode == utils.ModeColors.MODE_SPECIFIC
+        assert active_mode.colors is not None
+        active_mode.colors = [color]*active_mode.colors_max  # type: ignore
+        self.set_mode(active_mode)
+
+    def _set_mode_colors(self, colors: list[utils.RGBColor]):
+        '''
+        Sets the mode-specific color, if possible
+
+        :param color: the color to set the LED(s) to
+        '''
+        active_mode = self.modes[self.active_mode]
+        assert active_mode.color_mode == utils.ModeColors.MODE_SPECIFIC
+        assert active_mode.colors is not None
+        assert active_mode.colors_min <= len(  # type: ignore
+            colors) <= active_mode.colors_max
+        active_mode.colors = colors
+        self.set_mode(active_mode)
+
+    def set_color(self, color: utils.RGBColor, fast: bool = False):
+        '''
+        Sets the color of the device whether the current mode is per-led or
+        mode-specific
+
+        :param colors: the list of colors, one per LED
+        :param fast: If you care more about quickly setting colors than having correct internal state data, then set :code:`fast` to :code:`True` (only applies when not setting a mode-specific color)
+        '''
+        active_mode = self.modes[self.active_mode]
+        if active_mode.color_mode == utils.ModeColors.MODE_SPECIFIC:
+            self._set_mode_color(color)
+        elif active_mode.color_mode == utils.ModeColors.PER_LED:
+            self._set_device_color(color, fast)
+
+    def set_colors(self, colors: list[utils.RGBColor], fast: bool = False):
+        '''
+        Sets the colors of the device whether the current mode is per-led or
+        mode-specific
+
+        :param colors: the list of colors, one per LED or per mode-specific color
+        :param fast: If you care more about quickly setting colors than having correct internal state data, then set :code:`fast` to :code:`True` (only applies when not setting a mode-specific color)
+        '''
+        active_mode = self.modes[self.active_mode]
+        if active_mode.color_mode == utils.ModeColors.MODE_SPECIFIC:
+            self._set_mode_colors(colors)
+        elif active_mode.color_mode == utils.ModeColors.PER_LED:
+            self._set_device_colors(colors, fast)
+
+    def set_mode(self, mode: Union[int, str, utils.ModeData], save: bool = False):
         '''
         Sets the device's mode
 
         :param mode: the id, name, or the ModeData object itself to set as the mode
         '''
         if type(mode) == utils.ModeData:
             pass
         elif type(mode) == int:
             mode = self.modes[mode]
         elif type(mode) == str:
             try:
-                mode = next((m for m in self.modes if m.name.lower() == mode.lower()))
+                mode = next(
+                    (m for m in self.modes if m.name.lower() == mode.lower()))
             except StopIteration as e:
-                raise ValueError(f"Mode `{mode}` not found for device `{self.name}`") from e
-        data = mode.pack(self.comms._protocol_version)
+                raise ValueError(
+                    f"Mode `{mode}` not found for device `{self.name}`") from e
+        data = mode.pack(self.comms._protocol_version)  # type: ignore
         self.comms.send_header(
             self.id,
             utils.PacketType.RGBCONTROLLER_UPDATEMODE,
             len(data)
         )
         self.comms.send_data(data)
+        if save:
+            self.comms.send_header(
+                self.id,
+                utils.PacketType.RGBCONTROLLER_SAVEMODE,
+                len(data)
+            )
+            self.comms.send_data(data)
         self.update()
 
     def set_custom_mode(self):
+        '''
+        Sets the mode to whatever the device supports that provides the most
+        granular control
+        '''
         self.comms.send_header(
             self.id,
             utils.PacketType.RGBCONTROLLER_SETCUSTOMMODE,
             0
         )
+        self.update()
+        self.set_mode(self.active_mode)
+
+    def save_mode(self):
+        '''
+        Saves the currently selected mode
+        '''
+        data = self.modes[self.active_mode].pack(self.comms._protocol_version)
+        self.comms.send_header(
+            self.id,
+            utils.PacketType.RGBCONTROLLER_SAVEMODE,
+            len(data)
+        )
+        self.comms.send_data(data)
+
+    def off(self):
+        '''
+        Turns off device by setting the custom mode and then calling :any:`RGBObject.clear`
+        '''
+        self.set_custom_mode()
+        self.clear()
 
 
 class OpenRGBClient(utils.RGBObject):
     '''
     This is the only class you should need to manually instantiate.  It
     initializes the communication, gets the device information, and creates
     Devices, Zones, and LEDs for you.
     '''
 
-    def __init__(self, address: str = "127.0.0.1", port: int = 6742, name: str = "openrgb-python", protocol_version: int = None):
+    def __init__(self, address: str = "127.0.0.1", port: int = 6742, name: str = "openrgb-python", protocol_version: Optional[int] = None):
         '''
         :param address: the ip address of the SDK server
         :param port: the port of the SDK server
         :param name: the string that will be displayed on the OpenRGB SDK tab's list of clients
+        :param protocol_version: which protocol version to use
         '''
         self.device_num = 0
-        self.devices = []
-        self.profiles = []
-        self.comms = NetworkClient(self._callback, address, port, name, protocol_version)
+        self.devices: list[Device] = []
+        self.profiles: list[utils.Profile] = []
+        self.plugins: list[ORGBPlugin] = []
+        self.comms = NetworkClient(
+            self._callback, address, port, name, protocol_version)
         self.address = address
         self.port = port
         self.name = name
-        self.comms.requestDeviceNum()
-        while any((dev is None for dev in self.devices)):
-            sleep(.1)
-        if self.comms._protocol_version >= 2:
-            self.update_profiles()
+        self.update()
 
     def __repr__(self):
         return f"OpenRGBClient(address={self.address}, port={self.port}, name={self.name})"
 
-    def _callback(self, device: int, type: int, data: Optional):
+    def _callback(self, device: int, type: int, data: Any):
         if type == utils.PacketType.REQUEST_CONTROLLER_COUNT:
             if data != self.device_num or data != len(self.devices):
                 self.device_num = data
-                self.devices = [None for x in range(self.device_num)]
+                self.devices = [None for x in range(  # type: ignore
+                    self.device_num)]  
                 for x in range(self.device_num):
                     self.comms.requestDeviceData(x)
         elif type == utils.PacketType.REQUEST_CONTROLLER_DATA:
             try:
                 if self.devices[device] is None:
                     self.devices[device] = Device(data, device, self.comms)
                 else:
-                    self.devices[device]._update(data)
+                    self.devices[device]._update(data)  # type: ignore
             except IndexError:
                 self.comms.requestDeviceNum()
         elif type == utils.PacketType.DEVICE_LIST_UPDATED:
             self.device_num = 0
             self.comms.requestDeviceNum()
         elif type == utils.PacketType.REQUEST_PROFILE_LIST:
             self.profiles = data
+        elif type == utils.PacketType.REQUEST_PLUGIN_LIST:
+            for plugin in data:
+                if (all(plugin.id != existing.id for existing in self.plugins)):
+                    self.plugins.append(create_plugin(plugin, self.comms))
+        elif type == utils.PacketType.PLUGIN_SPECIFIC:
+            next(plugin for plugin in self.plugins if plugin.id == device)._recv(data)
 
     def set_color(self, color: utils.RGBColor, fast: bool = False):
         '''
         Sets the color of every device.
 
         :param color: the color to set the devices to
         :param fast: If you care more about quickly setting colors than having correct internal state data, then set :code:`fast` to :code:`True`
@@ -332,15 +453,16 @@
         :param local: Whether to load a local file or a profile from the server.
         :param directory: what directory the profile is in.  Defaults to OpenRGB's config directory for supported OS's (Windows or Linux), or falls back to using the current working directory.
         '''
         if local:
             assert type(name) is str
             if directory == '':
                 if platform.system() == "Linux":
-                    directory = environ['HOME'].rstrip("/") + "/.config/OpenRGB"
+                    directory = environ['HOME'].rstrip(
+                        "/") + "/.config/OpenRGB"
                 elif platform.system() == "Windows":
                     directory = environ['APPDATA'].rstrip("\\") + "\\OpenRGB"
                 else:
                     directory = '.'
             with open(f'{directory}/{name}.orp', 'rb') as f:
                 controllers = utils.LocalProfile.unpack(f).controllers
                 pairs = []
@@ -356,106 +478,119 @@
                     # print(device.name, new_controller.name)
                     if new_controller.colors != device.colors:
                         device.set_colors(new_controller.colors)
                     # print(new_controller.active_mode)
                     if new_controller.active_mode != device.active_mode:
                         device.set_mode(new_controller.active_mode)
         else:
-            if self.comms._protocol_version < 2:
-                raise utils.SDKVersionError("Your version of OpenRGB doesn't support SDK profile controls")
             if type(name) is str:
                 try:
-                    name = next(p for p in self.profiles if p.name.lower() == name.lower())
+                    name = next(
+                        p for p in self.profiles if p.name.lower() == name.lower())
                 except StopIteration as e:
-                    raise ValueError(f"`{name}` is not an existing profile") from e
+                    raise ValueError(
+                        f"`{name}` is not an existing profile") from e
             elif type(name) is int:
                 name = self.profiles[name]
             elif type(name) is utils.Profile:
                 pass
-            name = name.pack()
-            self.comms.send_header(0, utils.PacketType.REQUEST_LOAD_PROFILE, len(name))
-            self.comms.send_data(name)
+            raw_name = name.pack()  # type: ignore
+            self.comms.send_header(
+                0, utils.PacketType.REQUEST_LOAD_PROFILE, len(raw_name))
+            self.comms.send_data(raw_name)
 
     def save_profile(self, name: Union[str, int, utils.Profile], local: bool = False, directory: str = ''):
         '''
         Saves the current state of all of your devices to a new or existing
         OpenRGB profile
 
         :param name: Can be a profile's name, index, or even the Profile itself
         :param local: Whether to load a local file or a profile on the server.
         :param directory: what directory to save the profile in.  Defaults to OpenRGB's config directory for supported OS's (Windows or Linux), or falls back to using the current working directory.
         '''
         if local:
             self.update()
             if directory == '':
                 if platform.system() == "Linux":
-                    directory = environ['HOME'].rstrip("/") + "/.config/OpenRGB"
+                    directory = environ['HOME'].rstrip(
+                        "/") + "/.config/OpenRGB"
                 elif platform.system() == "Windows":
                     directory = environ['APPDATA'].rstrip("\\") + "\\OpenRGB"
                 else:
                     directory = '.'
             with open(f'{directory.rstrip("/")}/{name}.orp', 'wb') as f:
-                f.write(utils.Profile([dev.data for dev in self.devices]).pack())
+                f.write(utils.LocalProfile(
+                    [dev.data for dev in self.devices]).pack())
         else:
-            if self.comms._protocol_version < 2:
-                raise utils.SDKVersionError("Your version of OpenRGB doesn't support SDK profile controls")
             if type(name) is str:
                 try:
-                    name = next(p for p in self.profiles if p.name.lower() == name.lower())
+                    name = next(
+                        p for p in self.profiles if p.name.lower() == name.lower())
                 except StopIteration:
-                    name = utils.Profile(name)
+                    name = utils.Profile(name)  # type: ignore
             elif type(name) is int:
                 name = self.profiles[name]
             elif type(name) is utils.Profile:
                 pass
-            name = name.pack()
-            self.comms.send_header(0, utils.PacketType.REQUEST_SAVE_PROFILE, len(name))
-            self.comms.send_data(name)
+            raw_name = name.pack()  # type: ignore
+            self.comms.send_header(
+                0, utils.PacketType.REQUEST_SAVE_PROFILE, len(raw_name))
+            self.comms.send_data(raw_name)
             self.update_profiles()
 
     def delete_profile(self, name: Union[str, int, utils.Profile]):
         '''
         Deletes the selected profile
 
         :param name: Can be a profile's name, index, or even the Profile itself
         '''
-        if self.comms._protocol_version < 2:
-            raise utils.SDKVersionError("Your version of OpenRGB doesn't support SDK profile controls")
         if type(name) is str:
             try:
-                name = next(p for p in self.profiles if p.name.lower() == name.lower())
+                name = next(
+                    p for p in self.profiles if p.name.lower() == name.lower())
             except StopIteration as e:
                 raise ValueError(f"`{name}` is not an existing profile") from e
         elif type(name) is int:
             name = self.profiles[name]
         elif type(name) is utils.Profile:
             pass
-        name = name.pack()
-        self.comms.send_header(0, utils.PacketType.REQUEST_DELETE_PROFILE, len(name))
-        self.comms.send_data(name)
+        raw_name = name.pack()  # type: ignore
+        self.comms.send_header(
+            0, utils.PacketType.REQUEST_DELETE_PROFILE, len(raw_name))
+        self.comms.send_data(raw_name)
         self.update_profiles()
 
     def update(self):
         '''
         Gets the current state of your devices from the SDK server, which is
         useful if you change something from the gui or another SDK client and
         need to sync up the changes.
         '''
         self.comms.requestDeviceNum()
         for x in range(self.device_num):
             self.comms.requestDeviceData(x)
+        if self.comms._protocol_version >= 2:
+            self.update_profiles()
+        if self.comms._protocol_version >= 4:
+            self.update_plugins()
 
     def update_profiles(self):
         '''
         Gets the list of available profiles from the server.
         '''
-        if self.comms._protocol_version < 2:
-            raise utils.SDKVersionError("Your version of OpenRGB doesn't support SDK profile controls")
         self.comms.requestProfileList()
 
+    def update_plugins(self):
+        '''
+        Gets the list of enabled plugins from the server.
+        '''
+        self.comms.requestPluginList()
+        for plugin in self.plugins:
+            plugin.update()
+
     def show(self, fast: bool = False, force: bool = False):
         '''
         Shows all devices
 
         :param fast: If you care more about quickly setting colors than having correct internal state data, then set :code:`fast` to :code:`True`
         :param force: Sets all colors rather than trying to only set the ones that have been changed
         '''
@@ -479,15 +614,16 @@
 
     @protocol_version.setter
     def protocol_version(self, version: int):
         '''Sets the procol version of the connected SDK server'''
         if version <= self.comms.max_protocol_version:
             self.comms._protocol_version = version
         else:
-            raise ValueError(f"version {version} is greater than maximum supported version {self.comms.max_protocol_version}")
+            raise ValueError(
+                f"version {version} is greater than maximum supported version {self.comms.max_protocol_version}")
 
     @property
     def ee_devices(self):
         '''
         A subset of the device list that only includes devices with a direct
         control mode.  These devices are suitable to use with an effects engine.
         '''
```

### Comparing `openrgb-python-0.2.9/openrgb_python.egg-info/PKG-INFO` & `openrgb-python-0.3.0/openrgb_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrgb-python
-Version: 0.2.9
+Version: 0.3.0
 Summary: A python client for the OpenRGB SDK
 Home-page: https://github.com/jath03/openrgb-python
 Author: jath03
 License: UNKNOWN
 Description: # OpenRGB-Python
         
         
@@ -42,16 +42,17 @@
         Arch Linux:
         `yay -S python-openrgb-git`
         
         For a more stable package:
         
         `pip3 install openrgb-python`
         
-        Arch Linux:
-        `yay -S python-openrgb`
+        ~~Arch Linux:
+        `yay -S python-openrgb`~~
+        This AUR package is out of date. Use `python-openrgb-git` instead.
         
         Thanks to @GabMus for the AUR packages
         
         # Usage
         
         ```python
         from openrgb import OpenRGBClient
```

### Comparing `openrgb-python-0.2.9/setup.py` & `openrgb-python-0.3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="openrgb-python",
-    version='0.2.9',
+    version='0.3.0',
     author="jath03",
     description="A python client for the OpenRGB SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jath03/openrgb-python",
     packages=setuptools.find_packages(),
     classifiers=[
```

