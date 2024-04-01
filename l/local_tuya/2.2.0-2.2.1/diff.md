# Comparing `tmp/local_tuya-2.2.0.tar.gz` & `tmp/local_tuya-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_tuya-2.2.0.tar", max compression
+gzip compressed data, was "local_tuya-2.2.1.tar", max compression
```

## Comparing `local_tuya-2.2.0.tar` & `local_tuya-2.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1070 2024-02-01 17:06:18.203333 local_tuya-2.2.0/LICENSE
--rw-r--r--   0        0        0     2484 2024-02-01 17:06:18.203333 local_tuya-2.2.0/README.md
--rw-r--r--   0        0        0      445 2024-02-01 17:06:18.203333 local_tuya-2.2.0/local_tuya/__init__.py
--rw-r--r--   0        0        0      939 2024-02-01 17:06:18.203333 local_tuya-2.2.0/local_tuya/backoff.py
--rw-r--r--   0        0        0     1580 2024-02-01 17:06:18.203333 local_tuya-2.2.0/local_tuya/device/README.md
--rw-r--r--   0        0        0      213 2024-02-01 17:06:18.203333 local_tuya-2.2.0/local_tuya/device/__init__.py
--rw-r--r--   0        0        0     3341 2024-02-01 17:06:18.203333 local_tuya-2.2.0/local_tuya/device/buffer.py
--rw-r--r--   0        0        0      395 2024-02-01 17:06:18.203333 local_tuya-2.2.0/local_tuya/device/config.py
--rw-r--r--   0        0        0     1855 2024-02-01 17:06:18.203333 local_tuya-2.2.0/local_tuya/device/constraints.py
--rw-r--r--   0        0        0     2268 2024-02-01 17:06:18.203333 local_tuya-2.2.0/local_tuya/device/device.py
--rw-r--r--   0        0        0      786 2024-02-01 17:06:18.203333 local_tuya-2.2.0/local_tuya/device/enums.py
--rw-r--r--   0        0        0     1288 2024-02-01 17:06:18.203333 local_tuya-2.2.0/local_tuya/device/state.py
--rw-r--r--   0        0        0      541 2024-02-01 17:06:18.203333 local_tuya-2.2.0/local_tuya/errors.py
--rw-r--r--   0        0        0     1149 2024-02-01 17:06:18.203333 local_tuya-2.2.0/local_tuya/events.py
--rw-r--r--   0        0        0      943 2024-02-01 17:06:18.203333 local_tuya-2.2.0/local_tuya/protocol/README.md
--rw-r--r--   0        0        0      167 2024-02-01 17:06:18.203333 local_tuya-2.2.0/local_tuya/protocol/__init__.py
--rw-r--r--   0        0        0      895 2024-02-01 17:06:18.203333 local_tuya-2.2.0/local_tuya/protocol/config.py
--rw-r--r--   0        0        0      628 2024-02-01 17:06:18.203333 local_tuya-2.2.0/local_tuya/protocol/events.py
--rw-r--r--   0        0        0     1051 2024-02-01 17:06:18.203333 local_tuya-2.2.0/local_tuya/protocol/heartbeat.py
--rw-r--r--   0        0        0      321 2024-02-01 17:06:18.207333 local_tuya-2.2.0/local_tuya/protocol/message/__init__.py
--rw-r--r--   0        0        0      549 2024-02-01 17:06:18.207333 local_tuya-2.2.0/local_tuya/protocol/message/handlers/__init__.py
--rw-r--r--   0        0        0      827 2024-02-01 17:06:18.207333 local_tuya-2.2.0/local_tuya/protocol/message/handlers/crypto.py
--rw-r--r--   0        0        0      759 2024-02-01 17:06:18.207333 local_tuya-2.2.0/local_tuya/protocol/message/handlers/handler.py
--rw-r--r--   0        0        0     6480 2024-02-01 17:06:18.207333 local_tuya-2.2.0/local_tuya/protocol/message/handlers/v33.py
--rw-r--r--   0        0        0     1582 2024-02-01 17:06:18.207333 local_tuya-2.2.0/local_tuya/protocol/message/messages.py
--rw-r--r--   0        0        0     2631 2024-02-01 17:06:18.207333 local_tuya-2.2.0/local_tuya/protocol/protocol.py
--rw-r--r--   0        0        0     1711 2024-02-01 17:06:18.207333 local_tuya-2.2.0/local_tuya/protocol/receiver.py
--rw-r--r--   0        0        0     3453 2024-02-01 17:06:18.207333 local_tuya-2.2.0/local_tuya/protocol/sender.py
--rw-r--r--   0        0        0     2368 2024-02-01 17:06:18.207333 local_tuya-2.2.0/local_tuya/protocol/state.py
--rw-r--r--   0        0        0     4318 2024-02-01 17:06:18.207333 local_tuya-2.2.0/local_tuya/protocol/transport.py
--rw-r--r--   0        0        0        0 2024-02-01 17:06:18.207333 local_tuya-2.2.0/local_tuya/py.typed
--rw-r--r--   0        0        0      938 2024-02-01 17:06:18.207333 local_tuya-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     3258 1970-01-01 00:00:00.000000 local_tuya-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-01 15:42:55.128870 local_tuya-2.2.1/LICENSE
+-rw-r--r--   0        0        0     2499 2024-04-01 15:42:55.128870 local_tuya-2.2.1/README.md
+-rw-r--r--   0        0        0      445 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/__init__.py
+-rw-r--r--   0        0        0      939 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/backoff.py
+-rw-r--r--   0        0        0     1580 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/device/README.md
+-rw-r--r--   0        0        0      213 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/device/__init__.py
+-rw-r--r--   0        0        0     3341 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/device/buffer.py
+-rw-r--r--   0        0        0      395 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/device/config.py
+-rw-r--r--   0        0        0     1855 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/device/constraints.py
+-rw-r--r--   0        0        0     2268 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/device/device.py
+-rw-r--r--   0        0        0      786 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/device/enums.py
+-rw-r--r--   0        0        0     1288 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/device/state.py
+-rw-r--r--   0        0        0      541 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/errors.py
+-rw-r--r--   0        0        0     1149 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/events.py
+-rw-r--r--   0        0        0      943 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/README.md
+-rw-r--r--   0        0        0      167 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/__init__.py
+-rw-r--r--   0        0        0      895 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/config.py
+-rw-r--r--   0        0        0      616 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/events.py
+-rw-r--r--   0        0        0     1051 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/heartbeat.py
+-rw-r--r--   0        0        0      321 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/message/__init__.py
+-rw-r--r--   0        0        0      549 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/message/handlers/__init__.py
+-rw-r--r--   0        0        0      827 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/message/handlers/crypto.py
+-rw-r--r--   0        0        0      759 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/message/handlers/handler.py
+-rw-r--r--   0        0        0     6480 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/message/handlers/v33.py
+-rw-r--r--   0        0        0     1562 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/message/messages.py
+-rw-r--r--   0        0        0     2632 2024-04-01 15:42:55.132870 local_tuya-2.2.1/local_tuya/protocol/protocol.py
+-rw-r--r--   0        0        0     1711 2024-04-01 15:42:55.132870 local_tuya-2.2.1/local_tuya/protocol/receiver.py
+-rw-r--r--   0        0        0     3453 2024-04-01 15:42:55.132870 local_tuya-2.2.1/local_tuya/protocol/sender.py
+-rw-r--r--   0        0        0     2368 2024-04-01 15:42:55.132870 local_tuya-2.2.1/local_tuya/protocol/state.py
+-rw-r--r--   0        0        0     4318 2024-04-01 15:42:55.132870 local_tuya-2.2.1/local_tuya/protocol/transport.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:42:55.132870 local_tuya-2.2.1/local_tuya/py.typed
+-rw-r--r--   0        0        0      957 2024-04-01 15:42:55.132870 local_tuya-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 local_tuya-2.2.1/PKG-INFO
```

### Comparing `local_tuya-2.2.0/LICENSE` & `local_tuya-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/README.md` & `local_tuya-2.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # local-tuya
 
