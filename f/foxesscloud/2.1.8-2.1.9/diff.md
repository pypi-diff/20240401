# Comparing `tmp/foxesscloud-2.1.8.tar.gz` & `tmp/foxesscloud-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-hh17j2dx\foxesscloud-2.1.8.tar", last modified: Thu Mar 28 15:56:38 2024, max compression
+gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-xf0ec4om\foxesscloud-2.1.9.tar", last modified: Mon Apr  1 18:01:15 2024, max compression
```

## Comparing `foxesscloud-2.1.8.tar` & `foxesscloud-2.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 15:56:38.000000 foxesscloud-2.1.8/
--rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.1.8/LICENCE
--rw-rw-rw-   0        0        0    39006 2024-03-28 15:56:38.000000 foxesscloud-2.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    38451 2024-03-28 15:48:55.000000 foxesscloud-2.1.8/README.md
--rw-rw-rw-   0        0        0      635 2024-03-28 14:39:47.000000 foxesscloud-2.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-28 15:56:38.000000 foxesscloud-2.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-28 15:56:38.000000 foxesscloud-2.1.8/src/
-drwxrwxrwx   0        0        0        0 2024-03-28 15:56:38.000000 foxesscloud-2.1.8/src/foxesscloud/
--rw-rw-rw-   0        0        0   172475 2024-03-28 15:55:27.000000 foxesscloud-2.1.8/src/foxesscloud/foxesscloud.py
--rw-rw-rw-   0        0        0   166184 2024-03-28 15:43:40.000000 foxesscloud-2.1.8/src/foxesscloud/openapi.py
-drwxrwxrwx   0        0        0        0 2024-03-28 15:56:38.000000 foxesscloud-2.1.8/src/foxesscloud.egg-info/
--rw-rw-rw-   0        0        0    39006 2024-03-28 15:56:38.000000 foxesscloud-2.1.8/src/foxesscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-03-28 15:56:38.000000 foxesscloud-2.1.8/src/foxesscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 15:56:38.000000 foxesscloud-2.1.8/src/foxesscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-03-28 15:56:38.000000 foxesscloud-2.1.8/src/foxesscloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/
+-rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.1.9/LICENCE
+-rw-rw-rw-   0        0        0    39241 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    38686 2024-04-01 17:58:50.000000 foxesscloud-2.1.9/README.md
+-rw-rw-rw-   0        0        0      635 2024-04-01 13:28:21.000000 foxesscloud-2.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/src/foxesscloud/
+-rw-rw-rw-   0        0        0   174889 2024-04-01 17:51:43.000000 foxesscloud-2.1.9/src/foxesscloud/foxesscloud.py
+-rw-rw-rw-   0        0        0   169176 2024-04-01 17:51:43.000000 foxesscloud-2.1.9/src/foxesscloud/openapi.py
+drwxrwxrwx   0        0        0        0 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/src/foxesscloud.egg-info/
+-rw-rw-rw-   0        0        0    39241 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/src/foxesscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/src/foxesscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/src/foxesscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-01 18:01:15.000000 foxesscloud-2.1.9/src/foxesscloud.egg-info/top_level.txt
```

### Comparing `foxesscloud-2.1.8/LICENCE` & `foxesscloud-2.1.9/LICENCE`

 * *Files identical despite different names*

### Comparing `foxesscloud-2.1.8/PKG-INFO` & `foxesscloud-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxesscloud
-Version: 2.1.8
+Version: 2.1.9
 Summary: library for accessing Fox ESS cloud data using Open API
 Author-email: Tony Matthews <tony@quasair.co.uk>
 Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -454,14 +454,15 @@
 There are a number of different pre-configured tariffs:
 + Octopus Flux: off-peak from 02:00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed work mode change to Self Use at 7am and Feed In First at 4pm.
 + Intelligent Octopus: off-peak from 23:30 to 05:30, forecasts from 22:00 to 23:59
 + Octopus Cosy: off-peak from 04:00 to 07:00 and 13:00 to 16:00, peak from 16:00 to 19:00, forecasts from 02:00 to 03:59 and 12:00 to 12:59
 + Octopus Go: off peak from 00:30 to 04:30, forecasts from 22:00 to 23:59
 + Agile Octopus: off-peak from 02:30 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59
 + British Gas Electric Driver: off-peak from 00:00 to 05:00, forecasts from 22:00 to 23:59
++ Eco 7: Economy 7: off-peak from 00:30 to 07:30 GMT (01:30 to 08:30 during BST)
 
 Custom periods can be configured for specific times if required:
 + Custom: charging from 02:00 to 05:00, no off-peak or peak times, forecasts from 22:00 to 23:59
 
 The active tariff is configured by calling 'f.set_tariff() with the name of the tariff to use:
 
 ```
@@ -666,16 +667,18 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.1.8<br>
-Updated charge / discharge profiles for charge_needed() to show power flow in relation to work mode
+2.1.9<br>
+Update get_history() to use GMT or BST when plotting instead of mixed time zones.
+Added 'economy_7' tariff that charges using GMT when clocks change.
+Updated charge / discharge profiles for charge_needed() to show power flow in relation to work mode.
 Better reporting of reason for http error code.
 Template code for get_named_settings() added - not functional in this version due to Open API limitations.
 Update set_pvoutput() to allow push=2.
 Fix problem in set_pvoutput() sending summary to pushover when tou=1.
 Improve accuracy of time of use data in get_pvoutput().
 Improve handling of date / time for queries.
 Comments added to pvoutput data when exported exceeds generated.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.1.8 Summary: library for
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.1.9 Summary: library for
 accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
 quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
@@ -328,15 +328,16 @@
 work mode change to Self Use at 7am and Feed In First at 4pm. + Intelligent
 Octopus: off-peak from 23:30 to 05:30, forecasts from 22:00 to 23:59 + Octopus
 Cosy: off-peak from 04:00 to 07:00 and 13:00 to 16:00, peak from 16:00 to 19:
 00, forecasts from 02:00 to 03:59 and 12:00 to 12:59 + Octopus Go: off peak
 from 00:30 to 04:30, forecasts from 22:00 to 23:59 + Agile Octopus: off-peak
 from 02:30 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59 +
 British Gas Electric Driver: off-peak from 00:00 to 05:00, forecasts from 22:00
-to 23:59 Custom periods can be configured for specific times if required: +
+to 23:59 + Eco 7: Economy 7: off-peak from 00:30 to 07:30 GMT (01:30 to 08:30
+during BST) Custom periods can be configured for specific times if required: +
 Custom: charging from 02:00 to 05:00, no off-peak or peak times, forecasts from
 22:00 to 23:59 The active tariff is configured by calling 'f.set_tariff() with
 the name of the tariff to use: ``` f.set_tariff('flux') ``` When Agile Octopus
 is selected, a price based charging period is configured using the 30 minute
 price forecast. For example: ``` f.set_tariff('agile', product, region,
 start_at, end_by, duration, times, forecast_times, work_times, update,
 weighting, time_shift) ``` This gets the latest 30 minute pricing and uses this
@@ -458,17 +459,19 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.1.8
+(verbose) # Version Info 2.1.9
+Update get_history() to use GMT or BST when plotting instead of mixed time
+zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
-relation to work mode Better reporting of reason for http error code. Template
+relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
 of use data in get_pvoutput(). Improve handling of date / time for queries.
 Comments added to pvoutput data when exported exceeds generated. Fixed charge
 times being set incorrectly in set_tariff() when tariff is not Agile or Flux.
 Show inverter model info and flag error in charge_needed() if residual is less
```

