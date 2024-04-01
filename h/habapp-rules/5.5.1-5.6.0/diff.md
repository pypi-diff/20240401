# Comparing `tmp/habapp_rules-5.5.1.tar.gz` & `tmp/habapp_rules-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habapp_rules-5.5.1.tar", last modified: Thu Mar  7 13:20:34 2024, max compression
+gzip compressed data, was "habapp_rules-5.6.0.tar", last modified: Sun Mar 24 15:20:35 2024, max compression
```

## Comparing `habapp_rules-5.5.1.tar` & `habapp_rules-5.6.0.tar`

### file list

```diff
@@ -1,56 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:20:34.419117 habapp_rules-5.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-07 13:20:34.419117 habapp_rules-5.5.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:20:34.411117 habapp_rules-5.5.1/habapp_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:20:34.411117 habapp_rules-5.5.1/habapp_rules/actors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/actors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:20:34.411117 habapp_rules-5.5.1/habapp_rules/actors/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/actors/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/actors/config/light.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/actors/config/light_hcl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/actors/config/shading.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/actors/config/ventilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/actors/irrigation.py
--rw-r--r--   0 runner    (1001) docker     (127)    38658 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/actors/light.py
--rw-r--r--   0 runner    (1001) docker     (127)    16197 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/actors/light_hcl.py
--rw-r--r--   0 runner    (1001) docker     (127)    36944 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/actors/shading.py
--rw-r--r--   0 runner    (1001) docker     (127)    19218 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/actors/state_observer.py
--rw-r--r--   0 runner    (1001) docker     (127)    29831 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/actors/ventilation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:20:34.411117 habapp_rules-5.5.1/habapp_rules/bridge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/bridge/knx_mqtt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:20:34.415117 habapp_rules-5.5.1/habapp_rules/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/common/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/common/hysteresis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/common/logic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:20:34.415117 habapp_rules-5.5.1/habapp_rules/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/core/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/core/state_machine_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/core/timeout_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/core/type_of_day.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:20:34.415117 habapp_rules-5.5.1/habapp_rules/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/sensors/astro.py
--rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/sensors/dwd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13218 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/sensors/motion.py
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/sensors/sun.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:20:34.415117 habapp_rules-5.5.1/habapp_rules/system/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/system/presence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11767 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/system/sleep.py
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/habapp_rules/system/summer_winter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:20:34.415117 habapp_rules-5.5.1/habapp_rules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-07 13:20:34.000000 habapp_rules-5.5.1/habapp_rules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-07 13:20:34.000000 habapp_rules-5.5.1/habapp_rules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 13:20:34.000000 habapp_rules-5.5.1/habapp_rules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-07 13:20:34.000000 habapp_rules-5.5.1/habapp_rules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-07 13:20:34.000000 habapp_rules-5.5.1/habapp_rules.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 13:20:34.419117 habapp_rules-5.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-07 13:20:26.000000 habapp_rules-5.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.431302 habapp_rules-5.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-24 15:20:35.431302 habapp_rules-5.6.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.419302 habapp_rules-5.6.0/habapp_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.423302 habapp_rules-5.6.0/habapp_rules/actors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.423302 habapp_rules-5.6.0/habapp_rules/actors/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/config/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/config/light_hcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/config/shading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/config/ventilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/irrigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38658 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16197 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/light_hcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36944 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/shading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19218 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/state_observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29831 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/actors/ventilation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.423302 habapp_rules-5.6.0/habapp_rules/bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/bridge/knx_mqtt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.427302 habapp_rules-5.6.0/habapp_rules/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/common/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/common/hysteresis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/common/logic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.427302 habapp_rules-5.6.0/habapp_rules/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/core/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/core/state_machine_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/core/timeout_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/core/type_of_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.427302 habapp_rules-5.6.0/habapp_rules/energy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/energy/donut_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/energy/monthly_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.427302 habapp_rules-5.6.0/habapp_rules/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/sensors/astro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/sensors/dwd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13218 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/sensors/motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/sensors/sun.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.431302 habapp_rules-5.6.0/habapp_rules/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/system/presence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11767 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/system/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/habapp_rules/system/summer_winter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:20:35.431302 habapp_rules-5.6.0/habapp_rules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-24 15:20:35.000000 habapp_rules-5.6.0/habapp_rules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-24 15:20:35.000000 habapp_rules-5.6.0/habapp_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 15:20:35.000000 habapp_rules-5.6.0/habapp_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-24 15:20:35.000000 habapp_rules-5.6.0/habapp_rules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-24 15:20:35.000000 habapp_rules-5.6.0/habapp_rules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 15:20:35.431302 habapp_rules-5.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-24 15:20:27.000000 habapp_rules-5.6.0/setup.py
```

### Comparing `habapp_rules-5.5.1/LICENCE` & `habapp_rules-5.6.0/LICENCE`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/actors/config/light.py` & `habapp_rules-5.6.0/habapp_rules/actors/config/light.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/actors/config/light_hcl.py` & `habapp_rules-5.6.0/habapp_rules/actors/config/light_hcl.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/actors/config/shading.py` & `habapp_rules-5.6.0/habapp_rules/actors/config/shading.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/actors/config/ventilation.py` & `habapp_rules-5.6.0/habapp_rules/actors/config/ventilation.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/actors/irrigation.py` & `habapp_rules-5.6.0/habapp_rules/actors/irrigation.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/actors/light.py` & `habapp_rules-5.6.0/habapp_rules/actors/light.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/actors/light_hcl.py` & `habapp_rules-5.6.0/habapp_rules/actors/light_hcl.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/actors/shading.py` & `habapp_rules-5.6.0/habapp_rules/actors/shading.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/actors/state_observer.py` & `habapp_rules-5.6.0/habapp_rules/actors/state_observer.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/actors/ventilation.py` & `habapp_rules-5.6.0/habapp_rules/actors/ventilation.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/bridge/knx_mqtt.py` & `habapp_rules-5.6.0/habapp_rules/bridge/knx_mqtt.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/common/filter.py` & `habapp_rules-5.6.0/habapp_rules/common/filter.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/common/hysteresis.py` & `habapp_rules-5.6.0/habapp_rules/common/hysteresis.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/common/logic.py` & `habapp_rules-5.6.0/habapp_rules/common/logic.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/core/helper.py` & `habapp_rules-5.6.0/habapp_rules/core/helper.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/core/logger.py` & `habapp_rules-5.6.0/habapp_rules/core/logger.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/core/state_machine_rule.py` & `habapp_rules-5.6.0/habapp_rules/core/state_machine_rule.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/core/timeout_list.py` & `habapp_rules-5.6.0/habapp_rules/core/timeout_list.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/core/type_of_day.py` & `habapp_rules-5.6.0/habapp_rules/core/type_of_day.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/core/version.py` & `habapp_rules-5.6.0/habapp_rules/core/version.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/sensors/astro.py` & `habapp_rules-5.6.0/habapp_rules/sensors/astro.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/sensors/dwd.py` & `habapp_rules-5.6.0/habapp_rules/sensors/dwd.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/sensors/motion.py` & `habapp_rules-5.6.0/habapp_rules/sensors/motion.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/sensors/sun.py` & `habapp_rules-5.6.0/habapp_rules/sensors/sun.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/system/presence.py` & `habapp_rules-5.6.0/habapp_rules/system/presence.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/system/sleep.py` & `habapp_rules-5.6.0/habapp_rules/system/sleep.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules/system/summer_winter.py` & `habapp_rules-5.6.0/habapp_rules/system/summer_winter.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-5.5.1/habapp_rules.egg-info/SOURCES.txt` & `habapp_rules-5.6.0/habapp_rules.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 habapp_rules/core/exceptions.py
 habapp_rules/core/helper.py
 habapp_rules/core/logger.py
 habapp_rules/core/state_machine_rule.py
 habapp_rules/core/timeout_list.py
 habapp_rules/core/type_of_day.py
 habapp_rules/core/version.py
+habapp_rules/energy/__init__.py
+habapp_rules/energy/donut_chart.py
+habapp_rules/energy/monthly_report.py
 habapp_rules/sensors/__init__.py
 habapp_rules/sensors/astro.py
 habapp_rules/sensors/dwd.py
 habapp_rules/sensors/motion.py
 habapp_rules/sensors/sun.py
 habapp_rules/system/__init__.py
 habapp_rules/system/presence.py
```