-[![tests](https://github.com/gpajot/local-tuya/workflows/Test/badge.svg?branch=main&event=push)](https://github.com/gpajot/local-tuya/actions?query=workflow%3ATest+branch%3Amain+event%3Apush)
-[![version](https://img.shields.io/pypi/v/local-tuya?label=stable)](https://pypi.org/project/local-tuya/)
-[![python](https://img.shields.io/pypi/pyversions/local-tuya)](https://pypi.org/project/local-tuya/)
+[![tests](https://github.com/gpajot/local-tuya/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/gpajot/local-tuya/actions/workflows/test.yml?query=branch%3Amain+event%3Apush)
+[![version](https://img.shields.io/pypi/v/local_tuya?label=stable)](https://pypi.org/project/local_tuya/)
+[![python](https://img.shields.io/pypi/pyversions/local_tuya)](https://pypi.org/project/local_tuya/)
 
 Interface to Tuya devices over LAN.
 
 ## Features
 - asynchronous methods and transport
 - persistent communication to the device
 - automatic remote device state updates (remotes can still be used)
```

### Comparing `local_tuya-2.2.0/local_tuya/backoff.py` & `local_tuya-2.2.1/local_tuya/backoff.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/device/README.md` & `local_tuya-2.2.1/local_tuya/device/README.md`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/device/buffer.py` & `local_tuya-2.2.1/local_tuya/device/buffer.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/device/constraints.py` & `local_tuya-2.2.1/local_tuya/device/constraints.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/device/device.py` & `local_tuya-2.2.1/local_tuya/device/device.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/device/enums.py` & `local_tuya-2.2.1/local_tuya/device/enums.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/device/state.py` & `local_tuya-2.2.1/local_tuya/device/state.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/errors.py` & `local_tuya-2.2.1/local_tuya/errors.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/events.py` & `local_tuya-2.2.1/local_tuya/events.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/protocol/README.md` & `local_tuya-2.2.1/local_tuya/protocol/README.md`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/protocol/config.py` & `local_tuya-2.2.1/local_tuya/protocol/config.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/protocol/events.py` & `local_tuya-2.2.1/local_tuya/protocol/events.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 from dataclasses import dataclass
 from typing import Optional, Type
 
 from local_tuya.events import Event
 from local_tuya.protocol.message import Command, Response, Values
 
 
-class ConnectionEstablished(Event):
-    ...
+class ConnectionEstablished(Event): ...
 
 
 @dataclass
 class ConnectionLost(Event):
     error: Optional[Exception]
 
 
-class DataSent(bytes, Event):
-    ...
+class DataSent(bytes, Event): ...
 
 
-class DataReceived(bytes, Event):
-    ...
+class DataReceived(bytes, Event): ...
 
 
 @dataclass
 class CommandSent(Event):
     command: Command
```

### Comparing `local_tuya-2.2.0/local_tuya/protocol/heartbeat.py` & `local_tuya-2.2.1/local_tuya/protocol/heartbeat.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/protocol/message/handlers/__init__.py` & `local_tuya-2.2.1/local_tuya/protocol/message/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/protocol/message/handlers/crypto.py` & `local_tuya-2.2.1/local_tuya/protocol/message/handlers/crypto.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/protocol/message/handlers/handler.py` & `local_tuya-2.2.1/local_tuya/protocol/message/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/protocol/message/handlers/v33.py` & `local_tuya-2.2.1/local_tuya/protocol/message/handlers/v33.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/protocol/message/messages.py` & `local_tuya-2.2.1/local_tuya/protocol/message/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,20 +33,18 @@
     _error: Optional[ResponseError] = None
 
     @property
     def error(self) -> Optional[ResponseError]:
         return self._error
 
 
-class HeartbeatCommand(EmptyCommand):
-    ...
+class HeartbeatCommand(EmptyCommand): ...
 
 
-class HeartbeatResponse(EmptyResponse):
-    ...
+class HeartbeatResponse(EmptyResponse): ...
 
 
 class StatusResponse:
     def __init__(
         self,
         payload: Optional[Payload] = None,
         error: Optional[ResponseError] = None,
@@ -55,26 +53,23 @@
         self.values: Values = {}
         if payload and "dps" in payload and isinstance(payload["dps"], dict):
             self.values = payload["dps"]
         if not self.values and not self.error:
             self.error = DecodeResponseError("no dps in response")
 
 
-class StateCommand(EmptyCommand):
-    ...
+class StateCommand(EmptyCommand): ...
 
 
-class StateResponse(StatusResponse):
-    ...
+class StateResponse(StatusResponse): ...
 
 
 @dataclass
 class UpdateCommand:
     values: Values
 
     @property
     def payload(self) -> Payload:
         return {"dps": self.values}
 
 
-class UpdateResponse(EmptyResponse):
-    ...
+class UpdateResponse(EmptyResponse): ...
```

### Comparing `local_tuya-2.2.0/local_tuya/protocol/protocol.py` & `local_tuya-2.2.1/local_tuya/protocol/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from local_tuya.protocol.receiver import Receiver
 from local_tuya.protocol.sender import Sender
 from local_tuya.protocol.state import State
 from local_tuya.protocol.transport import Transport
 
 
 def _state_updated_callback(
-    func: Callable[[Values], Awaitable]
+    func: Callable[[Values], Awaitable],
 ) -> Callable[[StateUpdated], Awaitable]:
     async def _wrapper(event: StateUpdated) -> None:
         await func(event.values)
 
     return _wrapper
```

### Comparing `local_tuya-2.2.0/local_tuya/protocol/receiver.py` & `local_tuya-2.2.1/local_tuya/protocol/receiver.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/protocol/sender.py` & `local_tuya-2.2.1/local_tuya/protocol/sender.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/protocol/state.py` & `local_tuya-2.2.1/local_tuya/protocol/state.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/local_tuya/protocol/transport.py` & `local_tuya-2.2.1/local_tuya/protocol/transport.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.0/PKG-INFO` & `local_tuya-2.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: local_tuya
-Version: 2.2.0
+Version: 2.2.1
 Summary: Interface to Tuya devices over LAN.
 Home-page: https://github.com/gpajot/local-tuya
 License: MIT
 Author: Gabriel Pajot
 Author-email: gab@les-cactus.co
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -12,22 +12,23 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: concurrent-tasks (>=1.6,<2)
 Requires-Dist: pycryptodomex (>=3,<4)
+Requires-Dist: typing-extensions (>=4.10)
 Project-URL: Repository, https://github.com/gpajot/local-tuya
 Description-Content-Type: text/markdown
 
 # local-tuya
 
-[![tests](https://github.com/gpajot/local-tuya/workflows/Test/badge.svg?branch=main&event=push)](https://github.com/gpajot/local-tuya/actions?query=workflow%3ATest+branch%3Amain+event%3Apush)
-[![version](https://img.shields.io/pypi/v/local-tuya?label=stable)](https://pypi.org/project/local-tuya/)
-[![python](https://img.shields.io/pypi/pyversions/local-tuya)](https://pypi.org/project/local-tuya/)
+[![tests](https://github.com/gpajot/local-tuya/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/gpajot/local-tuya/actions/workflows/test.yml?query=branch%3Amain+event%3Apush)
+[![version](https://img.shields.io/pypi/v/local_tuya?label=stable)](https://pypi.org/project/local_tuya/)
+[![python](https://img.shields.io/pypi/pyversions/local_tuya)](https://pypi.org/project/local_tuya/)
 
 Interface to Tuya devices over LAN.
 
 ## Features
 - asynchronous methods and transport
 - persistent communication to the device
 - automatic remote device state updates (remotes can still be used)
```

