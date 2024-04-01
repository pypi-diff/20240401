# Comparing `tmp/scalr-ngine-0.8.0.tar.gz` & `tmp/scalr-ngine-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalr-ngine-0.8.0.tar", last modified: Thu Jun 24 06:26:39 2021, max compression
+gzip compressed data, was "scalr-ngine-0.9.0.tar", last modified: Mon Jul 12 20:02:57 2021, max compression
```

## Comparing `scalr-ngine-0.8.0.tar` & `scalr-ngine-0.9.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 06:26:39.973360 scalr-ngine-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2021-06-24 06:26:39.973360 scalr-ngine-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      562 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 06:26:39.973360 scalr-ngine-0.8.0/scalr/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5262 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 06:26:39.973360 scalr-ngine-0.8.0/scalr/cloud/
--rw-r--r--   0 runner    (1001) docker     (121)     3857 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2274 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/cloud/cloudscale_ch.py
--rw-r--r--   0 runner    (1001) docker     (121)     4284 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/cloud/cloudstack.py
--rw-r--r--   0 runner    (1001) docker     (121)     2352 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/cloud/digitalocean.py
--rw-r--r--   0 runner    (1001) docker     (121)      594 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/cloud/exoscale.py
--rw-r--r--   0 runner    (1001) docker     (121)     2581 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/cloud/hcloud.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 06:26:39.973360 scalr-ngine-0.8.0/scalr/factory/
--rw-r--r--   0 runner    (1001) docker     (121)      551 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/factory/policy.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/factory/scalr.py
--rw-r--r--   0 runner    (1001) docker     (121)      379 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 06:26:39.973360 scalr-ngine-0.8.0/scalr/model/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      194 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/model/policy.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/model/scalr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 06:26:39.973360 scalr-ngine-0.8.0/scalr/policy/
--rw-r--r--   0 runner    (1001) docker     (121)      343 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      869 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/policy/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/policy/random.py
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/policy/web.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/scalr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 06:26:39.973360 scalr-ngine-0.8.0/scalr_ngine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2021-06-24 06:26:39.000000 scalr-ngine-0.8.0/scalr_ngine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      711 2021-06-24 06:26:39.000000 scalr-ngine-0.8.0/scalr_ngine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-24 06:26:39.000000 scalr-ngine-0.8.0/scalr_ngine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-06-24 06:26:39.000000 scalr-ngine-0.8.0/scalr_ngine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-06-24 06:26:39.000000 scalr-ngine-0.8.0/scalr_ngine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-06-24 06:26:39.000000 scalr-ngine-0.8.0/scalr_ngine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-06-24 06:26:39.973360 scalr-ngine-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2021-06-24 06:26:31.000000 scalr-ngine-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 20:02:57.845181 scalr-ngine-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1080 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1198 2021-07-12 20:02:57.845181 scalr-ngine-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      562 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 20:02:57.841181 scalr-ngine-0.9.0/scalr/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5985 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 20:02:57.841181 scalr-ngine-0.9.0/scalr/cloud/
+-rw-r--r--   0 runner    (1001) docker     (121)     3857 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2274 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/cloud/cloudscale_ch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4284 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/cloud/cloudstack.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2352 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/cloud/digitalocean.py
+-rw-r--r--   0 runner    (1001) docker     (121)      594 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/cloud/exoscale.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2581 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/cloud/hcloud.py
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 20:02:57.841181 scalr-ngine-0.9.0/scalr/factory/
+-rw-r--r--   0 runner    (1001) docker     (121)      551 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/factory/policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/factory/scalr.py
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/log.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 20:02:57.841181 scalr-ngine-0.9.0/scalr/model/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/model/policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/model/scalr.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 20:02:57.841181 scalr-ngine-0.9.0/scalr/policy/
+-rw-r--r--   0 runner    (1001) docker     (121)      343 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      869 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/policy/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/policy/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/policy/random.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/policy/web.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/scalr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 20:02:57.845181 scalr-ngine-0.9.0/scalr_ngine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1198 2021-07-12 20:02:57.000000 scalr-ngine-0.9.0/scalr_ngine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2021-07-12 20:02:57.000000 scalr-ngine-0.9.0/scalr_ngine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-12 20:02:57.000000 scalr-ngine-0.9.0/scalr_ngine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-07-12 20:02:57.000000 scalr-ngine-0.9.0/scalr_ngine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-07-12 20:02:57.000000 scalr-ngine-0.9.0/scalr_ngine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-07-12 20:02:57.000000 scalr-ngine-0.9.0/scalr_ngine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-07-12 20:02:57.845181 scalr-ngine-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1478 2021-07-12 20:02:50.000000 scalr-ngine-0.9.0/setup.py
```

### Comparing `scalr-ngine-0.8.0/LICENSE` & `scalr-ngine-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scalr-ngine-0.8.0/PKG-INFO` & `scalr-ngine-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: scalr-ngine
-Version: 0.8.0
+Version: 0.9.0
 Summary: Autoscaling for Clouds.
 Home-page: https://github.com/ngine-io/scalr
 Author: René Moser
 Author-email: mail@renemoser.net
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Web Environment
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `scalr-ngine-0.8.0/README.md` & `scalr-ngine-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `scalr-ngine-0.8.0/scalr/app.py` & `scalr-ngine-0.9.0/scalr/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import os
 import sys
 
 import time
 import schedule
 from datetime import datetime
 from argparse import ArgumentParser
+from prometheus_client import start_http_server, Gauge
 
 from scalr.version import __version__
 from scalr.log import log
 from scalr.config import read_config
 
 from scalr.factory.scalr import ScalrFactory
 from scalr.factory.policy import PolicyFactory
 
