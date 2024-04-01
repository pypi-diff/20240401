# Comparing `tmp/besapi-3.2.2.tar.gz` & `tmp/besapi-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "besapi-3.2.2.tar", last modified: Thu Mar  7 22:39:54 2024, max compression
+gzip compressed data, was "besapi-3.2.4.tar", last modified: Mon Apr  1 17:03:57 2024, max compression
```

## Comparing `besapi-3.2.2.tar` & `besapi-3.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:39:54.702466 besapi-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-07 22:38:39.000000 besapi-3.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-07 22:38:39.000000 besapi-3.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-03-07 22:39:54.702466 besapi-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-03-07 22:38:39.000000 besapi-3.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-07 22:38:39.000000 besapi-3.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-07 22:39:54.702466 besapi-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-07 22:38:39.000000 besapi-3.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:39:54.698466 besapi-3.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:39:54.702466 besapi-3.2.2/src/besapi/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-07 22:38:39.000000 besapi-3.2.2/src/besapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-07 22:38:39.000000 besapi-3.2.2/src/besapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35459 2024-03-07 22:38:39.000000 besapi-3.2.2/src/besapi/besapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:39:54.702466 besapi-3.2.2/src/besapi/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    42635 2024-03-07 22:38:39.000000 besapi-3.2.2/src/besapi/schemas/BES.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    25664 2024-03-07 22:38:39.000000 besapi-3.2.2/src/besapi/schemas/BESAPI.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    20054 2024-03-07 22:38:39.000000 besapi-3.2.2/src/besapi/schemas/BESActionSettings.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:39:54.702466 besapi-3.2.2/src/besapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-03-07 22:39:54.000000 besapi-3.2.2/src/besapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-07 22:39:54.000000 besapi-3.2.2/src/besapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 22:39:54.000000 besapi-3.2.2/src/besapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-07 22:39:54.000000 besapi-3.2.2/src/besapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-07 22:39:54.000000 besapi-3.2.2/src/besapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:39:54.702466 besapi-3.2.2/src/bescli/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-07 22:38:39.000000 besapi-3.2.2/src/bescli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-07 22:38:39.000000 besapi-3.2.2/src/bescli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15127 2024-03-07 22:38:39.000000 besapi-3.2.2/src/bescli/bescli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 22:39:54.702466 besapi-3.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-03-07 22:38:39.000000 besapi-3.2.2/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:03:57.281728 besapi-3.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-01 17:02:18.000000 besapi-3.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 17:02:18.000000 besapi-3.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-01 17:03:57.281728 besapi-3.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-01 17:02:18.000000 besapi-3.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-01 17:02:18.000000 besapi-3.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-01 17:03:57.281728 besapi-3.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-01 17:02:18.000000 besapi-3.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:03:57.277728 besapi-3.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:03:57.277728 besapi-3.2.4/src/besapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-01 17:02:18.000000 besapi-3.2.4/src/besapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-01 17:02:18.000000 besapi-3.2.4/src/besapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36475 2024-04-01 17:02:18.000000 besapi-3.2.4/src/besapi/besapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:03:57.281728 besapi-3.2.4/src/besapi/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    42635 2024-04-01 17:02:18.000000 besapi-3.2.4/src/besapi/schemas/BES.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    25664 2024-04-01 17:02:18.000000 besapi-3.2.4/src/besapi/schemas/BESAPI.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    20054 2024-04-01 17:02:18.000000 besapi-3.2.4/src/besapi/schemas/BESActionSettings.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:03:57.281728 besapi-3.2.4/src/besapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-01 17:03:57.000000 besapi-3.2.4/src/besapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-01 17:03:57.000000 besapi-3.2.4/src/besapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 17:03:57.000000 besapi-3.2.4/src/besapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-01 17:03:57.000000 besapi-3.2.4/src/besapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 17:03:57.000000 besapi-3.2.4/src/besapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:03:57.281728 besapi-3.2.4/src/bescli/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-01 17:02:18.000000 besapi-3.2.4/src/bescli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 17:02:18.000000 besapi-3.2.4/src/bescli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15127 2024-04-01 17:02:18.000000 besapi-3.2.4/src/bescli/bescli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:03:57.281728 besapi-3.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-01 17:02:18.000000 besapi-3.2.4/tests/tests.py
```

### Comparing `besapi-3.2.2/LICENSE.txt` & `besapi-3.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `besapi-3.2.2/PKG-INFO` & `besapi-3.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besapi
-Version: 3.2.2
+Version: 3.2.4
 Summary: Library for working with the BigFix REST API
 Home-page: https://github.com/jgstew/besapi
 Author: Matt Hansen, James Stewart
 Author-email: hansen.m@psu.edu, james@jgstew.com
 License: MIT
 Keywords: bigfix iem tem rest api
 Classifier: Programming Language :: Python :: 3
```

