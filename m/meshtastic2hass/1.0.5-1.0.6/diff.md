# Comparing `tmp/meshtastic2hass-1.0.5.tar.gz` & `tmp/meshtastic2hass-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshtastic2hass-1.0.5.tar", last modified: Sat Feb  3 18:19:25 2024, max compression
+gzip compressed data, was "meshtastic2hass-1.0.6.tar", last modified: Mon Apr  1 14:09:30 2024, max compression
```

## Comparing `meshtastic2hass-1.0.5.tar` & `meshtastic2hass-1.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:19:25.628182 meshtastic2hass-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-03 18:19:12.000000 meshtastic2hass-1.0.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:19:25.620182 meshtastic2hass-1.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:19:25.624182 meshtastic2hass-1.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-02-03 18:19:12.000000 meshtastic2hass-1.0.5/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-03 18:19:12.000000 meshtastic2hass-1.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-02-03 18:19:12.000000 meshtastic2hass-1.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-02-03 18:19:12.000000 meshtastic2hass-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-02-03 18:19:25.628182 meshtastic2hass-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-02-03 18:19:12.000000 meshtastic2hass-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-02-03 18:19:12.000000 meshtastic2hass-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-02-03 18:19:25.628182 meshtastic2hass-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-03 18:19:12.000000 meshtastic2hass-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:19:25.624182 meshtastic2hass-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:19:25.624182 meshtastic2hass-1.0.5/src/meshtastic2hass/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-03 18:19:12.000000 meshtastic2hass-1.0.5/src/meshtastic2hass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-03 18:19:12.000000 meshtastic2hass-1.0.5/src/meshtastic2hass/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-02-03 18:19:12.000000 meshtastic2hass-1.0.5/src/meshtastic2hass/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-02-03 18:19:12.000000 meshtastic2hass-1.0.5/src/meshtastic2hass/meshtastic2hass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 18:19:25.628182 meshtastic2hass-1.0.5/src/meshtastic2hass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-02-03 18:19:25.000000 meshtastic2hass-1.0.5/src/meshtastic2hass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-02-03 18:19:25.000000 meshtastic2hass-1.0.5/src/meshtastic2hass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 18:19:25.000000 meshtastic2hass-1.0.5/src/meshtastic2hass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 18:19:25.000000 meshtastic2hass-1.0.5/src/meshtastic2hass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-03 18:19:25.000000 meshtastic2hass-1.0.5/src/meshtastic2hass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-03 18:19:25.000000 meshtastic2hass-1.0.5/src/meshtastic2hass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:09:30.141947 meshtastic2hass-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-01 14:09:18.000000 meshtastic2hass-1.0.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:09:30.137947 meshtastic2hass-1.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:09:30.137947 meshtastic2hass-1.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-01 14:09:18.000000 meshtastic2hass-1.0.6/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-01 14:09:18.000000 meshtastic2hass-1.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-01 14:09:18.000000 meshtastic2hass-1.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-01 14:09:18.000000 meshtastic2hass-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-01 14:09:30.141947 meshtastic2hass-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-01 14:09:18.000000 meshtastic2hass-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-01 14:09:18.000000 meshtastic2hass-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-01 14:09:30.141947 meshtastic2hass-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-01 14:09:18.000000 meshtastic2hass-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:09:30.137947 meshtastic2hass-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:09:30.137947 meshtastic2hass-1.0.6/src/meshtastic2hass/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-01 14:09:18.000000 meshtastic2hass-1.0.6/src/meshtastic2hass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-01 14:09:18.000000 meshtastic2hass-1.0.6/src/meshtastic2hass/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-01 14:09:18.000000 meshtastic2hass-1.0.6/src/meshtastic2hass/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14459 2024-04-01 14:09:18.000000 meshtastic2hass-1.0.6/src/meshtastic2hass/meshtastic2hass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:09:30.141947 meshtastic2hass-1.0.6/src/meshtastic2hass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-01 14:09:30.000000 meshtastic2hass-1.0.6/src/meshtastic2hass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-01 14:09:30.000000 meshtastic2hass-1.0.6/src/meshtastic2hass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:09:30.000000 meshtastic2hass-1.0.6/src/meshtastic2hass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:09:29.000000 meshtastic2hass-1.0.6/src/meshtastic2hass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-01 14:09:30.000000 meshtastic2hass-1.0.6/src/meshtastic2hass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 14:09:30.000000 meshtastic2hass-1.0.6/src/meshtastic2hass.egg-info/top_level.txt
```

### Comparing `meshtastic2hass-1.0.5/.coveragerc` & `meshtastic2hass-1.0.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.5/.github/workflows/python-package.yml` & `meshtastic2hass-1.0.6/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.5/.github/workflows/python-publish.yml` & `meshtastic2hass-1.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.5/.gitignore` & `meshtastic2hass-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.5/LICENSE` & `meshtastic2hass-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.5/PKG-INFO` & `meshtastic2hass-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: meshtastic2hass
-Version: 1.0.5
-Summary: Add a short description here!
+Version: 1.0.6
+Summary: A Python client that connects Meshtastic radios via MQTT to Home Assistant (Hass).
 Home-page: https://github.com/Mictronics/meshtastic2hass
 Author: Michael Wolf
 Author-email: michael@mictronics.de
 License: GPL v3+
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `meshtastic2hass-1.0.5/README.md` & `meshtastic2hass-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.5/setup.cfg` & `meshtastic2hass-1.0.6/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = meshtastic2hass
-description = Add a short description here!
+description = A Python client that connects Meshtastic radios via MQTT to Home Assistant (Hass).
 author = Michael Wolf
 author_email = michael@mictronics.de
 license = GPL v3+
 license_files = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/Mictronics/meshtastic2hass
```