### Comparing `foxesscloud-2.1.8/README.md` & `foxesscloud-2.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -440,14 +440,15 @@
 There are a number of different pre-configured tariffs:
 + Octopus Flux: off-peak from 02:00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed work mode change to Self Use at 7am and Feed In First at 4pm.
 + Intelligent Octopus: off-peak from 23:30 to 05:30, forecasts from 22:00 to 23:59
 + Octopus Cosy: off-peak from 04:00 to 07:00 and 13:00 to 16:00, peak from 16:00 to 19:00, forecasts from 02:00 to 03:59 and 12:00 to 12:59
 + Octopus Go: off peak from 00:30 to 04:30, forecasts from 22:00 to 23:59
 + Agile Octopus: off-peak from 02:30 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59
 + British Gas Electric Driver: off-peak from 00:00 to 05:00, forecasts from 22:00 to 23:59
++ Eco 7: Economy 7: off-peak from 00:30 to 07:30 GMT (01:30 to 08:30 during BST)
 
 Custom periods can be configured for specific times if required:
 + Custom: charging from 02:00 to 05:00, no off-peak or peak times, forecasts from 22:00 to 23:59
 
 The active tariff is configured by calling 'f.set_tariff() with the name of the tariff to use:
 
 ```
@@ -652,16 +653,18 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.1.8<br>
-Updated charge / discharge profiles for charge_needed() to show power flow in relation to work mode
+2.1.9<br>
+Update get_history() to use GMT or BST when plotting instead of mixed time zones.
+Added 'economy_7' tariff that charges using GMT when clocks change.
+Updated charge / discharge profiles for charge_needed() to show power flow in relation to work mode.
 Better reporting of reason for http error code.
 Template code for get_named_settings() added - not functional in this version due to Open API limitations.
 Update set_pvoutput() to allow push=2.
 Fix problem in set_pvoutput() sending summary to pushover when tou=1.
 Improve accuracy of time of use data in get_pvoutput().
 Improve handling of date / time for queries.
 Comments added to pvoutput data when exported exceeds generated.
```

#### html2text {}

```diff
@@ -321,15 +321,16 @@
 work mode change to Self Use at 7am and Feed In First at 4pm. + Intelligent
 Octopus: off-peak from 23:30 to 05:30, forecasts from 22:00 to 23:59 + Octopus
 Cosy: off-peak from 04:00 to 07:00 and 13:00 to 16:00, peak from 16:00 to 19:
 00, forecasts from 02:00 to 03:59 and 12:00 to 12:59 + Octopus Go: off peak
 from 00:30 to 04:30, forecasts from 22:00 to 23:59 + Agile Octopus: off-peak
 from 02:30 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59 +
 British Gas Electric Driver: off-peak from 00:00 to 05:00, forecasts from 22:00
-to 23:59 Custom periods can be configured for specific times if required: +
+to 23:59 + Eco 7: Economy 7: off-peak from 00:30 to 07:30 GMT (01:30 to 08:30
+during BST) Custom periods can be configured for specific times if required: +
 Custom: charging from 02:00 to 05:00, no off-peak or peak times, forecasts from
 22:00 to 23:59 The active tariff is configured by calling 'f.set_tariff() with
 the name of the tariff to use: ``` f.set_tariff('flux') ``` When Agile Octopus
 is selected, a price based charging period is configured using the 30 minute
 price forecast. For example: ``` f.set_tariff('agile', product, region,
 start_at, end_by, duration, times, forecast_times, work_times, update,
 weighting, time_shift) ``` This gets the latest 30 minute pricing and uses this
@@ -451,17 +452,19 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.1.8
+(verbose) # Version Info 2.1.9
+Update get_history() to use GMT or BST when plotting instead of mixed time
+zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
-relation to work mode Better reporting of reason for http error code. Template
+relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
 of use data in get_pvoutput(). Improve handling of date / time for queries.
 Comments added to pvoutput data when exported exceeds generated. Fixed charge
 times being set incorrectly in set_tariff() when tariff is not Agile or Flux.
 Show inverter model info and flag error in charge_needed() if residual is less
```

### Comparing `foxesscloud-2.1.8/pyproject.toml` & `foxesscloud-2.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "foxesscloud"
-version = "2.1.8"
+version = "2.1.9"
 authors = [
   {name="Tony Matthews", email="tony@quasair.co.uk"},
 ]
 description = "library for accessing Fox ESS cloud data using Open API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `foxesscloud-2.1.8/src/foxesscloud/foxesscloud.py` & `foxesscloud-2.1.9/src/foxesscloud/foxesscloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud
-Updated:  28 March 2024
+Updated:  01 April 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud web site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2023
 ##################################################################################################
 