### Comparing `besapi-3.2.2/README.md` & `besapi-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `besapi-3.2.2/setup.py` & `besapi-3.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `besapi-3.2.2/src/besapi/besapi.py` & `besapi-3.2.4/src/besapi/besapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 except ImportError:
     from urlparse import parse_qs as parse
 
 import requests
 from lxml import etree, objectify
 from pkg_resources import resource_filename
 
-__version__ = "3.2.2"
+__version__ = "3.2.4"
 
 besapi_logger = logging.getLogger("besapi")
 
 
 def rand_password(length=20):
     """get a random password"""
 
@@ -389,14 +389,42 @@
         return bool(self.last_connected)
 
     def logout(self):
         """clear session and close it"""
         self.session.cookies.clear()
         self.session.close()
 
+    def set_dashboard_variable_value(
+        self, dashboard_name, var_name, var_value, private=False
+    ):
+        """set the variable value from a dashboard datastore"""
+
+        dash_var_xml = f"""<BESAPI xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="BESAPI.xsd">
+            <DashboardData>
+                    <Dashboard>{dashboard_name}</Dashboard>
+                    <Name>{var_name}</Name>
+                    <IsPrivate>{str(private).lower()}</IsPrivate>
+                    <Value>{var_value}</Value>
+            </DashboardData>
+    </BESAPI>
+    """
+
+        return self.post(
+            f"dashboardvariable/{dashboard_name}/{var_name}", data=dash_var_xml
+        )
+
+    def get_dashboard_variable_value(self, dashboard_name, var_name):
+        """get the variable value from a dashboard datastore"""
+
+        return str(
+            self.get(
+                f"dashboardvariable/{dashboard_name}/{var_name}"
+            ).besobj.DashboardData.Value
+        )
+
     def validate_site_path(self, site_path, check_site_exists=True, raise_error=False):
         """make sure site_path is valid"""
 
         if site_path is None:
             if not raise_error:
                 return None
             raise ValueError("Site Path is `None` - NoneType Error")
```

### Comparing `besapi-3.2.2/src/besapi/schemas/BES.xsd` & `besapi-3.2.4/src/besapi/schemas/BES.xsd`

 * *Files identical despite different names*

### Comparing `besapi-3.2.2/src/besapi/schemas/BESAPI.xsd` & `besapi-3.2.4/src/besapi/schemas/BESAPI.xsd`

 * *Files identical despite different names*

### Comparing `besapi-3.2.2/src/besapi/schemas/BESActionSettings.xsd` & `besapi-3.2.4/src/besapi/schemas/BESActionSettings.xsd`

 * *Files identical despite different names*

### Comparing `besapi-3.2.2/src/besapi.egg-info/PKG-INFO` & `besapi-3.2.4/src/besapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besapi
-Version: 3.2.2
+Version: 3.2.4
 Summary: Library for working with the BigFix REST API
 Home-page: https://github.com/jgstew/besapi
 Author: Matt Hansen, James Stewart
 Author-email: hansen.m@psu.edu, james@jgstew.com
 License: MIT
 Keywords: bigfix iem tem rest api
 Classifier: Programming Language :: Python :: 3
```

### Comparing `besapi-3.2.2/src/bescli/bescli.py` & `besapi-3.2.4/src/bescli/bescli.py`

 * *Files identical despite different names*

### Comparing `besapi-3.2.2/tests/tests.py` & `besapi-3.2.4/tests/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 """
 Test besapi
 """
 
 import argparse
 import os
+import random
 import subprocess
 import sys
 
 # check for --test_pip arg
 parser = argparse.ArgumentParser()
 parser.add_argument(
     "--test_pip", help="to test package installed with pip", action="store_true"
@@ -124,14 +125,28 @@
     upload_result = bigfix_cli.bes_conn.upload(
         "./besapi/__init__.py", "test_besapi_upload.txt"
     )
     # print(upload_result)
     assert "test_besapi_upload.txt</URL>" in str(upload_result)
     print(bigfix_cli.bes_conn.parse_upload_result_to_prefetch(upload_result))
 
+    dashboard_name = "_PyBESAPI_tests.py"
+    var_name = "TestVarName"
+    var_value = "TestVarValue " + str(random.randint(0, 9999))
+
+    print(
+        bigfix_cli.bes_conn.set_dashboard_variable_value(
+            dashboard_name, var_name, var_value
+        )
+    )
+
+    assert var_value in str(
+        bigfix_cli.bes_conn.get_dashboard_variable_value(dashboard_name, var_name)
+    )
+
     if os.name == "nt":
         subprocess.run(
             'CMD /C python -m besapi ls clear ls conf "query number of bes computers" version error_count exit',
             check=True,
         )
         bes_conn = besapi.besapi.get_bes_conn_using_config_file()
         print("login succeeded:", bes_conn.login())
```

