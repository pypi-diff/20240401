# Comparing `tmp/pyiikocloudapi-0.0.8.tar.gz` & `tmp/pyiikocloudapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiikocloudapi-0.0.8.tar", last modified: Sat Mar 11 15:51:43 2023, max compression
+gzip compressed data, was "pyiikocloudapi-0.0.9.tar", last modified: Fri Mar 17 18:24:49 2023, max compression
```

## Comparing `pyiikocloudapi-0.0.8.tar` & `pyiikocloudapi-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 macmini    (501) staff       (20)        0 2023-03-11 15:51:43.558671 pyiikocloudapi-0.0.8/
--rwxr-xr-x   0 macmini    (501) staff       (20)     1080 2021-03-12 14:58:16.000000 pyiikocloudapi-0.0.8/LICENSE
--rw-r--r--   0 macmini    (501) staff       (20)    13946 2023-03-11 15:51:43.558774 pyiikocloudapi-0.0.8/PKG-INFO
--rw-r--r--   0 macmini    (501) staff       (20)    13500 2022-07-26 19:44:32.000000 pyiikocloudapi-0.0.8/README.md
-drwxr-xr-x   0 macmini    (501) staff       (20)        0 2023-03-11 15:51:43.556764 pyiikocloudapi-0.0.8/pyiikocloudapi/
--rw-r--r--   0 macmini    (501) staff       (20)      185 2023-03-11 15:51:36.000000 pyiikocloudapi-0.0.8/pyiikocloudapi/__init__.py
--rw-r--r--   0 macmini    (501) staff       (20)    62003 2023-03-11 15:51:36.000000 pyiikocloudapi-0.0.8/pyiikocloudapi/api.py
--rw-r--r--   0 macmini    (501) staff       (20)     3519 2022-05-18 18:20:46.000000 pyiikocloudapi-0.0.8/pyiikocloudapi/decorators.py
--rw-r--r--   0 macmini    (501) staff       (20)     1571 2022-05-12 19:37:43.000000 pyiikocloudapi-0.0.8/pyiikocloudapi/exception.py
--rw-r--r--   0 macmini    (501) staff       (20)    34029 2022-12-21 10:32:15.000000 pyiikocloudapi-0.0.8/pyiikocloudapi/models.py
-drwxr-xr-x   0 macmini    (501) staff       (20)        0 2023-03-11 15:51:43.558506 pyiikocloudapi-0.0.8/pyiikocloudapi.egg-info/
--rw-r--r--   0 macmini    (501) staff       (20)    13946 2023-03-11 15:51:43.000000 pyiikocloudapi-0.0.8/pyiikocloudapi.egg-info/PKG-INFO
--rw-r--r--   0 macmini    (501) staff       (20)      393 2023-03-11 15:51:43.000000 pyiikocloudapi-0.0.8/pyiikocloudapi.egg-info/SOURCES.txt
--rw-r--r--   0 macmini    (501) staff       (20)        1 2023-03-11 15:51:43.000000 pyiikocloudapi-0.0.8/pyiikocloudapi.egg-info/dependency_links.txt
--rw-r--r--   0 macmini    (501) staff       (20)        1 2022-07-30 09:23:27.000000 pyiikocloudapi-0.0.8/pyiikocloudapi.egg-info/not-zip-safe
--rw-r--r--   0 macmini    (501) staff       (20)       18 2023-03-11 15:51:43.000000 pyiikocloudapi-0.0.8/pyiikocloudapi.egg-info/requires.txt
--rw-r--r--   0 macmini    (501) staff       (20)       15 2023-03-11 15:51:43.000000 pyiikocloudapi-0.0.8/pyiikocloudapi.egg-info/top_level.txt
--rwxr-xr-x   0 macmini    (501) staff       (20)       38 2023-03-11 15:51:43.559199 pyiikocloudapi-0.0.8/setup.cfg
--rwxr-xr-x   0 macmini    (501) staff       (20)      801 2023-03-11 15:51:36.000000 pyiikocloudapi-0.0.8/setup.py
+drwxr-xr-x   0 macmini    (501) staff       (20)        0 2023-03-17 18:24:49.310040 pyiikocloudapi-0.0.9/
+-rwxr-xr-x   0 macmini    (501) staff       (20)     1080 2021-03-12 14:58:16.000000 pyiikocloudapi-0.0.9/LICENSE
+-rw-r--r--   0 macmini    (501) staff       (20)    13946 2023-03-17 18:24:49.310143 pyiikocloudapi-0.0.9/PKG-INFO
+-rw-r--r--   0 macmini    (501) staff       (20)    13500 2022-07-26 19:44:32.000000 pyiikocloudapi-0.0.9/README.md
+drwxr-xr-x   0 macmini    (501) staff       (20)        0 2023-03-17 18:24:49.308040 pyiikocloudapi-0.0.9/pyiikocloudapi/
+-rw-r--r--   0 macmini    (501) staff       (20)      185 2023-03-17 18:24:44.000000 pyiikocloudapi-0.0.9/pyiikocloudapi/__init__.py
+-rw-r--r--   0 macmini    (501) staff       (20)    62031 2023-03-17 18:24:18.000000 pyiikocloudapi-0.0.9/pyiikocloudapi/api.py
+-rw-r--r--   0 macmini    (501) staff       (20)     3519 2022-05-18 18:20:46.000000 pyiikocloudapi-0.0.9/pyiikocloudapi/decorators.py
+-rw-r--r--   0 macmini    (501) staff       (20)     1571 2022-05-12 19:37:43.000000 pyiikocloudapi-0.0.9/pyiikocloudapi/exception.py
+-rw-r--r--   0 macmini    (501) staff       (20)    34029 2022-12-21 10:32:15.000000 pyiikocloudapi-0.0.9/pyiikocloudapi/models.py
+drwxr-xr-x   0 macmini    (501) staff       (20)        0 2023-03-17 18:24:49.309847 pyiikocloudapi-0.0.9/pyiikocloudapi.egg-info/
+-rw-r--r--   0 macmini    (501) staff       (20)    13946 2023-03-17 18:24:49.000000 pyiikocloudapi-0.0.9/pyiikocloudapi.egg-info/PKG-INFO
+-rw-r--r--   0 macmini    (501) staff       (20)      393 2023-03-17 18:24:49.000000 pyiikocloudapi-0.0.9/pyiikocloudapi.egg-info/SOURCES.txt
+-rw-r--r--   0 macmini    (501) staff       (20)        1 2023-03-17 18:24:49.000000 pyiikocloudapi-0.0.9/pyiikocloudapi.egg-info/dependency_links.txt
+-rw-r--r--   0 macmini    (501) staff       (20)        1 2022-07-30 09:23:27.000000 pyiikocloudapi-0.0.9/pyiikocloudapi.egg-info/not-zip-safe
+-rw-r--r--   0 macmini    (501) staff       (20)       18 2023-03-17 18:24:49.000000 pyiikocloudapi-0.0.9/pyiikocloudapi.egg-info/requires.txt
+-rw-r--r--   0 macmini    (501) staff       (20)       15 2023-03-17 18:24:49.000000 pyiikocloudapi-0.0.9/pyiikocloudapi.egg-info/top_level.txt
+-rwxr-xr-x   0 macmini    (501) staff       (20)       38 2023-03-17 18:24:49.310551 pyiikocloudapi-0.0.9/setup.cfg
+-rwxr-xr-x   0 macmini    (501) staff       (20)      801 2023-03-17 18:24:18.000000 pyiikocloudapi-0.0.9/setup.py
```

### Comparing `pyiikocloudapi-0.0.8/LICENSE` & `pyiikocloudapi-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiikocloudapi-0.0.8/PKG-INFO` & `pyiikocloudapi-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiikocloudapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python services for convenient work with iiko Transport
 Home-page: UNKNOWN
 Author: kebrick
 Author-email: ruban.kebr@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/kebrick/pyiikocloupapi
 Project-URL: Tracker, https://github.com/kebrick/pyiikocloupapi/issues