-version = "1.3.0"
+version = "1.3.1"
 print(f"FoxESS-Cloud version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -419,15 +419,15 @@
 device_list = None
 device = None
 device_id = None
 device_sn = None
 raw_vars = None
 
 def get_device(sn=None):
-    global token, device_list, device, device_id, device_sn, firmware, battery, raw_vars, debug_setting, messages, flag, schedule, templates
+    global token, device_list, device, device_id, device_sn, firmware, battery, raw_vars, debug_setting, messages, flag, schedule, templates, remote_settings
     if get_token() is None:
         return None
     if device is not None:
         if sn is None:
             return device
         if device_sn[:len(sn)].upper() == sn.upper():
             return device
@@ -471,15 +471,15 @@
     device_sn = device.get('deviceSN')
     battery = None
     battery_settings = None
     schedule = None
     templates = None
     raw_vars = get_vars()
     firmware = get_firmware()
-    device['key'] = firmware.get('key') if firmware is not None else None
+    remote_settings = get_ui()
     # parse the model code to work out attributes
     model_code = device['deviceType'].upper()
     # first 2 letters / numbers e.g. H1, H3, KH
     if model_code[:2] == 'KH':
         model_code = 'KH-' + model_code[2:]
     elif model_code[:4] == 'AIO-':
         model_code = 'AIO' + model_code[4:]
@@ -559,19 +559,14 @@
         errno = response.json().get('errno')
         output(f"** get_firmware(), no result data, {errno_message(errno)}")
         return None
     firmware = result.get('softVersion')
     if firmware is None:
         output(f"** no firmware data")
         return None
-    protocol = result.get('protocolVersion')
-    firmware['protocol'] = protocol
-    if protocol is not None:
-        part = protocol.split('.')
-        firmware['key'] = part[0].lower() + part[1] if len(part) >= 2 else None
     return firmware
 
 ##################################################################################################
 # get battery info and save to battery
 ##################################################################################################
 
 battery = None
@@ -784,32 +779,98 @@
     get_min()
     return battery_settings
 
 ##################################################################################################
 # get remote settings
 ##################################################################################################
 
-# ui is locked for end user
+remote_settings = None              # raw UI info
+named_settings = None               # processed UI info
+merge_settings = {                  # keys to add
+    'WorkMode': {'keys': {
+        'h115__': 'operation_mode__work_mode',
+        'h116__': 'operation_mode__work_mode',
+        },
+        'values': ['SelfUse', 'Feedin', 'Backup']},
+    'BatteryVolt': {'keys': {
+        'h115__': ['h115__14', 'h115__15', 'h115__16'],
+        'h116__': ['h116__15', 'h116__16', 'h116__17'],
+        },
+        'type': 'list',
+        'valueType': 'float',
+        'unit': 'V'},
+    'BatteryTemp': {'keys': {
+        'h115__': 'h115__17',
+        'h116__': 'h116__18',
+        },
+        'type': 'list',
+        'valueType': 'int',
+        'unit': '℃'},
+}
+
 def get_ui():
-    global token, device_id, debug_setting, messages
+    global device_id, debug_setting, messages, remote_settings, named_settings, merge_settings
     if get_device() is None:
         return None
-    if debug_setting > 1:
-        output(f"getting ui settings")
-    params = {'deviceID': device_id}
-    response = signed_get(path="/c/v0/device/setting/ui", params=params)
-    if response.status_code != 200:
-        output(f"** get_ui() got response code {response.status_code}: {response.reason}")
-        return None
-    result = response.json().get('result')
-    if result is None:
-        errno = response.json().get('errno')
-        output(f"** get_ui(), no result data, {errno_message(errno)}")
-        return None
-    return result
+    if remote_settings is None:
+        if debug_setting > 1:
+            output(f"getting ui settings")
+        params = {'id': device_id}
+        response = signed_get(path="/generic/v0/device/setting/ui", params=params)
+        if response.status_code != 200:
+            output(f"** get_ui() got response code {response.status_code}: {response.reason}")
+            return None
+        result = response.json().get('result')
+        if result is None:
+            errno = response.json().get('errno')
+            output(f"** get_ui(), no result data, {errno_message(errno)}")
+            return None
+        remote_settings = result
+        protocol = remote_settings['protocol'].lower().replace('xx','__')
+        named_settings = {'_protocol': protocol}
+        volt_n = 0
+        volt_keys = []
+        for p in remote_settings['parameters']:
+            if p['name'][:11] == 'BatteryVolt':    # merge BatteryVolts
+                volt_n += 1
+                volt_keys.append(p['key'])
+                if volt_n == 3:
+                    named_settings['BatteryVolt'] = {'key': volt_keys, 'type': 'list', 'valueType': 'float', 'unit': p['properties'][0]['unit']}
+                elif volt_n > 3:
+                    print(f"** get_ui(): more than 3 groups found for BatteryVolt")
+            elif p['name'][:11] == 'BatteryTemp':
+                named_settings['BatteryTemp'] = {'key': p['key'], 'type': 'list', 'valueType': 'int', 'unit': p['properties'][0]['unit']}
+            else:
+                items = []
+                block = p['block'] and len(p['properties']) > 1
+                for e in p['properties']:
+                    valueType = e['elemType']['valueType']
+                    item = {'name': e['key'].replace(protocol,'')} if block else {'key': e['key']} #, 'group': p['name']}
+                    if e['elemType'].get('uiItems') is not None:
+                        item['values'] = e['elemType']['uiItems']
+                    elif e.get('range') is not None:
+                        item['range'] = e['range']
+                        item['valueType'] = 'float' if type(e['range']['hi']) is float else 'int'
+                    else:
+                        item['type'] = valueType
+                    if e.get('unit') is not None and len(e['unit']) > 0:
+                        item['unit'] = e['unit']
+                    if block:
+                        items.append(item)
+                    else:
+                        named_settings[e['name']] = item
+                if block:
+                    named_settings[p['name']] = {'key': p['key'], 'type': 'block', 'items': items}
+        for name in merge_settings.keys():
+            if named_settings.get(name) is None and merge_settings[name]['keys'].get(protocol) is not None:
+                named_settings[name] = {'keys': merge_settings[name]['keys'][protocol]}
+                for k in merge_settings[name].keys():
+                    if k != 'keys':
+                        named_settings[name][k] = merge_settings[name][k]
+    return remote_settings
 
 def get_remote_settings(key):
     global token, device_id, debug_setting, messages
     if get_device() is None:
         return None
     if debug_setting > 1:
         output(f"getting remote settings")
@@ -836,112 +897,68 @@
         return None
     values = result.get('values')
     if values is None:
         output(f"** get_remote_settings(), no values data")
         return None
     return values
 
-# table of protocol specific keys for different named settings
-named_settings = {
-    'cell_volts': {'convert': 'float', 'units': 'V', 'rw': False,
-        'h115': ['h115__14', 'h115__15', 'h115__16'],
-        'h116': ['h116__15', 'h116__16', 'h116__17']},
-    'cell_temps': {'convert': 'float', 'units': '°C', 'rw': False,
-        'h115': 'h115__17',
-        'h116': 'h116__18'},
-    'work_mode': {'rw': True,
-        'h115': 'operation_mode__work_mode',
-        'h116': 'operation_mode__work_mode'},
-    'max_soc': {'convert': 'int', 'units': '%', 'rw': True,
-        'h116': 'h116__basic2__03'},
-    'export_limit': {'convert': 'int', 'units': 'W', 'rw': True,
-        'h116': 'h116__basic2__05'}
-}
-
-def get_keys(name):
-    global device, named_settings
-    info = named_settings.get(name)
-    if info is None:
-        output(f"** get_keys() unknown setting name {name}")
-        return None
-    if get_device() is None:
-        return None
-    protocol = device.get('key')
-    if protocol is None:
-        output(f"** get_keys() no protocol key for device")
-        return None
-    keys = info.get(protocol)
-    if keys is None:
-        output(f"** get_keys() unknown protocol key: {protocol}")
-        return None
-    return keys
-
-
-def get_cell_volts():
-    keys = get_keys('cell_volts')
-    values = get_remote_settings(keys)
-    if values is None:
-        return None
-    cell_volts = []
-    for k in sorted(values.keys()):
-        v = c_float(values[k])
-        if v != 0:
-            cell_volts.append(v)
-    return cell_volts
-
-
-def get_cell_temps():
-    keys = get_keys('cell_temps')
-    values = get_remote_settings(keys)
-    if values is None:
-        return None
-    cell_temps = []
-    for k in sorted(values.keys()):
-        t = c_float(values[k])
-        if t > -50:
-            cell_temps.append(t)
-    return cell_temps
-
-
 def get_named_settings(name):
     global named_settings
-    keys = get_keys(name)
+    if type(name) is list:
+        result = []
+        for n in name:
+            result.append(get_named_settings(n))
+        return result
+    if named_settings is None or named_settings.get(name) is None:
+        output(f"** get_named_settings(): {name} was not recognised")
+        return None
+    keys = named_settings[name].get('keys')
     if keys is None:
         return None
-    values = get_remote_settings(keys)
-    if values is None:
+    result = get_remote_settings(keys)
+    if result is None:
         return None
-    result = []
-    convert = named_settings[name].get('convert')
-    for k in sorted(values.keys()):
-        v = values[k]
-        if convert is None:
-            result.append(v)
-        elif convert == 'int':
-            result.append(c_int(v))
-        elif convert == 'float':
-            result.append(c_float(v))
-        else:
-            result.append(v)
-    if len(result) == 1:
-        return result[0]
+    result_type = named_settings[name].get('type')
+    value_type = named_settings[name].get('valueType')
+    if result_type is None:
+        v = result.get([k for k in result.keys()][0])
+        return v if value_type is None else c_float(v) if value_type == 'float' else c_int(v)
+    if result_type == 'list':
+        values = []
+        for k in sorted(result.keys()):
+            values.append(result[k] if value_type is None else c_float(result[k]) if value_type == 'float' else c_int(result[k]))
+        return values
     return result
 
-
 ##################################################################################################
-# get work mode
+# wrappers for named settings
 ##################################################################################################
 
 work_mode = None
 
 def get_work_mode():
     global work_mode
-    work_mode = get_named_settings('work_mode')
+    if get_device() is None:
+        return None
+    work_mode = get_named_settings('WorkMode')
     return work_mode
 
+def get_cell_volts():
+    values = get_named_settings('BatteryVolt')
+    if values is None:
+        return None
+    return [v for v in values if v > 0]
+
+def get_cell_temps():
+    values = get_named_settings('BatteryTemp')
+    if values is None:
+        return None
+    return [v for v in values if v > -50]
+
+
 ##################################################################################################
 # set work mode
 ##################################################################################################
 
 work_modes = ['SelfUse', 'Feedin', 'Backup', 'ForceCharge', 'ForceDischarge']
 settable_modes = work_modes[:3]
 
@@ -1282,14 +1299,17 @@
     if save is not None:
         file_name = save + "_raw_" + time_span + "_" + d[0:10].replace('-','') + ".txt"
         file = open(file_name, 'w')
         json.dump(result, file, indent=4, ensure_ascii= False)
         file.close()
     for var in result:
         var['date'] = d[0:10]
+        # remove 1 hour over-run when clocks go forward 1 hour
+        while len(var['data']) > 0 and var['data'][-1]['time'][0:10] != d[0:10]:
+            var['data'].pop()
     if 'meterPower2' in v and invert_ct2 == 1:
         ct2_index = v.index('meterPower2')
         for y in result[ct2_index]['data']:
             y['value'] = - y['value']
     if summary <= 0 or time_span == 'hour':
         if summary == -1:     # return last value only for each variable
             for v in result:
@@ -1385,15 +1405,15 @@
             del var['data']
     if plot > 0 and summary < 2:
         plot_raw(result, plot, station)
     return result
 
 # plot raw results data
 def plot_raw(result, plot=1, station=0):
-    global site, device_sn, legend_location
+    global site, device_sn, legend_location, sample_time
     if result is None:
         return
     # work out what we have
     units = []
     vars = []
     dates = []
     for v in result:
@@ -1407,52 +1427,41 @@
     dates = sorted(dates)
     if len(vars) == 0 or len(dates) == 0:
         return
     # plot variables by date with the same units on the same charts
     for unit in units:
         lines = 0
         for d in dates:
-            # get time labels for X axix
+            # get time labels for X axis
             if lines == 0:
-                labels = []
-                for v in [v for v in result if v['unit'] == unit and v['date'] == d]:
-                    h = 0
-                    i = 0
-                    while h < 24:
-                        h = int(v['data'][i]['time'][11:13]) if i < len(v['data']) else h + 1
-                        labels.append(f"{h:02d}:00")
-                        i += 12
-                    break
                 plt.figure(figsize=(figure_width, figure_width/3))
-                plt.xticks(ticks=range(0, len(labels)), labels=labels, rotation=90, fontsize=8)
-                plt.xlim(-1, len(labels))
+                all_x = []
             for v in [v for v in result if v['unit'] == unit and v['date'] == d]:
                 n = len(v['data'])
-                x =[]
-                h = 0
-                old_minute = 0
-                for i in range(0,n):
-                    new_minute = int(v['data'][i]['time'][14:16])
-                    h += 1 if new_minute < old_minute else 0
-                    x.append(h + new_minute / 60)
-                    old_minute = new_minute
+                x = [time_hours(v['data'][i]['time'][11:]) for i in range(0,n)]
+                all_x += x
                 y = [v['data'][i]['value'] if v['data'][i]['value'] is not None else 0.0 for i in range(0, n)]
                 name = v['name']
                 label = f"{name} / {d}" if plot == 2 and len(dates) > 1 else name
                 plt.plot(x, y ,label=label)
                 lines += 1
             if lines >= 1 and (plot == 1 or d == dates[-1]) :
+                bst = 1 if  min(all_x) < 0 else 0
+                labels = [f"{h:02d}:00" for h in range(0, 25)]
+                plt.xticks(ticks=range(0 - bst, 25 - bst), labels=labels, rotation=90, fontsize=8)
+                plt.xlim(-1 - bst, 25)
                 if lines > 1:
                     plt.legend(fontsize=6, loc=legend_location)
                 title = ""
                 if plot == 1 or len(dates) == 1 or lines == 1:
                     title = f"{d} / "
                 if len(vars) == 1 or lines == 1:
                     title = f"{name} / {title}"
                 title = f"{title}{unit} / {site['name'] if station == 1 else device_sn}"
+                title += '' if bst == 0 else ' (BST)'
                 plt.title(title, fontsize=12)
                 plt.grid()
                 plot_show()
                 lines = 0
     return
 
 ##################################################################################################
@@ -1464,15 +1473,15 @@
 # summary = 0, 1, 2: do a quick total energy report for a day
 # save = "xxxxx": save the report results to xxxxx_raw_<time_span>_<d>.json
 # load = "<file>": load the report results from <file>
 # plot = 0: no plot, 1 = plot variables separately, 2 = combine variables
 # station = 0: use device_id, 1 = use station_id
 ##################################################################################################
 
-report_vars = ['solar', 'input','generation', 'feedin', 'loads', 'gridConsumption', 'chargeEnergyToTal', 'dischargeEnergyToTal']
+report_vars = ['yield', 'input','generation', 'feedin', 'loads', 'gridConsumption', 'chargeEnergyToTal', 'dischargeEnergyToTal']
 report_names = ['PV Yield', 'Input', 'Generation', 'Grid Export', 'Consumption', 'Grid Import', 'Battery Charge', 'Battery Discharge']
 
 # fix power values after fox corrupts high word of 32-bit energy total
 fix_values = 1
 fix_value_threshold = 200000000.0
 fix_value_mask = 0x0000FFFF
 
@@ -1766,19 +1775,21 @@
 
 # convert time string HH:MM:SS to decimal hours
 def time_hours(t, d = None):
     if t is None:
         t = d
     if type(t) is float:
         return t
-    elif type(t) is int:
+    if type(t) is int:
         return float(t)
-    elif type(t) is str and t.replace(':', '').isnumeric() and t.count(':') <= 2:
+    offset = 1 if 'BST' in t else 0
+    t = t[0:8]
+    if type(t) is str and t.replace(':', '').isnumeric() and t.count(':') <= 2:
         t += ':00' if t.count(':') == 1 else ''
-        return sum(float(t) / x for x, t in zip([1, 60, 3600], t.split(":")))
+        return sum(float(t) / x for x, t in zip([1, 60, 3600], t.split(":"))) - offset
     output(f"** invalid time string {t}")
     return None
 
 # convert decimal hours to time string HH:MM:SS
 def hours_time(h, ss = False, day = False, mm = True):
     if h is None:
         return "None"
@@ -1926,24 +1937,34 @@
     'off_peak1': {'start': 0.0, 'end': 5.0, 'force': 1},
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},
     'peak': {'start': 0.0, 'end': 0.0 },
     'peak2': {'start': 0.0, 'end': 0.0 },
     'forecast_times': [22, 23]
     }
 
