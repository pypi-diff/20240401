# Comparing `tmp/py_nessus_pro-1.1.4.tar.gz` & `tmp/py_nessus_pro-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_nessus_pro-1.1.4.tar", last modified: Tue Feb  6 12:39:53 2024, max compression
+gzip compressed data, was "py_nessus_pro-1.2.0.tar", last modified: Mon Apr  1 20:24:02 2024, max compression
```

## Comparing `py_nessus_pro-1.1.4.tar` & `py_nessus_pro-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 12:39:53.178825 py_nessus_pro-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-02-06 12:39:43.000000 py_nessus_pro-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-02-06 12:39:53.178825 py_nessus_pro-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-02-06 12:39:43.000000 py_nessus_pro-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 12:39:53.178825 py_nessus_pro-1.1.4/py_nessus_pro/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 12:39:43.000000 py_nessus_pro-1.1.4/py_nessus_pro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-02-06 12:39:43.000000 py_nessus_pro-1.1.4/py_nessus_pro/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-02-06 12:39:43.000000 py_nessus_pro-1.1.4/py_nessus_pro/py_nessus_pro.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-02-06 12:39:43.000000 py_nessus_pro-1.1.4/py_nessus_pro/py_nessus_pro_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-02-06 12:39:43.000000 py_nessus_pro-1.1.4/py_nessus_pro/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 12:39:53.178825 py_nessus_pro-1.1.4/py_nessus_pro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-02-06 12:39:53.000000 py_nessus_pro-1.1.4/py_nessus_pro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-02-06 12:39:53.000000 py_nessus_pro-1.1.4/py_nessus_pro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 12:39:53.000000 py_nessus_pro-1.1.4/py_nessus_pro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-06 12:39:53.000000 py_nessus_pro-1.1.4/py_nessus_pro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-06 12:39:53.000000 py_nessus_pro-1.1.4/py_nessus_pro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-06 12:39:53.000000 py_nessus_pro-1.1.4/py_nessus_pro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 12:39:53.178825 py_nessus_pro-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-02-06 12:39:43.000000 py_nessus_pro-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:24:02.163110 py_nessus_pro-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-01 20:23:58.000000 py_nessus_pro-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-01 20:24:02.163110 py_nessus_pro-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-01 20:23:58.000000 py_nessus_pro-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:24:02.163110 py_nessus_pro-1.2.0/py_nessus_pro/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:23:58.000000 py_nessus_pro-1.2.0/py_nessus_pro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-01 20:23:58.000000 py_nessus_pro-1.2.0/py_nessus_pro/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-04-01 20:23:58.000000 py_nessus_pro-1.2.0/py_nessus_pro/py_nessus_pro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-01 20:23:58.000000 py_nessus_pro-1.2.0/py_nessus_pro/py_nessus_pro_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-04-01 20:23:58.000000 py_nessus_pro-1.2.0/py_nessus_pro/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:24:02.163110 py_nessus_pro-1.2.0/py_nessus_pro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-01 20:24:02.000000 py_nessus_pro-1.2.0/py_nessus_pro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-01 20:24:02.000000 py_nessus_pro-1.2.0/py_nessus_pro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:24:02.000000 py_nessus_pro-1.2.0/py_nessus_pro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-01 20:24:02.000000 py_nessus_pro-1.2.0/py_nessus_pro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-01 20:24:02.000000 py_nessus_pro-1.2.0/py_nessus_pro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 20:24:02.000000 py_nessus_pro-1.2.0/py_nessus_pro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:24:02.163110 py_nessus_pro-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-01 20:23:58.000000 py_nessus_pro-1.2.0/setup.py
```

### Comparing `py_nessus_pro-1.1.4/LICENSE` & `py_nessus_pro-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_nessus_pro-1.1.4/PKG-INFO` & `py_nessus_pro-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_nessus_pro
-Version: 1.1.4
+Version: 1.2.0
 Summary: Python library for managing Nessus Professional.
 Home-page: https://github.com/Matbe34/py-nessus-pro
 Author: Matbe34
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 Requires-Dist: selenium
 Requires-Dist: beautifulsoup4
```

### Comparing `py_nessus_pro-1.1.4/README.md` & `py_nessus_pro-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `py_nessus_pro-1.1.4/py_nessus_pro/logger.py` & `py_nessus_pro-1.2.0/py_nessus_pro/logger.py`

 * *Files identical despite different names*

### Comparing `py_nessus_pro-1.1.4/py_nessus_pro/py_nessus_pro.py` & `py_nessus_pro-1.2.0/py_nessus_pro/py_nessus_pro.py`

 * *Files identical despite different names*

### Comparing `py_nessus_pro-1.1.4/py_nessus_pro/py_nessus_pro_cli.py` & `py_nessus_pro-1.2.0/py_nessus_pro/py_nessus_pro_cli.py`

 * *Files identical despite different names*