### Comparing `meshtastic2hass-1.0.5/setup.py` & `meshtastic2hass-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.5/src/meshtastic2hass/__init__.py` & `meshtastic2hass-1.0.6/src/meshtastic2hass/__init__.py`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.5/src/meshtastic2hass/globals.py` & `meshtastic2hass-1.0.6/src/meshtastic2hass/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,15 @@
                 device_class="current",
                 unit="mA",
                 property="ch3Current",
                 type="float",
             ),
         ]
         self.mqttTopicPrefix = "msh/2/json"
+        self.channelList = []
 
     def reset(self):
         """Reset all of our globals. If you add a member, add it to this method, too."""
         self.args = None
         self.parser = None
         self.loop = None
         self.mqtt = None
@@ -244,7 +245,11 @@
     def getSensors(self):
         """Get the MQTT sensor configuration"""
         return self.mqttSensors
 
     def getTopicPrefix(self):
         """Get the MQTT topic prefix"""
         return self.mqttTopicPrefix
+
+    def getChannelList(self):
+        """Get the local nodes channel list"""
+        return self.channelList
```

### Comparing `meshtastic2hass-1.0.5/src/meshtastic2hass/meshtastic2hass.py` & `meshtastic2hass-1.0.6/src/meshtastic2hass/meshtastic2hass.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,23 +22,24 @@
 import json
 import os
 import signal
 import sys
 
 import meshtastic
 import meshtastic.serial_interface
+from meshtastic import config_pb2
 import paho.mqtt.client as mqttClient
 from globals import Globals
 from pubsub import pub
 from tomlkit import toml_file
 
 __author__ = "Michael Wolf aka Mictronics"
 __copyright__ = "2024, (C) Michael Wolf"
 __license__ = "GPL v3+"
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 
 
 def onReceiveTelemetry(packet, interface, topic=pub.AUTO_TOPIC):
     """Callback invoked when a telemetry or position packet arrives."""
     # Create JSON from Mesh packet.
     _globals = Globals.getInstance()
     mqtt = _globals.getMQTT()
@@ -138,43 +139,50 @@
         mqtt.publish(
             mqttTopic, json.dumps(jsonObj, separators=(",", ":")), qos=1
         ).wait_for_publish(1)
 
 
 def onReceiveText(packet, interface, topic=pub.AUTO_TOPIC):
     """Callback invoked when a text packet arrives."""