+# time periods for Economy 7
+economy_7 = {
+    'name': 'Eco 7',
+    'off_peak1': {'start': 0.5, 'end': 7.5, 'force': 1, 'gmt': 1},
+    'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},
+    'peak': {'start': 0.0, 'end': 0.0 },
+    'peak2': {'start': 0.0, 'end': 0.0 },
+    'forecast_times': [22, 23]
+    }
+
 # custom time periods / template
 custom_periods = {'name': 'Custom',
     'off_peak1': {'start': 2.0, 'end': 5.0, 'force': 1},
     'off_peak2': {'start': 15.0, 'end': 16.0, 'force': 0},
     'peak': {'start': 16.0, 'end': 19.0 },
     'peak2': {'start': 0.0, 'end': 0.0 },
     'forecast_times': [22, 23]
     }
 
-tariff_list = [octopus_flux, intelligent_octopus, octopus_cosy, octopus_go, agile_octopus, bg_driver, custom_periods]
+tariff_list = [octopus_flux, intelligent_octopus, octopus_cosy, octopus_go, agile_octopus, bg_driver, economy_7, custom_periods]
 tariff = octopus_flux
 
 ##################################################################################################
 # Octopus Energy Agile Price
 ##################################################################################################
 
 # base settings
@@ -2115,21 +2136,23 @@
     start_at = time_hours(period.get('start'), tariff['off_peak1']['start'])
     end_by = time_hours(period.get('end'), tariff['off_peak1']['end'])
     duration = 3 if period.get('duration') is None else period['duration']
     charge_pm = start_at >= tariff_config['pm_start'] and end_by < tariff_config['am_start']
     am_pm = 'PM' if charge_pm else 'AM'
     start = start_at if duration > 0 else 0.0
     end = end_by if duration > 0 else 0.0
