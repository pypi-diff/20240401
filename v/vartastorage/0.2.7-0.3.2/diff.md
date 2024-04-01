# Comparing `tmp/vartastorage-0.2.7.tar.gz` & `tmp/vartastorage-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vartastorage-0.2.7.tar", last modified: Fri Mar 15 20:20:31 2024, max compression
+gzip compressed data, was "vartastorage-0.3.2.tar", last modified: Mon Apr  1 11:01:41 2024, max compression
```

## Comparing `vartastorage-0.2.7.tar` & `vartastorage-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:20:31.296237 vartastorage-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-15 20:20:31.296237 vartastorage-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-15 20:20:21.000000 vartastorage-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 20:20:31.296237 vartastorage-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-15 20:20:21.000000 vartastorage-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:20:31.292237 vartastorage-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:20:31.296237 vartastorage-0.2.7/src/vartastorage/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-15 20:20:21.000000 vartastorage-0.2.7/src/vartastorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-03-15 20:20:21.000000 vartastorage-0.2.7/src/vartastorage/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-03-15 20:20:21.000000 vartastorage-0.2.7/src/vartastorage/vartastorage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:20:31.296237 vartastorage-0.2.7/src/vartastorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-15 20:20:31.000000 vartastorage-0.2.7/src/vartastorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-15 20:20:31.000000 vartastorage-0.2.7/src/vartastorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 20:20:31.000000 vartastorage-0.2.7/src/vartastorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 20:20:21.000000 vartastorage-0.2.7/src/vartastorage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-15 20:20:31.000000 vartastorage-0.2.7/src/vartastorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-15 20:20:31.000000 vartastorage-0.2.7/src/vartastorage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:41.704043 vartastorage-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-01 11:01:41.700043 vartastorage-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-01 11:01:37.000000 vartastorage-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 11:01:41.704043 vartastorage-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-01 11:01:37.000000 vartastorage-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:41.700043 vartastorage-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:41.700043 vartastorage-0.3.2/src/vartastorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:37.000000 vartastorage-0.3.2/src/vartastorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-01 11:01:37.000000 vartastorage-0.3.2/src/vartastorage/cgi_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-01 11:01:37.000000 vartastorage-0.3.2/src/vartastorage/cgi_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-01 11:01:37.000000 vartastorage-0.3.2/src/vartastorage/modbus_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-01 11:01:37.000000 vartastorage-0.3.2/src/vartastorage/vartastorage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:41.700043 vartastorage-0.3.2/src/vartastorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-01 11:01:41.000000 vartastorage-0.3.2/src/vartastorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-01 11:01:41.000000 vartastorage-0.3.2/src/vartastorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:01:41.000000 vartastorage-0.3.2/src/vartastorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:01:41.000000 vartastorage-0.3.2/src/vartastorage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 11:01:41.000000 vartastorage-0.3.2/src/vartastorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 11:01:41.000000 vartastorage-0.3.2/src/vartastorage.egg-info/top_level.txt
```

### Comparing `vartastorage-0.2.7/README.md` & `vartastorage-0.3.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 # Vartastorage
-With this Python module you can read modbus registers and xml api values from various VARTA batteries. 
+
+With this Python module you can read modbus registers and xml api values from various VARTA batteries.
 Tested on my VARTA element/12 battery.
 Should work for other VARTA element, pulse, pulse neo, link and flex storage devices as well.
 
 ## Setup
+
 pip3 install vartastorage
 
 ## Usage
+
 ```python
 from vartastorage.vartastorage import VartaStorage
 
 # ip and port for modbus host
 varta = VartaStorage('10.0.2.3',502)
 
 # in case of a password protected cgi/xml endpoint you can authenticate as well.
 # user1 is for some varta devices a standard user
 varta = VartaStorage('10.0.2.3', 502, username="user1", password="yourpassword")
 
+# the CGI endpoints are covered by default. You can only use the modbus part as well
+varta = VartaStorage("10.0.2.3", 502, cgi=False)
+
 # update all values provided by modbus server
-varta.get_all_data_modbus()
+all_data = varta.get_all_data()
 
-# show current grid power
-print(varta.grid_power)
+# update all values provided by modbus server
+modbus_data = varta.get_all_data_modbus()
 
-# update only state of charge
-varta.get_soc()
+# show current grid power
+print(modbus_data.grid_power)
 
 # show battery SoC
-print(varta.soc)
-
-```
+print(modbus_data.soc)
+```
```

### Comparing `vartastorage-0.2.7/setup.py` & `vartastorage-0.3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import setuptools
 
 setuptools.setup(
     name="vartastorage",
-    version="0.2.7",
+    version="0.3.2",
     description="VARTA Battery",
-    long_description='With this Python module you can read modbus registers and xml/cgi api values from various VARTA batteries',
+    long_description="""
+        With this Python module you can read modbus registers
+        and xml/cgi api values from various VARTA batteries""",
     url="http://github.com/vip0r/vartastorage",
     author="edAndy",
     author_email="an-dy@gmx.de",
     license="APACHE",
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     zip_safe=False,
-    python_requires='>=3.5',
+    python_requires=">=3.11",
     install_requires=[
         "pymodbus",
         "requests",
     ],
-)
+)
```

