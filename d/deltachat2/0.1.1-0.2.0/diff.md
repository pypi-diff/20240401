# Comparing `tmp/deltachat2-0.1.1.tar.gz` & `tmp/deltachat2-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat2-0.1.1.tar", last modified: Sat Mar 30 09:52:29 2024, max compression
+gzip compressed data, was "deltachat2-0.2.0.tar", last modified: Mon Apr  1 14:07:59 2024, max compression
```

## Comparing `deltachat2-0.1.1.tar` & `deltachat2-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:52:29.131635 deltachat2-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:52:29.123635 deltachat2-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:52:29.127635 deltachat2-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-30 09:52:19.000000 deltachat2-0.1.1/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-30 09:52:19.000000 deltachat2-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-03-30 09:52:19.000000 deltachat2-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-03-30 09:52:29.131635 deltachat2-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-30 09:52:19.000000 deltachat2-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:52:29.127635 deltachat2-0.1.1/deltachat2/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-30 09:52:19.000000 deltachat2-0.1.1/deltachat2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-30 09:52:19.000000 deltachat2-0.1.1/deltachat2/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-03-30 09:52:19.000000 deltachat2-0.1.1/deltachat2/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-03-30 09:52:19.000000 deltachat2-0.1.1/deltachat2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-03-30 09:52:19.000000 deltachat2-0.1.1/deltachat2/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-30 09:52:19.000000 deltachat2-0.1.1/deltachat2/rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-03-30 09:52:19.000000 deltachat2-0.1.1/deltachat2/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-03-30 09:52:19.000000 deltachat2-0.1.1/deltachat2/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-30 09:52:19.000000 deltachat2-0.1.1/deltachat2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:52:29.131635 deltachat2-0.1.1/deltachat2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-03-30 09:52:29.000000 deltachat2-0.1.1/deltachat2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-30 09:52:29.000000 deltachat2-0.1.1/deltachat2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 09:52:29.000000 deltachat2-0.1.1/deltachat2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-30 09:52:29.000000 deltachat2-0.1.1/deltachat2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-30 09:52:29.000000 deltachat2-0.1.1/deltachat2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:52:29.127635 deltachat2-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-30 09:52:19.000000 deltachat2-0.1.1/examples/client.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1256 2024-03-30 09:52:19.000000 deltachat2-0.1.1/examples/echobot.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-30 09:52:19.000000 deltachat2-0.1.1/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-30 09:52:19.000000 deltachat2-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 09:52:29.131635 deltachat2-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:07:59.995344 deltachat2-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:07:59.991344 deltachat2-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:07:59.991344 deltachat2-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-01 14:07:50.000000 deltachat2-0.2.0/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-01 14:07:50.000000 deltachat2-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-01 14:07:50.000000 deltachat2-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-01 14:07:59.995344 deltachat2-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-01 14:07:50.000000 deltachat2-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:07:59.995344 deltachat2-0.2.0/deltachat2/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:07:59.995344 deltachat2-0.2.0/deltachat2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-01 14:07:59.000000 deltachat2-0.2.0/deltachat2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-01 14:07:59.000000 deltachat2-0.2.0/deltachat2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:07:59.000000 deltachat2-0.2.0/deltachat2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-01 14:07:59.000000 deltachat2-0.2.0/deltachat2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 14:07:59.000000 deltachat2-0.2.0/deltachat2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:07:59.995344 deltachat2-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-01 14:07:50.000000 deltachat2-0.2.0/examples/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1256 2024-04-01 14:07:50.000000 deltachat2-0.2.0/examples/echobot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-01 14:07:50.000000 deltachat2-0.2.0/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-01 14:07:50.000000 deltachat2-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:07:59.995344 deltachat2-0.2.0/setup.cfg
```

### Comparing `deltachat2-0.1.1/.github/workflows/python-ci.yml` & `deltachat2-0.2.0/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `deltachat2-0.1.1/LICENSE` & `deltachat2-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deltachat2-0.1.1/PKG-INFO` & `deltachat2-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat2
-Version: 0.1.1
+Version: 0.2.0
 Summary: Client library for Delta Chat core JSON-RPC interface
 Author-email: adbenitez <adb@merlinux.eu>
 Keywords: deltachat
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `deltachat2-0.1.1/README.md` & `deltachat2-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `deltachat2-0.1.1/deltachat2/_utils.py` & `deltachat2-0.2.0/deltachat2/_utils.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.1.1/deltachat2/bot.py` & `deltachat2-0.2.0/deltachat2/bot.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.1.1/deltachat2/client.py` & `deltachat2-0.2.0/deltachat2/client.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.1.1/deltachat2/events.py` & `deltachat2-0.2.0/deltachat2/events.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.1.1/deltachat2/rpc.py` & `deltachat2-0.2.0/deltachat2/rpc.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.1.1/deltachat2/transport.py` & `deltachat2-0.2.0/deltachat2/transport.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.1.1/deltachat2/types.py` & `deltachat2-0.2.0/deltachat2/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -130,14 +130,118 @@
     CHAT_PROTECTION_DISABLED = "ChatProtectionDisabled"
     WEBXDC_STATUS_UPDATE = "WebxdcStatusUpdate"
     EPHEMERAL_TIMER_CHANGED = "EphemeralTimerChanged"
     MULTI_DEVICE_SYNC = "MultiDeviceSync"
     WEBXDC_INFO_MESSAGE = "WebxdcInfoMessage"
 
 
+class MessageState(IntEnum):
+    """State of the message."""
+
+    UNDEFINED = 0
+    IN_FRESH = 10
+    IN_NOTICED = 13
+    IN_SEEN = 16
+    OUT_PREPARING = 18
+    OUT_DRAFT = 19
+    OUT_PENDING = 20
+    OUT_FAILED = 24
+    OUT_DELIVERED = 26
+    OUT_MDN_RCVD = 28
+
+
+class SpecialMessageId(IntEnum):
+    """Special message ids"""
+
+    DAYMARKER = 9
+    LAST_SPECIAL = 9
+
+
+class CertificateChecks(IntEnum):
+    """Certificate checks mode"""
+
+    AUTOMATIC = 0
+    STRICT = 1
+    ACCEPT_INVALID_CERTIFICATES = 3
+
+
+class Connectivity(IntEnum):
+    """Connectivity states"""
+
+    NOT_CONNECTED = 1000
+    CONNECTING = 2000
+    WORKING = 3000
+    CONNECTED = 4000
+
+
+class KeyGenType(IntEnum):
+    """Type of the key to generate"""
+
+    DEFAULT = 0
+    RSA2048 = 1
+    ED25519 = 2
+    RSA4096 = 3
+
+
+# "Lp" means "login parameters"
+class LpAuthFlag(IntEnum):
+    """Authorization flags"""
+
+    OAUTH2 = 0x2
+    NORMAL = 0x4
+
+
+class MediaQuality(IntEnum):
+    """Media quality setting"""
+
+    BALANCED = 0
+    WORSE = 1
+
+
+class ProviderStatus(IntEnum):
+    """Provider status according to manual testing"""
+
+    OK = 1
+    PREPARATION = 2
+    BROKEN = 3
+
+
+class PushNotifyState(IntEnum):
+    """Push notifications state"""
+
+    NOT_CONNECTED = 0
+    HEARTBEAT = 1
+    CONNECTED = 2
+
+
+class ShowEmails(IntEnum):
+    """Show emails mode"""
+
+    OFF = 0
+    ACCEPTED_CONTACTS = 1
+    ALL = 2
+
+
+class SocketSecurity(IntEnum):
+    """Socket security"""
+
+    AUTOMATIC = 0
+    SSL = 1
+    STARTTLS = 2
+    PLAIN = 3
+
+
+class VideochatType(IntEnum):
+    """Video chat URL type"""
+
+    UNKNOWN = 0
+    BASICWEBRTC = 1
+    JITSI = 2
+
+
 class CoreEvent(AttrDict):
     """Delta Chat core Event"""
 
     kind: EventType
 
 
 @dataclass
```

### Comparing `deltachat2-0.1.1/deltachat2/util.py` & `deltachat2-0.2.0/deltachat2/util.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.1.1/deltachat2.egg-info/PKG-INFO` & `deltachat2-0.2.0/deltachat2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat2
-Version: 0.1.1
+Version: 0.2.0
 Summary: Client library for Delta Chat core JSON-RPC interface
 Author-email: adbenitez <adb@merlinux.eu>
 Keywords: deltachat
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `deltachat2-0.1.1/examples/client.py` & `deltachat2-0.2.0/examples/client.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.1.1/examples/echobot.py` & `deltachat2-0.2.0/examples/echobot.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.1.1/pyproject.toml` & `deltachat2-0.2.0/pyproject.toml`

 * *Files identical despite different names*