+    gmt = ''
     if charge_pm:
         tariff['off_peak2']['start'] = start
         tariff['off_peak2']['end'] = end
     else:
         tariff['off_peak1']['start'] = start
         tariff['off_peak1']['end'] = end
-    print(f"\n{tariff['name']} {am_pm} charging period: {hours_time(start)} to {hours_time(end)}")
+        gmt = ' GMT' if tariff['off_peak1'].get('gmt') is not None else ''
+    print(f"\n{tariff['name']} {am_pm} charging period: {hours_time(start)} to {hours_time(end)}{gmt}")
     return 1
 
 # set tariff and AM/PM charge time period
 def set_tariff(find, update=1, start_at=None, end_by=None, duration=None, times=None, forecast_times=None, work_times=None, d=None, **settings):
     global debug_setting, agile_octopus, tariff, tariff_list
     print(f"\n---------------- set_tariff -----------------")
     # validate parameters
@@ -2388,14 +2411,18 @@
     if hour_adjustment != 0:    # change happens in the next 2 days - work out if today, tomorrow or day after tomorrow
         change_hour = 1 if daylight_changes(system_time, f"{tomorrow} 00:00") != 0 else 25 if daylight_changes(f"{tomorrow} 00:00", f"{day_after_tomorrow} 00:00") != 0 else 49
         change_hour += 1 if hour_adjustment > 0 else 0
     # get next charge times from am/pm charge times
     force_charge = 0 if force_charge is None else force_charge
     start_am = time_hours(tariff['off_peak1']['start'] if tariff is not None else 2.0)
     end_am = time_hours(tariff['off_peak1']['end'] if tariff is not None else 5.0)
+    # adjust charge times for Economy 7 in BST
+    if time_offset > 0 and tariff is not None and tariff['off_peak1'].get('gmt') is not None:
+        start_am += 1
+        end_am += 1
     force_charge_am = 0 if tariff is not None and tariff['off_peak1']['force'] == 0 or force_charge == 0 else force_charge
     time_to_am = round_time(start_am - base_hour)
     start_pm = time_hours(tariff['off_peak2']['start'] if tariff is not None else 0.0)
     end_pm = time_hours(tariff['off_peak2']['end'] if tariff is not None else 0.0)
     force_charge_pm = 0 if tariff is not None and tariff['off_peak2']['force'] == 0 or force_charge == 0 else 1
     time_to_pm = round_time(start_pm - base_hour) if start_pm > 0 else None
     no_go1 = time_to_am is not None and hour_in(hour_now, {'start': round_time(start_am - 0.25), 'end': round_time(end_am + 0.25)})
@@ -2542,15 +2569,16 @@
     print(f"  Model:     {model}")
     print(f"  Rating:    {device_power:.2f}kW")
     print(f"  Export:    {export_power:.2f}kW")
     print(f"  Charge:    {charge_current:.1f}A, {charge_limit:.2f}kW, {charge_loss * 100:.1f}% efficient")
     print(f"  Discharge: {discharge_current:.1f}A, {discharge_limit:.2f}kW, {discharge_loss * 100:.1f}% efficient")
     print(f"  Inverter:  {inverter_power:.0f}W power consumption")
     print(f"  BMS:       {bms_power:.0f}W power consumption")
-    print(f"  Work Mode: {current_mode}")
+    if current_mode is not None:
+        print(f"  Work Mode: {current_mode}")
     # get consumption data
     annual_consumption = charge_config['annual_consumption']
     if annual_consumption is not None:
         consumption = annual_consumption / 365 * seasonality[now.month - 1] / sum(seasonality) * 12
         consumption_by_hour = daily_consumption
         print(f"\nEstimated consumption: {consumption:.1f}kWh")
     else:
```

### Comparing `foxesscloud-2.1.8/src/foxesscloud/openapi.py` & `foxesscloud-2.1.9/src/foxesscloud/openapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud using Open API
-Updated:  28 March 2024
+Updated:  01 April 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud api site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2024
 ##################################################################################################
 
