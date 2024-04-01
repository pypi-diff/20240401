# Comparing `tmp/marble_client-1.1.1.tar.gz` & `tmp/marble_client-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marble_client-1.1.1.tar", last modified: Tue Feb 13 18:02:32 2024, max compression
+gzip compressed data, was "marble_client-1.1.2.tar", last modified: Mon Apr  1 13:48:40 2024, max compression
```

## Comparing `marble_client-1.1.1.tar` & `marble_client-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:02:32.725241 marble_client-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-02-13 18:02:22.000000 marble_client-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-02-13 18:02:32.725241 marble_client-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-02-13 18:02:22.000000 marble_client-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:02:32.725241 marble_client-1.1.1/marble_client/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-13 18:02:22.000000 marble_client-1.1.1/marble_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-02-13 18:02:22.000000 marble_client-1.1.1/marble_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-13 18:02:22.000000 marble_client-1.1.1/marble_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-13 18:02:22.000000 marble_client-1.1.1/marble_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-02-13 18:02:22.000000 marble_client-1.1.1/marble_client/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-02-13 18:02:22.000000 marble_client-1.1.1/marble_client/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:02:32.725241 marble_client-1.1.1/marble_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-02-13 18:02:32.000000 marble_client-1.1.1/marble_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-02-13 18:02:32.000000 marble_client-1.1.1/marble_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 18:02:32.000000 marble_client-1.1.1/marble_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-13 18:02:32.000000 marble_client-1.1.1/marble_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-13 18:02:32.000000 marble_client-1.1.1/marble_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-02-13 18:02:22.000000 marble_client-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-13 18:02:22.000000 marble_client-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 18:02:32.725241 marble_client-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:48:40.565268 marble_client-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-01 13:48:33.000000 marble_client-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-04-01 13:48:40.565268 marble_client-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-01 13:48:33.000000 marble_client-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:48:40.561268 marble_client-1.1.2/marble_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-01 13:48:33.000000 marble_client-1.1.2/marble_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-01 13:48:33.000000 marble_client-1.1.2/marble_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-01 13:48:33.000000 marble_client-1.1.2/marble_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-01 13:48:33.000000 marble_client-1.1.2/marble_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-01 13:48:33.000000 marble_client-1.1.2/marble_client/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-01 13:48:33.000000 marble_client-1.1.2/marble_client/services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:48:40.565268 marble_client-1.1.2/marble_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-04-01 13:48:40.000000 marble_client-1.1.2/marble_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-01 13:48:40.000000 marble_client-1.1.2/marble_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:48:40.000000 marble_client-1.1.2/marble_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-01 13:48:40.000000 marble_client-1.1.2/marble_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 13:48:40.000000 marble_client-1.1.2/marble_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-01 13:48:33.000000 marble_client-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 13:48:33.000000 marble_client-1.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:48:40.565268 marble_client-1.1.2/setup.cfg
```

### Comparing `marble_client-1.1.1/LICENSE` & `marble_client-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `marble_client-1.1.1/PKG-INFO` & `marble_client-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marble_client
-Version: 1.1.1
+Version: 1.1.2
 Summary: A python client to access information about the Marble climate infomatics network
 Author-email: Deepak Chandan <dchandan@cs.toronto.edu>
 License: MIT License
         
         Copyright (c) 2023 Data Analytics for Canadian Climate Services
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `marble_client-1.1.1/README.md` & `marble_client-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `marble_client-1.1.1/marble_client/client.py` & `marble_client-1.1.2/marble_client/client.py`

 * *Files identical despite different names*

### Comparing `marble_client-1.1.1/marble_client/constants.py` & `marble_client-1.1.2/marble_client/constants.py`

 * *Files identical despite different names*

### Comparing `marble_client-1.1.1/marble_client/node.py` & `marble_client-1.1.2/marble_client/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self._name = nodename
 
         for item in jsondata["links"]:
             setattr(self, "_links_" + item["rel"].replace("-", "_"), item["href"])
 
         self._services: list[str] = []
 
-        for service in jsondata["services"]:
+        for service in jsondata.get("services", []):
             s = MarbleService(service)
             setattr(self, s.name, s)
             self._services.append(s.name)
 
     def is_online(self) -> bool:
         try:
             registry = requests.get(self.url)
```

### Comparing `marble_client-1.1.1/marble_client/services.py` & `marble_client-1.1.2/marble_client/services.py`

 * *Files identical despite different names*

### Comparing `marble_client-1.1.1/marble_client.egg-info/PKG-INFO` & `marble_client-1.1.2/marble_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marble_client
-Version: 1.1.1
+Version: 1.1.2
 Summary: A python client to access information about the Marble climate infomatics network
 Author-email: Deepak Chandan <dchandan@cs.toronto.edu>
 License: MIT License
         
         Copyright (c) 2023 Data Analytics for Canadian Climate Services
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `marble_client-1.1.1/pyproject.toml` & `marble_client-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 description = "A python client to access information about the Marble climate infomatics network"
 dynamic = ["dependencies"]
 keywords = ["climate", "climate infomatics", "climate data", "DACCS", "Marble"]
 license = {file = "LICENSE"}
 name = "marble_client"
 readme = "README.md"
 requires-python = ">=3.9"
-version = "1.1.1"
+version = "1.1.2"
 
 [project.urls]
 # Homepage will change to Marble homepage when that goes live
 "Bug Tracker" = "https://github.com/DACCS-Climate/marble_client_python/issues"
 "Homepage" = "https://github.com/DACCS-Climate/marble_client_python"
 
 [tool.setuptools]
```