+metric_min = Gauge('scalr_min', 'Min amount of resources')
+metric_max = Gauge('scalr_max', 'Max amount of resources')
+metric_desired = Gauge('scalr_desired', 'Desired amount of resources')
+metric_current = Gauge('scalr_current', 'Current amount of resources')
+metric_max_step_down = Gauge('scalr_max_step_down', 'Max step for scaling down')
+
 def get_scaling_factor(policy_configs: list) -> int:
     scaling_factor: int = 0
     for policy_config in policy_configs:
         try:
             log.info(f"Processing {policy_config['name']}")
 
             policy_factory = PolicyFactory()
@@ -80,17 +87,14 @@
         # Break on request
         if time_rule.get('on_match', '') == 'break':
             log.info(f"Breaking on match requested")
             return base_rule
 
     return base_rule
 
-
-
-
 def app() -> None:
     print("")
     try:
         config: dict = read_config(config_source=os.getenv('SCALR_CONFIG', 'config.yml'))
         base_rule = config.get('base_rule') or dict()
         base_rule = process_time_rules(
             time_rules=config.get('time_rules') or list(),
@@ -111,14 +115,21 @@
         )
 
         scalr.scale(
             factor=get_scaling_factor(
                 policy_configs=config.get('policies', [])
             )
         )
+
+        # Set exporter metrics
+        metric_min.set(scalr.min)
+        metric_max.set(scalr.max)
+        metric_current.set(scalr.current)
+        metric_desired.set(scalr.desired)
+        metric_max_step_down.set(scalr.max_step_down)
     except Exception as ex:
         log.error(ex)
         sys.exit(1)
 
 def run_periodic(interval: int = 60) -> None:
     log.info(f"Running periodic in intervals of {interval}s")
     schedule.every(interval).seconds.do(app)
@@ -140,14 +151,15 @@
         print(f"version {__version__}")
         sys.exit(0)
 
     log.info(f"Starting, version {__version__}")
 
     if args.periodic:
         try:
+            start_http_server(int(os.environ.get('SCALR_PROMETHEUS_EXPORTER_PORT', 8000)))
             run_periodic(args.interval)
         except KeyboardInterrupt:
             print("")
             log.info(f"Stopping...")
             schedule.clear()
             log.info(f"done")
             pass
```

### Comparing `scalr-ngine-0.8.0/scalr/cloud/__init__.py` & `scalr-ngine-0.9.0/scalr/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `scalr-ngine-0.8.0/scalr/cloud/cloudscale_ch.py` & `scalr-ngine-0.9.0/scalr/cloud/cloudscale_ch.py`

 * *Files identical despite different names*

### Comparing `scalr-ngine-0.8.0/scalr/cloud/cloudstack.py` & `scalr-ngine-0.9.0/scalr/cloud/cloudstack.py`

 * *Files identical despite different names*

### Comparing `scalr-ngine-0.8.0/scalr/cloud/digitalocean.py` & `scalr-ngine-0.9.0/scalr/cloud/digitalocean.py`

 * *Files identical despite different names*

### Comparing `scalr-ngine-0.8.0/scalr/cloud/exoscale.py` & `scalr-ngine-0.9.0/scalr/cloud/exoscale.py`

 * *Files identical despite different names*

### Comparing `scalr-ngine-0.8.0/scalr/cloud/hcloud.py` & `scalr-ngine-0.9.0/scalr/cloud/hcloud.py`

 * *Files identical despite different names*

### Comparing `scalr-ngine-0.8.0/scalr/config.py` & `scalr-ngine-0.9.0/scalr/config.py`

 * *Files identical despite different names*

### Comparing `scalr-ngine-0.8.0/scalr/factory/__init__.py` & `scalr-ngine-0.9.0/scalr/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `scalr-ngine-0.8.0/scalr/factory/scalr.py` & `scalr-ngine-0.9.0/scalr/factory/scalr.py`

 * *Files identical despite different names*

### Comparing `scalr-ngine-0.8.0/scalr/policy/influxdb.py` & `scalr-ngine-0.9.0/scalr/policy/influxdb.py`

 * *Files identical despite different names*

### Comparing `scalr-ngine-0.8.0/scalr/policy/web.py` & `scalr-ngine-0.9.0/scalr/policy/web.py`

 * *Files identical despite different names*

### Comparing `scalr-ngine-0.8.0/scalr_ngine.egg-info/PKG-INFO` & `scalr-ngine-0.9.0/scalr_ngine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: scalr-ngine
-Version: 0.8.0
+Version: 0.9.0
 Summary: Autoscaling for Clouds.
 Home-page: https://github.com/ngine-io/scalr
 Author: René Moser
 Author-email: mail@renemoser.net
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Web Environment
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `scalr-ngine-0.8.0/scalr_ngine.egg-info/SOURCES.txt` & `scalr-ngine-0.9.0/scalr_ngine.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 scalr/factory/policy.py
 scalr/factory/scalr.py
 scalr/model/__init__.py
 scalr/model/policy.py
 scalr/model/scalr.py
 scalr/policy/__init__.py
 scalr/policy/influxdb.py
+scalr/policy/prometheus.py
 scalr/policy/random.py
 scalr/policy/web.py
 scalr_ngine.egg-info/PKG-INFO
 scalr_ngine.egg-info/SOURCES.txt
 scalr_ngine.egg-info/dependency_links.txt
 scalr_ngine.egg-info/entry_points.txt
 scalr_ngine.egg-info/requires.txt
```

### Comparing `scalr-ngine-0.8.0/setup.py` & `scalr-ngine-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ngine-io/scalr",
     packages=find_packages(exclude=["test.*", "tests"]),
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Environment :: Web Environment",
     ],
     install_requires=install_requires,
     tests_require=tests_require,
```