-version = "2.1.8"
+version = "2.1.9"
 print(f"FoxESS-Cloud Open API version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -400,15 +400,15 @@
 ##################################################################################################
 
 device_list = None
 device = None
 device_sn = None
 
 def get_device(sn=None):
-    global device_list, device, device_sn, battery, debug_setting, schedule
+    global device_list, device, device_sn, battery, debug_setting, schedule, remote_settings
     if get_vars() is None:
         return None
     if device is not None:
         if sn is None:
             return device
         if device_sn[:len(sn)].upper() == sn.upper():
             return device
@@ -457,15 +457,15 @@
         output(f"** get_device(), no detail result data, {errno_message(response)}")
         return None
     device = result
     battery = None
     battery_settings = None
     schedule = None
     get_generation()
-    device['key'] = None
+#    remote_settings = get_ui()
     # parse the model code to work out attributes
     model_code = device['deviceType'].upper()
     # first 2 letters / numbers e.g. H1, H3, KH
     if model_code[:2] == 'KH':
         model_code = 'KH-' + model_code[2:]
     elif model_code[:4] == 'AIO-':
         model_code = 'AIO' + model_code[4:]
@@ -515,15 +515,14 @@
     if result is None:
         output(f"** get_generation(), no result data, {errno_message(response)}")
         return None
     if result.get('today') is None:
         result['today'] = 0.0
     if update == 1:
         device['generationToday'] = result['today']
-        device['generationMonth'] = result['month']
         device['generationTotal'] = result['cumulative'] 
     return result
 
 ##################################################################################################
 # get battery info and save to battery
 ##################################################################################################
 
@@ -737,31 +736,98 @@
     get_min()
     return battery_settings
 
 ##################################################################################################
 # get remote settings
 ##################################################################################################
 
-# ui is locked for end user
+remote_settings = None              # raw UI info
+named_settings = None               # processed UI info
+merge_settings = {                  # keys to add
+    'WorkMode': {'keys': {
+        'h115__': 'operation_mode__work_mode',
+        'h116__': 'operation_mode__work_mode',
+        },
+        'values': ['SelfUse', 'Feedin', 'Backup']},
+    'BatteryVolt': {'keys': {
+        'h115__': ['h115__14', 'h115__15', 'h115__16'],
+        'h116__': ['h116__15', 'h116__16', 'h116__17'],
+        },
+        'type': 'list',
+        'valueType': 'float',
+        'unit': 'V'},
+    'BatteryTemp': {'keys': {
+        'h115__': 'h115__17',
+        'h116__': 'h116__18',
+        },
+        'type': 'list',
+        'valueType': 'int',
+        'unit': '℃'},
+}
+
 def get_ui():
-    global token, device_id, debug_setting, messages
+    global device_id, debug_setting, messages, remote_settings, named_settings, merge_settings
     if get_device() is None:
         return None
-    if debug_setting > 1:
-        output(f"getting ui settings")
-    params = {'deviceID': device_id}
-    response = signed_get(path="/op/v0/device/setting/ui", params=params)
-    if response.status_code != 200:
-        output(f"** get_ui() got response code {response.status_code}: {response.reason}")
-        return None
-    result = response.json().get('result')
-    if result is None:
-        output(f"** get_ui(), no result data, {errno_message(response)}")
-        return None
-    return result
+    if remote_settings is None:
+        if debug_setting > 1:
+            output(f"getting ui settings")
+        params = {'id': device_id}
+        response = signed_get(path="/generic/v0/device/setting/ui", params=params)
+        if response.status_code != 200:
+            output(f"** get_ui() got response code {response.status_code}: {response.reason}")
+            return None
+        result = response.json().get('result')
+        if result is None:
+            errno = response.json().get('errno')
+            output(f"** get_ui(), no result data, {errno_message(errno)}")
+            return None
+        remote_settings = result
+        protocol = remote_settings['protocol'].lower().replace('xx','__')
+        named_settings = {'_protocol': protocol}
+        volt_n = 0
+        volt_keys = []
+        for p in remote_settings['parameters']:
+            if p['name'][:11] == 'BatteryVolt':    # merge BatteryVolts
+                volt_n += 1
+                volt_keys.append(p['key'])
+                if volt_n == 3:
+                    named_settings['BatteryVolt'] = {'key': volt_keys, 'type': 'list', 'valueType': 'float', 'unit': p['properties'][0]['unit']}
+                elif volt_n > 3:
+                    print(f"** get_ui(): more than 3 groups found for BatteryVolt")
+            elif p['name'][:11] == 'BatteryTemp':
+                named_settings['BatteryTemp'] = {'key': p['key'], 'type': 'list', 'valueType': 'int', 'unit': p['properties'][0]['unit']}
+            else:
+                items = []
+                block = p['block'] and len(p['properties']) > 1
+                for e in p['properties']:
+                    valueType = e['elemType']['valueType']
+                    item = {'name': e['key'].replace(protocol,'')} if block else {'key': e['key']} #, 'group': p['name']}
+                    if e['elemType'].get('uiItems') is not None:
+                        item['values'] = e['elemType']['uiItems']
+                    elif e.get('range') is not None:
+                        item['range'] = e['range']
+                        item['valueType'] = 'float' if type(e['range']['hi']) is float else 'int'
+                    else:
+                        item['type'] = valueType
+                    if e.get('unit') is not None and len(e['unit']) > 0:
+                        item['unit'] = e['unit']
+                    if block:
+                        items.append(item)
+                    else:
+                        named_settings[e['name']] = item
+                if block:
+                    named_settings[p['name']] = {'key': p['key'], 'type': 'block', 'items': items}
+        for name in merge_settings.keys():
+            if named_settings.get(name) is None and merge_settings[name]['keys'].get(protocol) is not None:
+                named_settings[name] = {'keys': merge_settings[name]['keys'][protocol]}
+                for k in merge_settings[name].keys():
+                    if k != 'keys':
+                        named_settings[name][k] = merge_settings[name][k]
+    return remote_settings
 
 def get_remote_settings(key):
     global token, device_id, debug_setting, messages
     if get_device() is None:
         return None
     if debug_setting > 1:
         output(f"getting remote settings")
@@ -773,133 +839,100 @@
             v = get_remote_settings(k)
             if v is None:
                 return
             for x in v.keys():
                 values[x] = v[x]
         return values
     params = {'id': device_id, 'hasVersionHead': 1, 'key': key}
-    response = signed_get(path="/op/v0/device/setting/get", params=params)
+    response = signed_get(path="/c/v0/device/setting/get", params=params)
     if response.status_code != 200:
         output(f"** get_remote_settings() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
-        output(f"** get_remote_settings(), no result data, {errno_message(response)}")
+        errno = response.json().get('errno')
+        output(f"** get_remote_settings(), no result data, {errno_message(errno)}")
         return None
     values = result.get('values')
     if values is None:
         output(f"** get_remote_settings(), no values data")
         return None
     return values
 
-# table of protocol specific keys for different settings
-named_settings = {
-    'cell_volts': {'convert': 'float', 'units': 'V', 'rw': False,
-        'h115': ['h115__14', 'h115__15', 'h115__16'],
-        'h116': ['h116__15', 'h116__16', 'h116__17']},
-    'cell_temps': {'convert': 'float', 'units': '°C', 'rw': False,
-        'h115': 'h115__17',
-        'h116': 'h116__18'},
-    'work_mode': {'rw': True,
-        'h115': 'operation_mode__work_mode',
-        'h116': 'operation_mode__work_mode'},
-    'max_soc': {'convert': 'int', 'units': '%', 'rw': True,
-        'h116': 'h116__basic2__03'},
-    'export_limit': {'convert': 'int', 'units': 'W', 'rw': True,
-        'h116': 'h116__basic2__05'}
-}
-
-def get_keys(name):
-    global device, named_settings
-    info = named_settings.get(name)
-    if info is None:
-        output(f"** get_keys() unknown setting name {name}")
-        return None
-    if get_device() is None:
-        return None
-    protocol = device.get('key')
-    if protocol is None:
-        output(f"** get_keys() no protocol key for device")
-        return None
-    keys = info.get(protocol)
-    if keys is None:
-        output(f"** get_keys() unknown protocol key: {protocol}")
-        return None
-    return keys
-
-def get_cell_volts():
-    keys = get_keys('cell_volts')
-    values = get_remote_settings(keys)
-    if values is None:
-        return None
-    cell_volts = []
-    for k in sorted(values.keys()):
-        v = c_float(values[k])
-        if v != 0:
-            cell_volts.append(v)
-    return cell_volts
-
-def get_cell_temps():
-    keys = get_keys('cell_temps')
-    values = get_remote_settings(keys)
-    if values is None:
-        return None
-    cell_temps = []
-    for k in sorted(values.keys()):
-        t = c_float(values[k])
-        if t > -50:
-            cell_temps.append(t)
-    return cell_temps
-
 def get_named_settings(name):
     global named_settings
-    keys = get_keys(name)
+    if type(name) is list:
+        result = []
+        for n in name:
+            result.append(get_named_settings(n))
+        return result
+    if named_settings is None or named_settings.get(name) is None:
+        output(f"** get_named_settings(): {name} was not recognised")
+        return None
+    keys = named_settings[name].get('keys')
     if keys is None:
         return None
-    values = get_remote_settings(keys)
-    if values is None:
+    result = get_remote_settings(keys)
+    if result is None:
         return None
-    result = []
-    convert = named_settings[name].get('convert')
-    for k in sorted(values.keys()):
-        v = values[k]
-        if convert is None:
-            result.append(v)
-        elif convert == 'int':
-            result.append(c_int(v))
-        elif convert == 'float':
-            result.append(c_float(v))
-        else:
-            result.append(v)
-    if len(result) == 1:
-        return result[0]
+    result_type = named_settings[name].get('type')
+    value_type = named_settings[name].get('valueType')
+    if result_type is None:
+        v = result.get([k for k in result.keys()][0])
+        return v if value_type is None else c_float(v) if value_type == 'float' else c_int(v)
+    if result_type == 'list':
+        values = []
+        for k in sorted(result.keys()):
+            values.append(result[k] if value_type is None else c_float(result[k]) if value_type == 'float' else c_int(result[k]))
+        return values
     return result
 
 ##################################################################################################
-# get work mode
+# wrappers for named settings
 ##################################################################################################
 
 work_mode = None
 
 def get_work_mode():
     global work_mode
-    ## settings not available
+#    print(f"** get_work_mode(): not available via Open API")
     return None
-    work_mode = get_named_settings('work_mode')
+    if get_device() is None:
+        return None
+    work_mode = get_named_settings('WorkMode')
     return work_mode
 
+def get_cell_volts():
+    print(f"** get_cell_volts(): not available via Open API")
+    return None
+    values = get_named_settings('BatteryVolt')
+    if values is None:
+        return None
+    return [v for v in values if v > 0]
+
+def get_cell_temps():
+    print(f"** get_cell_temps(): not available via Open API")
+    return None
+    values = get_named_settings('BatteryTemp')
+    if values is None:
+        return None
+    return [v for v in values if v > -50]
+
+
 ##################################################################################################
 # set work mode
 ##################################################################################################
 
 work_modes = ['SelfUse', 'Feedin', 'Backup', 'ForceCharge', 'ForceDischarge']
 settable_modes = work_modes[:3]
 
 def set_work_mode(mode, force = 0):
     global token, device_sn, work_modes, work_mode, debug_setting
+    printf("** set_work_mode(): not available via Open API")
+    return None
     if get_device() is None:
         return None
     if mode not in settable_modes:
         output(f"** work mode: must be one of {settable_modes}")
         return None
     if get_schedule().get('enable'):
         if force == 0:
@@ -1172,14 +1205,17 @@
     if save is not None:
         file_name = save + "_history_" + time_span + "_" + d[0:10].replace('-','') + ".txt"
         file = open(file_name, 'w')
         json.dump(result, file, indent=4, ensure_ascii= False)
         file.close()
     for var in result:
         var['date'] = d[0:10]
+        # remove 1 hour over-run when clocks go forward 1 hour
+        while len(var['data']) > 0 and var['data'][-1]['time'][0:10] != d[0:10]:
+            var['data'].pop()
         if var.get('variable') == 'meterPower2' and invert_ct2 == 1:
             for y in var['data']:
                 y['value'] = -y['value']
         elif var['variable'] == 'ResidualEnergy':
             var['unit'] = 'kWh'
             for y in var['data']:
                  y['value'] *= residual_scale
@@ -1273,15 +1309,15 @@
             del var['data']
     if plot > 0 and summary < 2:
         plot_history(result, plot)
     return result
 
 # plot raw results data
 def plot_history(result, plot=1):
-    global site, device_sn, legend_location
+    global site, device_sn, legend_location, sample_time
     if result is None:
         return
     # work out what we have
     units = []
     vars = []
     dates = []
     for v in result:
@@ -1297,50 +1333,39 @@
         return
     # plot variables by date with the same units on the same charts
     for unit in units:
         lines = 0
         for d in dates:
             # get time labels for X axix
             if lines == 0:
-                labels = []
-                for v in [v for v in result if v['unit'] == unit and v['date'] == d]:
-                    h = 0
-                    i = 0
-                    while h < 24:
-                        h = int(v['data'][i]['time'][11:13]) if i < len(v['data']) else h + 1
-                        labels.append(f"{h:02d}:00")
-                        i += 12
-                    break
                 plt.figure(figsize=(figure_width, figure_width/3))
-                plt.xticks(ticks=range(0, len(labels)), labels=labels, rotation=90, fontsize=8)
-                plt.xlim(-1, len(labels))
+                all_x = []
             for v in [v for v in result if v['unit'] == unit and v['date'] == d]:
                 n = len(v['data'])
-                x =[]
-                h = 0
-                old_minute = 0
-                for i in range(0,n):
-                    new_minute = int(v['data'][i]['time'][14:16])
-                    h += 1 if new_minute < old_minute else 0
-                    x.append(h + new_minute / 60)
-                    old_minute = new_minute
+                x = [time_hours(v['data'][i]['time'][11:]) for i in range(0,n)]
+                all_x += x
                 y = [v['data'][i]['value'] if v['data'][i]['value'] is not None else 0.0 for i in range(0, n)]
                 name = v['name']
                 label = f"{name} / {d}" if plot == 2 and len(dates) > 1 else name
                 plt.plot(x, y ,label=label)
                 lines += 1
             if lines >= 1 and (plot == 1 or d == dates[-1]) :
+                bst = 1 if min(all_x) < 0 else 0
+                labels = [f"{h:02d}:00" for h in range(0, 25)]
+                plt.xticks(ticks=range(0 - bst, 25 - bst), labels=labels, rotation=90, fontsize=8)
+                plt.xlim(-1 - bst, 25 - bst)
                 if lines > 1:
                     plt.legend(fontsize=6, loc=legend_location)
                 title = ""
                 if plot == 1 or len(dates) == 1 or lines == 1:
                     title = f"{d} / "
                 if len(vars) == 1 or lines == 1:
                     title = f"{name} / {title}"
                 title = f"{title}{unit} / {device_sn}"
+                title += '' if bst == 0 else ' (BST)'
                 plt.title(title, fontsize=12)
                 plt.grid()
                 plot_show()
                 lines = 0
     return
 
 ##################################################################################################
@@ -1623,19 +1648,21 @@
 
 # convert time string HH:MM:SS to decimal hours
 def time_hours(t, d = None):
     if t is None:
         t = d
     if type(t) is float:
         return t
-    elif type(t) is int:
+    if type(t) is int:
         return float(t)
-    elif type(t) is str and t.replace(':', '').isnumeric() and t.count(':') <= 2:
+    offset = 1 if 'BST' in t else 0
+    t = t[0:8]
+    if type(t) is str and t.replace(':', '').isnumeric() and t.count(':') <= 2:
         t += ':00' if t.count(':') == 1 else ''
-        return sum(float(t) / x for x, t in zip([1, 60, 3600], t.split(":")))
+        return sum(float(t) / x for x, t in zip([1, 60, 3600], t.split(":"))) - offset
     output(f"** invalid time string {t}")
     return None
 
 # convert decimal hours to time string HH:MM:SS
 def hours_time(h, ss = False, day = False, mm = True):
     if h is None:
         return "None"
@@ -1783,24 +1810,34 @@
     'off_peak1': {'start': 0.0, 'end': 5.0, 'force': 1},
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},
     'peak': {'start': 0.0, 'end': 0.0 },
     'peak2': {'start': 0.0, 'end': 0.0 },
     'forecast_times': [22, 23]
     }
 
