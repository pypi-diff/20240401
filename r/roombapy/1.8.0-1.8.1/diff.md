# Comparing `tmp/roombapy-1.8.0.tar.gz` & `tmp/roombapy-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roombapy-1.8.0.tar", max compression
+gzip compressed data, was "roombapy-1.8.1.tar", max compression
```

## Comparing `roombapy-1.8.0.tar` & `roombapy-1.8.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2024-04-01 19:55:56.579450 roombapy-1.8.0/LICENSE
--rw-r--r--   0        0        0     1520 2024-04-01 19:55:56.579450 roombapy-1.8.0/README.md
--rw-r--r--   0        0        0     2009 2024-04-01 19:55:56.579450 roombapy-1.8.0/pyproject.toml
--rw-r--r--   0        0        0      431 2024-04-01 19:55:56.579450 roombapy-1.8.0/roombapy/__init__.py
--rw-r--r--   0        0        0     5041 2024-04-01 19:55:56.579450 roombapy-1.8.0/roombapy/cli.py
--rw-r--r--   0        0        0     4538 2024-04-01 19:55:56.579450 roombapy-1.8.0/roombapy/const.py
--rw-r--r--   0        0        0     3720 2024-04-01 19:55:56.579450 roombapy-1.8.0/roombapy/discovery.py
--rw-r--r--   0        0        0     2895 2024-04-01 19:55:56.579450 roombapy-1.8.0/roombapy/getpassword.py
--rw-r--r--   0        0        0        0 2024-04-01 19:55:56.579450 roombapy-1.8.0/roombapy/py.typed
--rw-r--r--   0        0        0     6089 2024-04-01 19:55:56.583450 roombapy-1.8.0/roombapy/remote_client.py
--rw-r--r--   0        0        0    18685 2024-04-01 19:55:56.583450 roombapy-1.8.0/roombapy/roomba.py
--rw-r--r--   0        0        0      797 2024-04-01 19:55:56.583450 roombapy-1.8.0/roombapy/roomba_factory.py
--rw-r--r--   0        0        0     1583 2024-04-01 19:55:56.583450 roombapy-1.8.0/roombapy/roomba_info.py
--rw-r--r--   0        0        0     2603 1970-01-01 00:00:00.000000 roombapy-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-01 20:27:26.840017 roombapy-1.8.1/LICENSE
+-rw-r--r--   0        0        0     1520 2024-04-01 20:27:26.840017 roombapy-1.8.1/README.md
+-rw-r--r--   0        0        0     2009 2024-04-01 20:27:26.840017 roombapy-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0      431 2024-04-01 20:27:26.840017 roombapy-1.8.1/roombapy/__init__.py
+-rw-r--r--   0        0        0     5041 2024-04-01 20:27:26.840017 roombapy-1.8.1/roombapy/cli.py
+-rw-r--r--   0        0        0     4538 2024-04-01 20:27:26.840017 roombapy-1.8.1/roombapy/const.py
+-rw-r--r--   0        0        0     3720 2024-04-01 20:27:26.840017 roombapy-1.8.1/roombapy/discovery.py
+-rw-r--r--   0        0        0     2895 2024-04-01 20:27:26.840017 roombapy-1.8.1/roombapy/getpassword.py
+-rw-r--r--   0        0        0        0 2024-04-01 20:27:26.840017 roombapy-1.8.1/roombapy/py.typed
+-rw-r--r--   0        0        0     6089 2024-04-01 20:27:26.840017 roombapy-1.8.1/roombapy/remote_client.py
+-rw-r--r--   0        0        0    18685 2024-04-01 20:27:26.840017 roombapy-1.8.1/roombapy/roomba.py
+-rw-r--r--   0        0        0      797 2024-04-01 20:27:26.840017 roombapy-1.8.1/roombapy/roomba_factory.py
+-rw-r--r--   0        0        0     1590 2024-04-01 20:27:26.840017 roombapy-1.8.1/roombapy/roomba_info.py
+-rw-r--r--   0        0        0     2603 1970-01-01 00:00:00.000000 roombapy-1.8.1/PKG-INFO
```

### Comparing `roombapy-1.8.0/LICENSE` & `roombapy-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `roombapy-1.8.0/README.md` & `roombapy-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `roombapy-1.8.0/pyproject.toml` & `roombapy-1.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "roombapy"
-version = "1.8.0"
+version = "1.8.1"
 description = "Python program and library to control Wi-Fi enabled iRobot Roombas"
 authors = ["Philipp Schmitt <philipp@schmitt.co>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/pschmitt/roombapy"
 classifiers = [
     "Topic :: Software Development",
```

### Comparing `roombapy-1.8.0/roombapy/cli.py` & `roombapy-1.8.1/roombapy/cli.py`

 * *Files identical despite different names*

### Comparing `roombapy-1.8.0/roombapy/const.py` & `roombapy-1.8.1/roombapy/const.py`

 * *Files identical despite different names*

### Comparing `roombapy-1.8.0/roombapy/discovery.py` & `roombapy-1.8.1/roombapy/discovery.py`

 * *Files identical despite different names*

### Comparing `roombapy-1.8.0/roombapy/getpassword.py` & `roombapy-1.8.1/roombapy/getpassword.py`

 * *Files identical despite different names*

### Comparing `roombapy-1.8.0/roombapy/remote_client.py` & `roombapy-1.8.1/roombapy/remote_client.py`

 * *Files identical despite different names*

### Comparing `roombapy-1.8.0/roombapy/roomba.py` & `roombapy-1.8.1/roombapy/roomba.py`

 * *Files identical despite different names*

### Comparing `roombapy-1.8.0/roombapy/roomba_factory.py` & `roombapy-1.8.1/roombapy/roomba_factory.py`

 * *Files identical despite different names*

### Comparing `roombapy-1.8.0/roombapy/roomba_info.py` & `roombapy-1.8.1/roombapy/roomba_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from dataclasses import dataclass, field
 from functools import cached_property
 
 from mashumaro import field_options
 from mashumaro.mixins.orjson import DataClassORJSONMixin
 
-Capabilities = dict[str, int] | None
+Capabilities = dict[str, int | None] | None
 
 
 @dataclass
 class RoombaInfo(DataClassORJSONMixin):
     """Class for storing information about a Roomba device."""
 
     hostname: str
```

### Comparing `roombapy-1.8.0/PKG-INFO` & `roombapy-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roombapy
-Version: 1.8.0
+Version: 1.8.1
 Summary: Python program and library to control Wi-Fi enabled iRobot Roombas
 Home-page: https://github.com/pschmitt/roombapy
 License: MIT
 Author: Philipp Schmitt
 Author-email: philipp@schmitt.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