### Comparing `py_nessus_pro-1.1.4/py_nessus_pro/scan.py` & `py_nessus_pro-1.2.0/py_nessus_pro/scan.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     nessus_server = ""
     headers = {}
 
     export_types = {
         "nessus":"",
         "csv":"",
         "html":"vuln_by_host;compliance_exec;remediations;",
-        "pdf":"vuln_by_host;compliance_exec;remediations;",
+        # Disable pdf export as some Nessus installations do not support it
+        # "pdf":"vuln_by_host;compliance_exec;remediations;",
     }
 
     def __init__(self, nessus_server: str, headers: dict, folder_map: dict, policy_map: dict, name: str = "", targets: str = "", id: str = "", folder: str = ""):
         self.id = id
         self.metadata = json.loads('''{
             "uuid":"ab4bacd2-05f6-425c-9d79-3ba3940ad1c24e51e1f403febe40",
             "settings":{
@@ -122,19 +123,22 @@
     def get_metadata(self):
         return self.metadata
         
     def get_status(self):
         if self.id:
             x = json.loads(requests.get(f"{self.nessus_server}/scans/{self.id}", headers=self.headers, verify=False).text)
             res = {}
-            res["status"] = x["info"]["status"]
-            res["scan_start"] = x["info"]["scan_start"] if res["status"] != "empty" else None
-            res["scan_end"] = x["info"]["scan_end"] if res["status"] == "completed" else None 
-            res["name"] = x["info"]["name"]
-            return res
+            if x.get("info", None):
+                res["status"] = x["info"]["status"]
+                res["scan_start"] = x["info"].get("scan_start", None)
+                res["scan_end"] = x["info"].get("scan_end", None )
+                res["name"] = x["info"]["name"]
+                return res
+            else:
+                return "Error retrieving scan status, check authorization issues or retry request."
         else:
             return "Scan not posted yet"
     
     def post(self):
         if not self.metadata["settings"]["text_targets"]:
             raise Exception("[!] No targets provided")
         x = json.loads(requests.post(f"{self.nessus_server}/scans", headers=self.headers, json = self.metadata, verify=False).text)
@@ -151,26 +155,25 @@
             "metadata":self.metadata,
         }
 
     def get_reports(self, path: str):
         if not self.id:
             log.error("Scan not posted yet")
             return
-        if self.get_status()["status"] != "completed":
-            log.error("Scan not completed yet")
+        if self.get_status()["status"] not in ["completed", "canceled", "imported"]:
+            log.error("Scan not finished yet")
             return
 
         for t in self.export_types:
             data = json.loads('{"format":"csv","reportContents":{"csvColumns":{"id":true,"cve":true,"cvss":true,"risk":true,"hostname":true,"protocol":true,"port":true,"plugin_name":true,"synopsis":true,"description":true,"solution":true,"see_also":true,"plugin_output":true,"stig_severity":true,"cvss3_base_score":true,"cvss_temporal_score":true,"cvss3_temporal_score":true,"vpr_score":true,"risk_factor":true,"references":true,"plugin_information":true,"exploitable_with":true}},"extraFilters":{"host_ids":[],"plugin_ids":[]}}')
             data["format"] = t
 
             if t in ["html", "pdf"]:
                 data = json.loads('{"format":"", "chapters": "vuln_by_plugin"}')
                 data["format"] = t
-                # data = json.loads('{"format":"html", "chapters": "vuln_by_host;compliance_exec;remediations;"}')                
 
             res = json.loads(requests.post(f"{self.nessus_server}/scans/{self.id}/export", headers=self.headers, json = data, verify=False).text)
             if "token" in res:
                 log.debug("Export in progress: " + res["token"])
                 status = json.loads(requests.get(f"{self.nessus_server}/tokens/{res['token']}/status", headers=self.headers, verify=False).text)
                 while status["status"] != "ready":
                     if status["status"] == "error":
```

### Comparing `py_nessus_pro-1.1.4/py_nessus_pro.egg-info/PKG-INFO` & `py_nessus_pro-1.2.0/py_nessus_pro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_nessus_pro
-Version: 1.1.4
+Version: 1.2.0
 Summary: Python library for managing Nessus Professional.
 Home-page: https://github.com/Matbe34/py-nessus-pro
 Author: Matbe34
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 Requires-Dist: selenium
 Requires-Dist: beautifulsoup4
```

### Comparing `py_nessus_pro-1.1.4/setup.py` & `py_nessus_pro-1.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='py_nessus_pro',
-    version='1.1.4',
+    version='1.2.0',
     packages=find_packages(),
     install_requires=[
          'selenium',
          'beautifulsoup4',
          'python-slugify',
          'requests',
          'logger',
```