+# time periods for Economy 7
+economy_7 = {
+    'name': 'Eco 7',
+    'off_peak1': {'start': 0.5, 'end': 7.5, 'force': 1, 'gmt': 1},
+    'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},
+    'peak': {'start': 0.0, 'end': 0.0 },
+    'peak2': {'start': 0.0, 'end': 0.0 },
+    'forecast_times': [22, 23]
+    }
+
 # custom time periods / template
 custom_periods = {'name': 'Custom',
     'off_peak1': {'start': 2.0, 'end': 5.0, 'force': 1},
     'off_peak2': {'start': 15.0, 'end': 16.0, 'force': 0},
     'peak': {'start': 16.0, 'end': 19.0 },
     'peak2': {'start': 0.0, 'end': 0.0 },
     'forecast_times': [22, 23]
     }
 
-tariff_list = [octopus_flux, intelligent_octopus, octopus_cosy, octopus_go, agile_octopus, bg_driver, custom_periods]
+tariff_list = [octopus_flux, intelligent_octopus, octopus_cosy, octopus_go, agile_octopus, bg_driver, economy_7, custom_periods]
 tariff = octopus_flux
 
 ##################################################################################################
 # Octopus Energy Agile Price
 ##################################################################################################
 
 # base settings
@@ -1972,21 +2009,23 @@
     start_at = time_hours(period.get('start'), tariff['off_peak1']['start'])
     end_by = time_hours(period.get('end'), tariff['off_peak1']['end'])
     duration = 3 if period.get('duration') is None else period['duration']
     charge_pm = start_at >= tariff_config['pm_start'] and end_by < tariff_config['am_start']
     am_pm = 'PM' if charge_pm else 'AM'
     start = start_at if duration > 0 else 0.0
     end = end_by if duration > 0 else 0.0
+    gmt = ""
     if charge_pm:
         tariff['off_peak2']['start'] = start
         tariff['off_peak2']['end'] = end
     else:
         tariff['off_peak1']['start'] = start
         tariff['off_peak1']['end'] = end