```

### Comparing `pyiikocloudapi-0.0.8/README.md` & `pyiikocloudapi-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyiikocloudapi-0.0.8/pyiikocloudapi/api.py` & `pyiikocloudapi-0.0.9/pyiikocloudapi/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -972,15 +972,15 @@
             "organizationId": organization_id,
             "order": order,
         }
         if terminal_group_id is not None:
             data["terminalGroupId"] = terminal_group_id
 
         if create_order_settings is not None:
-            data["createOrderSettings"] = create_order_settings
+            data["createOrderSettings"] = {"transportToFrontTimeout":create_order_settings}
 
         try:
 
             return self._post_request(
                 url="/api/1/deliveries/create",
                 data=data,
                 model_response_data=BaseCreatedDeliveryOrderInfoModel,
```

### Comparing `pyiikocloudapi-0.0.8/pyiikocloudapi/decorators.py` & `pyiikocloudapi-0.0.9/pyiikocloudapi/decorators.py`

 * *Files identical despite different names*

### Comparing `pyiikocloudapi-0.0.8/pyiikocloudapi/exception.py` & `pyiikocloudapi-0.0.9/pyiikocloudapi/exception.py`

 * *Files identical despite different names*

### Comparing `pyiikocloudapi-0.0.8/pyiikocloudapi/models.py` & `pyiikocloudapi-0.0.9/pyiikocloudapi/models.py`

 * *Files identical despite different names*

### Comparing `pyiikocloudapi-0.0.8/pyiikocloudapi.egg-info/PKG-INFO` & `pyiikocloudapi-0.0.9/pyiikocloudapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiikocloudapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python services for convenient work with iiko Transport
 Home-page: UNKNOWN
 Author: kebrick
 Author-email: ruban.kebr@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/kebrick/pyiikocloupapi
 Project-URL: Tracker, https://github.com/kebrick/pyiikocloupapi/issues
```

### Comparing `pyiikocloudapi-0.0.8/setup.py` & `pyiikocloudapi-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 setup(
     name='pyiikocloudapi',
     version=VERSION,
     description='Python services for convenient work with iiko Transport',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['pyiikocloudapi'],
```