-    _globals = Globals.getInstance()
-    mqtt = _globals.getMQTT()
-    topicPrefix = _globals.getTopicPrefix()
-    jsonObj = {}
-    fromId = packet.get("fromId")
-    shortName = interface.nodes.get(fromId).get("user").get("shortName")
-    # No special characters allowed in config topic
-    fromId = fromId.strip("!")
-    # Publish auto discovery configuration for MQTT text entity
-    mqttTopic = f"homeassistant/text/{fromId}/config"
-    jsonObj["name"] = f"{shortName} Text"
-    jsonObj["unique_id"] = f"{shortName.lower()}_text"
-    jsonObj["command_topic"] = f"{topicPrefix}/{fromId}/command"
-    jsonObj["state_topic"] = f"{topicPrefix}/{fromId}/state"
-    jsonObj["value_template"] = "{{ value_json.text }}"
-    jsonObj["mode"] = "text"
-    jsonObj["icon"] = "mdi:message-text"
-    mqtt.publish(
-        mqttTopic, json.dumps(jsonObj, separators=(",", ":")), qos=1
-    ).wait_for_publish(1)
-    # Publish position payload for device tracker in attributes topic
-    jsonObj.clear()
-    text = packet.get("decoded").get("text")
-    if text:
-        jsonObj["text"] = text
-        mqttTopic = f"{topicPrefix}/{fromId}/state"
+    try:
+        _globals = Globals.getInstance()
+        mqtt = _globals.getMQTT()
+        channelList = _globals.getChannelList()
+        topicPrefix = _globals.getTopicPrefix()
+        jsonObj = {}
+        fromName = interface.nodes.get(packet.get("fromId")).get("user").get("shortName")
+        if packet.get('channel'):
+            channelNumber = packet['channel']
+        else:
+            channelNumber = 0
+        channelName = channelList[channelNumber]
+        # Publish auto discovery configuration for MQTT text entity per channel
+        mqttTopic = f"homeassistant/text/{channelName}/config"
+        jsonObj["name"] = f"{channelName}"
+        jsonObj["unique_id"] = f"channel_{channelName.lower()}"
+        jsonObj["command_topic"] = f"{topicPrefix}/{channelName.lower()}/command"
+        jsonObj["state_topic"] = f"{topicPrefix}/{channelName.lower()}/state"
+        jsonObj["value_template"] = "{{ value_json.text }}"
+        jsonObj["mode"] = "text"
+        jsonObj["icon"] = "mdi:message-text"
         mqtt.publish(
             mqttTopic, json.dumps(jsonObj, separators=(",", ":")), qos=1
         ).wait_for_publish(1)
+        # Publish received text in corresponding channel entity in attributes topic
+        jsonObj.clear()
+        text = packet.get("decoded").get("text")
+        if text:
+            jsonObj["text"] = f"{fromName}: {text}"
+            mqttTopic = f"{topicPrefix}/{channelName.lower()}/state"
+            mqtt.publish(
+                mqttTopic, json.dumps(jsonObj, separators=(",", ":")), qos=1
+            ).wait_for_publish(1)
+
+    except Exception as ex:
+        print(f"Error processing text: {ex}")
 
 
 def onConnect(interface, topic=pub.AUTO_TOPIC):
     """Callback invoked when we connect to a radio"""
     print(f"Connection: {topic.getName()}")
 
 
@@ -182,25 +190,46 @@
     """Callback invoked when we disconnect from a radio"""
     print(f"Connection: {topic.getName()}")
     _globals = Globals.getInstance()
     if _globals.getLoop() is not None:
         _globals.getLoop().stop()
 
 
+def toCamelCase(string):
+    words = string.split('_')
+    camelCaseString = ''.join(word.capitalize() for word in words)
+    return camelCaseString
+
+
 def onConnected(interface):
     """Callback invoked when we are connected to a radio"""
     try:
         _globals = Globals.getInstance()
         print("Radio: connected")
         pub.subscribe(onReceiveText, "meshtastic.receive.text")
         pub.subscribe(onReceiveTelemetry, "meshtastic.receive.telemetry")
         pub.subscribe(onReceivePosition, "meshtastic.receive.position")
         pub.subscribe(onConnect, "meshtastic.connection.established")
         pub.subscribe(onDisconnect, "meshtastic.connection.lost")
 
+        channelList = _globals.getChannelList()
+        node = interface.getNode('^local')
+        deviceChannels = node.channels
+        for deviceChannel in deviceChannels:
+            if deviceChannel.role:
+                if deviceChannel.settings.name:
+                    channelList.append(deviceChannel.settings.name)
+
+                else:
+                    # If channel name is blank, use the modem preset
+                    loraConfig = node.localConfig.lora
+                    modemPresetEnum = loraConfig.modem_preset
+                    modemPresetString = config_pb2._CONFIG_LORACONFIG_MODEMPRESET.values_by_number[modemPresetEnum].name
+                    channelList.append(toCamelCase(modemPresetString))
+
     except Exception as ex:
         print(f"Aborting due to: {ex}")
         interface.close()
         sys.exit(1)
 
 
 def onMQTTMessage(mqttc, obj, msg):
```

### Comparing `meshtastic2hass-1.0.5/src/meshtastic2hass.egg-info/PKG-INFO` & `meshtastic2hass-1.0.6/src/meshtastic2hass.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: meshtastic2hass
-Version: 1.0.5
-Summary: Add a short description here!
+Version: 1.0.6
+Summary: A Python client that connects Meshtastic radios via MQTT to Home Assistant (Hass).
 Home-page: https://github.com/Mictronics/meshtastic2hass
 Author: Michael Wolf
 Author-email: michael@mictronics.de
 License: GPL v3+
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `meshtastic2hass-1.0.5/src/meshtastic2hass.egg-info/SOURCES.txt` & `meshtastic2hass-1.0.6/src/meshtastic2hass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