-    print(f"\n{tariff['name']} {am_pm} charging period: {hours_time(start)} to {hours_time(end)}")
+        gmt = " GMT" if tariff['off_peak1'].get('gmt') is not None else ""
+    print(f"\n{tariff['name']} {am_pm} charging period: {hours_time(start)} to {hours_time(end)}{gmt}")
     return 1
 
 # set tariff and AM/PM charge time period
 def set_tariff(find, update=1, start_at=None, end_by=None, duration=None, times=None, forecast_times=None, work_times=None, d=None, **settings):
     global debug_setting, agile_octopus, tariff, tariff_list
     print(f"\n---------------- set_tariff -----------------")
     # validate parameters
@@ -2245,14 +2284,18 @@
     if hour_adjustment != 0:    # change happens in the next 2 days - work out if today, tomorrow or day after tomorrow
         change_hour = 1 if daylight_changes(system_time, f"{tomorrow} 00:00") != 0 else 25 if daylight_changes(f"{tomorrow} 00:00", f"{day_after_tomorrow} 00:00") != 0 else 49
         change_hour += 1 if hour_adjustment > 0 else 0
     # get next charge times from am/pm charge times
     force_charge = 0 if force_charge is None else force_charge
     start_am = time_hours(tariff['off_peak1']['start'] if tariff is not None else 2.0)
     end_am = time_hours(tariff['off_peak1']['end'] if tariff is not None else 5.0)
+    # adjust times for Economy 7 in BST
+    if time_offset > 0 and tariff is not None and tariff['off_peak1'].get('gmt') is not None:
+        start_am += 1
+        end_am += 1
     force_charge_am = 0 if tariff is not None and tariff['off_peak1']['force'] == 0 or force_charge == 0 else force_charge
     time_to_am = round_time(start_am - base_hour)
     start_pm = time_hours(tariff['off_peak2']['start'] if tariff is not None else 0.0)
     end_pm = time_hours(tariff['off_peak2']['end'] if tariff is not None else 0.0)
     force_charge_pm = 0 if tariff is not None and tariff['off_peak2']['force'] == 0 or force_charge == 0 else 1
     time_to_pm = round_time(start_pm - base_hour) if start_pm > 0 else None
     no_go1 = time_to_am is not None and hour_in(hour_now, {'start': round_time(start_am - 0.25), 'end': round_time(end_am + 0.25)})
@@ -2396,15 +2439,16 @@
     print(f"  Model:     {model}")
     print(f"  Rating:    {device_power:.2f}kW")
     print(f"  Export:    {export_power:.2f}kW")
     print(f"  Charge:    {charge_current:.1f}A, {charge_limit:.2f}kW, {charge_loss * 100:.1f}% efficient")
     print(f"  Discharge: {discharge_current:.1f}A, {discharge_limit:.2f}kW, {discharge_loss * 100:.1f}% efficient")
     print(f"  Inverter:  {inverter_power:.0f}W power consumption")
     print(f"  BMS:       {bms_power:.0f}W power consumption")
-    print(f"  Work Mode: {current_mode}")
+    if current_mode is not None:
+        print(f"  Work Mode: {current_mode}")
     # get consumption data
     annual_consumption = charge_config['annual_consumption']
     if annual_consumption is not None:
         consumption = annual_consumption / 365 * seasonality[now.month - 1] / sum(seasonality) * 12
         consumption_by_hour = daily_consumption
         print(f"\nEstimated consumption: {consumption:.1f}kWh")
     else:
```

### Comparing `foxesscloud-2.1.8/src/foxesscloud.egg-info/PKG-INFO` & `foxesscloud-2.1.9/src/foxesscloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxesscloud
-Version: 2.1.8
+Version: 2.1.9
 Summary: library for accessing Fox ESS cloud data using Open API
 Author-email: Tony Matthews <tony@quasair.co.uk>
 Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -454,14 +454,15 @@
 There are a number of different pre-configured tariffs:
 + Octopus Flux: off-peak from 02:00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed work mode change to Self Use at 7am and Feed In First at 4pm.
 + Intelligent Octopus: off-peak from 23:30 to 05:30, forecasts from 22:00 to 23:59
 + Octopus Cosy: off-peak from 04:00 to 07:00 and 13:00 to 16:00, peak from 16:00 to 19:00, forecasts from 02:00 to 03:59 and 12:00 to 12:59
 + Octopus Go: off peak from 00:30 to 04:30, forecasts from 22:00 to 23:59
 + Agile Octopus: off-peak from 02:30 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59
 + British Gas Electric Driver: off-peak from 00:00 to 05:00, forecasts from 22:00 to 23:59
++ Eco 7: Economy 7: off-peak from 00:30 to 07:30 GMT (01:30 to 08:30 during BST)
 
 Custom periods can be configured for specific times if required:
 + Custom: charging from 02:00 to 05:00, no off-peak or peak times, forecasts from 22:00 to 23:59
 
 The active tariff is configured by calling 'f.set_tariff() with the name of the tariff to use:
 
 ```
@@ -666,16 +667,18 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.1.8<br>
-Updated charge / discharge profiles for charge_needed() to show power flow in relation to work mode
+2.1.9<br>
+Update get_history() to use GMT or BST when plotting instead of mixed time zones.
+Added 'economy_7' tariff that charges using GMT when clocks change.
+Updated charge / discharge profiles for charge_needed() to show power flow in relation to work mode.
 Better reporting of reason for http error code.
 Template code for get_named_settings() added - not functional in this version due to Open API limitations.
 Update set_pvoutput() to allow push=2.
 Fix problem in set_pvoutput() sending summary to pushover when tou=1.
 Improve accuracy of time of use data in get_pvoutput().
 Improve handling of date / time for queries.
 Comments added to pvoutput data when exported exceeds generated.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.1.8 Summary: library for
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.1.9 Summary: library for
 accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
 quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
@@ -328,15 +328,16 @@
 work mode change to Self Use at 7am and Feed In First at 4pm. + Intelligent
 Octopus: off-peak from 23:30 to 05:30, forecasts from 22:00 to 23:59 + Octopus
 Cosy: off-peak from 04:00 to 07:00 and 13:00 to 16:00, peak from 16:00 to 19:
 00, forecasts from 02:00 to 03:59 and 12:00 to 12:59 + Octopus Go: off peak
 from 00:30 to 04:30, forecasts from 22:00 to 23:59 + Agile Octopus: off-peak
 from 02:30 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59 +
 British Gas Electric Driver: off-peak from 00:00 to 05:00, forecasts from 22:00
-to 23:59 Custom periods can be configured for specific times if required: +
+to 23:59 + Eco 7: Economy 7: off-peak from 00:30 to 07:30 GMT (01:30 to 08:30
+during BST) Custom periods can be configured for specific times if required: +
 Custom: charging from 02:00 to 05:00, no off-peak or peak times, forecasts from
 22:00 to 23:59 The active tariff is configured by calling 'f.set_tariff() with
 the name of the tariff to use: ``` f.set_tariff('flux') ``` When Agile Octopus
 is selected, a price based charging period is configured using the 30 minute
 price forecast. For example: ``` f.set_tariff('agile', product, region,
 start_at, end_by, duration, times, forecast_times, work_times, update,
 weighting, time_shift) ``` This gets the latest 30 minute pricing and uses this
@@ -458,17 +459,19 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.1.8
+(verbose) # Version Info 2.1.9
+Update get_history() to use GMT or BST when plotting instead of mixed time
+zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
-relation to work mode Better reporting of reason for http error code. Template
+relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
 of use data in get_pvoutput(). Improve handling of date / time for queries.
 Comments added to pvoutput data when exported exceeds generated. Fixed charge
 times being set incorrectly in set_tariff() when tariff is not Agile or Flux.
 Show inverter model info and flag error in charge_needed() if residual is less
```

