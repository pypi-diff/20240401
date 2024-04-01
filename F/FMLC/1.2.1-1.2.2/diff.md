# Comparing `tmp/FMLC-1.2.1.tar.gz` & `tmp/FMLC-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FMLC-1.2.1.tar", last modified: Tue Mar 22 19:09:02 2022, max compression
+gzip compressed data, was "FMLC-1.2.2.tar", last modified: Mon Apr  1 21:36:33 2024, max compression
```

## Comparing `FMLC-1.2.1.tar` & `FMLC-1.2.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-03-22 19:09:02.102778 FMLC-1.2.1/
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-03-22 19:09:01.951573 FMLC-1.2.1/FMLC.egg-info/
--rwxr-xr-x   0 root         (0) root         (0)     4583 2022-03-22 19:09:00.000000 FMLC-1.2.1/FMLC.egg-info/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)      416 2022-03-22 19:09:01.000000 FMLC-1.2.1/FMLC.egg-info/SOURCES.txt
--rwxr-xr-x   0 root         (0) root         (0)        1 2022-03-22 19:09:01.000000 FMLC-1.2.1/FMLC.egg-info/dependency_links.txt
--rwxr-xr-x   0 root         (0) root         (0)       22 2022-03-22 19:09:01.000000 FMLC-1.2.1/FMLC.egg-info/requires.txt
--rwxr-xr-x   0 root         (0) root         (0)        5 2022-03-22 19:09:01.000000 FMLC-1.2.1/FMLC.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)     4583 2022-03-22 19:09:02.099892 FMLC-1.2.1/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     4166 2021-10-16 00:02:14.000000 FMLC-1.2.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-03-22 19:09:02.006691 FMLC-1.2.1/fmlc/
--rwxr-xr-x   0 root         (0) root         (0)      183 2022-03-22 19:06:56.000000 FMLC-1.2.1/fmlc/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6573 2022-03-21 18:37:24.000000 FMLC-1.2.1/fmlc/baseclasses.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-03-22 19:09:02.037794 FMLC-1.2.1/fmlc/pythonDB/
--rwxr-xr-x   0 root         (0) root         (0)        0 2021-10-16 03:25:47.000000 FMLC-1.2.1/fmlc/pythonDB/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     3631 2021-10-16 03:25:47.000000 FMLC-1.2.1/fmlc/pythonDB/pythonDB.py
--rwxr-xr-x   0 root         (0) root         (0)     2963 2022-03-04 17:51:53.000000 FMLC-1.2.1/fmlc/pythonDB/utility.py
--rwxr-xr-x   0 root         (0) root         (0)    23925 2022-03-21 19:01:39.000000 FMLC-1.2.1/fmlc/stackedclasses.py
--rwxr-xr-x   0 root         (0) root         (0)     3204 2022-03-04 18:47:33.000000 FMLC-1.2.1/fmlc/triggering.py
--rwxr-xr-x   0 root         (0) root         (0)      974 2021-10-28 18:36:58.000000 FMLC-1.2.1/fmlc/utility.py
--rwxr-xr-x   0 root         (0) root         (0)       92 2021-05-26 21:44:20.000000 FMLC-1.2.1/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)       38 2022-03-22 19:09:02.104457 FMLC-1.2.1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      833 2022-03-22 19:07:06.000000 FMLC-1.2.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-03-22 19:09:02.076009 FMLC-1.2.1/test/
--rwxr-xr-x   0 root         (0) root         (0)      835 2021-10-16 03:27:39.000000 FMLC-1.2.1/test/test_baseclasses.py
--rwxr-xr-x   0 root         (0) root         (0)     4267 2021-10-16 03:28:15.000000 FMLC-1.2.1/test/test_others.py
--rwxr-xr-x   0 root         (0) root         (0)    17675 2022-03-22 18:18:49.000000 FMLC-1.2.1/test/test_query_control.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-01 21:36:33.961983 FMLC-1.2.2/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-01 21:36:33.943490 FMLC-1.2.2/FMLC.egg-info/
+-rwxr-xr-x   0 root         (0) root         (0)     4711 2024-04-01 21:36:33.000000 FMLC-1.2.2/FMLC.egg-info/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)      428 2024-04-01 21:36:33.000000 FMLC-1.2.2/FMLC.egg-info/SOURCES.txt
+-rwxr-xr-x   0 root         (0) root         (0)        1 2024-04-01 21:36:33.000000 FMLC-1.2.2/FMLC.egg-info/dependency_links.txt
+-rwxr-xr-x   0 root         (0) root         (0)       22 2024-04-01 21:36:33.000000 FMLC-1.2.2/FMLC.egg-info/requires.txt
+-rwxr-xr-x   0 root         (0) root         (0)        5 2024-04-01 21:36:33.000000 FMLC-1.2.2/FMLC.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)     4711 2024-04-01 21:36:33.953534 FMLC-1.2.2/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     4194 2024-04-01 21:35:24.000000 FMLC-1.2.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-01 21:36:33.849860 FMLC-1.2.2/fmlc/
+-rwxr-xr-x   0 root         (0) root         (0)      178 2024-04-01 21:35:24.000000 FMLC-1.2.2/fmlc/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6467 2024-04-01 21:35:24.000000 FMLC-1.2.2/fmlc/baseclasses.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-01 21:36:33.887430 FMLC-1.2.2/fmlc/pythonDB/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 21:35:24.000000 FMLC-1.2.2/fmlc/pythonDB/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     3508 2024-04-01 21:35:24.000000 FMLC-1.2.2/fmlc/pythonDB/pythonDB.py
+-rwxr-xr-x   0 root         (0) root         (0)     3081 2024-04-01 21:35:24.000000 FMLC-1.2.2/fmlc/pythonDB/utility.py
+-rwxr-xr-x   0 root         (0) root         (0)    23619 2024-04-01 21:35:24.000000 FMLC-1.2.2/fmlc/stackedclasses.py
+-rwxr-xr-x   0 root         (0) root         (0)     3111 2024-04-01 21:35:24.000000 FMLC-1.2.2/fmlc/triggering.py
+-rwxr-xr-x   0 root         (0) root         (0)     1727 2024-04-01 21:35:24.000000 FMLC-1.2.2/fmlc/utility.py
+-rwxr-xr-x   0 root         (0) root         (0)     2440 2024-04-01 21:35:24.000000 FMLC-1.2.2/license.txt
+-rwxr-xr-x   0 root         (0) root         (0)       88 2024-04-01 21:35:24.000000 FMLC-1.2.2/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)       38 2024-04-01 21:36:33.964647 FMLC-1.2.2/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1135 2024-04-01 21:35:24.000000 FMLC-1.2.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-01 21:36:33.928526 FMLC-1.2.2/test/
+-rwxr-xr-x   0 root         (0) root         (0)      808 2024-04-01 21:35:24.000000 FMLC-1.2.2/test/test_baseclasses.py
+-rwxr-xr-x   0 root         (0) root         (0)     4144 2024-04-01 21:35:24.000000 FMLC-1.2.2/test/test_others.py
+-rwxr-xr-x   0 root         (0) root         (0)    17311 2024-04-01 21:35:24.000000 FMLC-1.2.2/test/test_query_control.py
```

### Comparing `FMLC-1.2.1/FMLC.egg-info/PKG-INFO` & `FMLC-1.2.2/FMLC.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: FMLC
-Version: 1.2.1
+Version: 1.2.2
 Summary: A framework/backend for multi-layer and multi-time domain controller.
 Home-page: https://github.com/LBNL-ETA/FMLC
 Author: Gehbauer, Christoph
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/LBNL-ETA/FMLC/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: license.txt
+Requires-Dist: pandas
+Requires-Dist: requests
+Requires-Dist: numpy
 
 # FMLC
-![Actions Status](https://github.com/LBNL-ETA/FMLC/workflows/Python%20application/badge.svg)
+[![Actions Status](https://github.com/LBNL-ETA/FMLC/actions/workflows/python-app.yml/badge.svg)](https://github.com/LBNL-ETA/FMLC/actions/workflows/python-app.yml)
+
 #### Framework for Multi Layer Control in Python
 -------------------------------------------------------------------------
 
 This package is developed to serve as a framework for control applications (microgrid control, building automation, energy management, electric vehicle fleet aggregation, etc.). In particular, this framework is built to handle the parallelization, timing/triggering, data logging, and error handling of multiple controller modules.
 
 ## General
 This package is developed as a framework/backend for multi-layer and multi-time domain controller. One example application are advanced controller based on [Model Predictive Control](https://en.wikipedia.org/wiki/Model_predictive_control) (MPC) where different sub-modules (e.g., weather forecast, energy management, real-time control), with different time constants, have to be coordinated. This framework allows parallelization using the `multiprocessing` module in Python.
@@ -52,9 +55,7 @@
 
 NOTICE.  This Software was developed under funding from the U.S. Department of Energy and the U.S. Government consequently retains certain rights.  As such, the U.S. Government has been granted for itself and others acting on its behalf a paid-up, nonexclusive, irrevocable, worldwide license in the Software to reproduce, distribute copies to the public, prepare derivative works, and perform publicly and display publicly, and to permit other to do so.
 
 ## Cite
 To cite the FMLC package, please use:
 
 *Gehbauer, Christoph, Müller, J., Swenson, T. and Vrettos, E. 2019. Photovoltaic and Behind-the-Meter Battery Storage: Advanced Smart Inverter Controls and Field Demonstration. California Energy Commission.*
-
-
```

### Comparing `FMLC-1.2.1/PKG-INFO` & `FMLC-1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: FMLC
-Version: 1.2.1
+Version: 1.2.2
 Summary: A framework/backend for multi-layer and multi-time domain controller.
 Home-page: https://github.com/LBNL-ETA/FMLC
 Author: Gehbauer, Christoph
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/LBNL-ETA/FMLC/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: license.txt
+Requires-Dist: pandas
+Requires-Dist: requests
+Requires-Dist: numpy
 
 # FMLC
-![Actions Status](https://github.com/LBNL-ETA/FMLC/workflows/Python%20application/badge.svg)
+[![Actions Status](https://github.com/LBNL-ETA/FMLC/actions/workflows/python-app.yml/badge.svg)](https://github.com/LBNL-ETA/FMLC/actions/workflows/python-app.yml)
+
 #### Framework for Multi Layer Control in Python
 -------------------------------------------------------------------------
 
 This package is developed to serve as a framework for control applications (microgrid control, building automation, energy management, electric vehicle fleet aggregation, etc.). In particular, this framework is built to handle the parallelization, timing/triggering, data logging, and error handling of multiple controller modules.
 
 ## General
 This package is developed as a framework/backend for multi-layer and multi-time domain controller. One example application are advanced controller based on [Model Predictive Control](https://en.wikipedia.org/wiki/Model_predictive_control) (MPC) where different sub-modules (e.g., weather forecast, energy management, real-time control), with different time constants, have to be coordinated. This framework allows parallelization using the `multiprocessing` module in Python.
@@ -52,9 +55,7 @@
 
 NOTICE.  This Software was developed under funding from the U.S. Department of Energy and the U.S. Government consequently retains certain rights.  As such, the U.S. Government has been granted for itself and others acting on its behalf a paid-up, nonexclusive, irrevocable, worldwide license in the Software to reproduce, distribute copies to the public, prepare derivative works, and perform publicly and display publicly, and to permit other to do so.
 
 ## Cite
 To cite the FMLC package, please use:
 
 *Gehbauer, Christoph, Müller, J., Swenson, T. and Vrettos, E. 2019. Photovoltaic and Behind-the-Meter Battery Storage: Advanced Smart Inverter Controls and Field Demonstration. California Energy Commission.*
-
-
```

### Comparing `FMLC-1.2.1/README.md` & `FMLC-1.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-# FMLC
-![Actions Status](https://github.com/LBNL-ETA/FMLC/workflows/Python%20application/badge.svg)
-#### Framework for Multi Layer Control in Python
--------------------------------------------------------------------------
-
-This package is developed to serve as a framework for control applications (microgrid control, building automation, energy management, electric vehicle fleet aggregation, etc.). In particular, this framework is built to handle the parallelization, timing/triggering, data logging, and error handling of multiple controller modules.
-
-## General
-This package is developed as a framework/backend for multi-layer and multi-time domain controller. One example application are advanced controller based on [Model Predictive Control](https://en.wikipedia.org/wiki/Model_predictive_control) (MPC) where different sub-modules (e.g., weather forecast, energy management, real-time control), with different time constants, have to be coordinated. This framework allows parallelization using the `multiprocessing` module in Python.
-
-*Please note that the FMLC package and especially the examples are still under development. Please open an issue for specific questions*
-
-## Getting Started
-The following link permits users to clone the source directory containing the [FMLC](https://github.com/LBNL-ETA/FMLC) package.
-
-The package depends on external modules which can be installed from pypi with `pip install -r requirements.txt`.
-
-This [file](https://github.com/LBNL-ETA/FMLC/blob/master/documentation/baseclass.md) contains a detailed documentation of how to use `baseclasses.py` to create controller objects.   
-The `stackedclasses.py` is a Python script to handle the parallelization, timing/triggering, data logging, and error handling of multiple controller modules. Its detailed documentation can be found [here](https://github.com/LBNL-ETA/FMLC/blob/master/documentation/stackedclasses.md).    
-A complete example can be found [here](https://github.com/LBNL-ETA/FMLC/blob/master/examples/Test.ipynb).   
-
-## Example
-To illustrate and test its functionality, each module executes some tests, when called as `main`.
-
-The `python triggering.py` command provides an example of the interal triggering of modules, while the `python baseclasses.py` command provides a simple example of a single controller.
-
-Further, and example Jupyter notebook can be found [here](https://github.com/LBNL-ETA/FMLC/tree/master/examples) where a full controller stack, with different time constants, is illustrated. Please note that in order to work properly on Windows, the notebook must be exported to Python code.
-
-Another application example can be found [here](https://github.com/LBNL-ETA/DOPER) where FMLC is used to coordiante MPC controls on three differernt time domains:
-* Day-ahead control: invoked once per day; complex model
-* Supervisory energy management: invoked every 5 minutes with a 24 hour horizon
-* Fast-acting control: invoked every second with an hourly horizon 
-
-## License
-Framework for Multi Layer Control in Python (FMLC) Copyright (c) 2019, The Regents of the University of California, through Lawrence Berkeley National Laboratory (subject to receipt of any required approvals from the U.S. Dept. of Energy).  All rights reserved.
-
-If you have questions about your rights to use or distribute this software, please contact Berkeley Lab's Intellectual Property Office at IPO@lbl.gov.
-
-NOTICE.  This Software was developed under funding from the U.S. Department of Energy and the U.S. Government consequently retains certain rights.  As such, the U.S. Government has been granted for itself and others acting on its behalf a paid-up, nonexclusive, irrevocable, worldwide license in the Software to reproduce, distribute copies to the public, prepare derivative works, and perform publicly and display publicly, and to permit other to do so.
-
-## Cite
-To cite the FMLC package, please use:
-
-*Gehbauer, Christoph, Müller, J., Swenson, T. and Vrettos, E. 2019. Photovoltaic and Behind-the-Meter Battery Storage: Advanced Smart Inverter Controls and Field Demonstration. California Energy Commission.*
+# FMLC
+[![Actions Status](https://github.com/LBNL-ETA/FMLC/actions/workflows/python-app.yml/badge.svg)](https://github.com/LBNL-ETA/FMLC/actions/workflows/python-app.yml)
+
+#### Framework for Multi Layer Control in Python
+-------------------------------------------------------------------------
+
+This package is developed to serve as a framework for control applications (microgrid control, building automation, energy management, electric vehicle fleet aggregation, etc.). In particular, this framework is built to handle the parallelization, timing/triggering, data logging, and error handling of multiple controller modules.
+
+## General
+This package is developed as a framework/backend for multi-layer and multi-time domain controller. One example application are advanced controller based on [Model Predictive Control](https://en.wikipedia.org/wiki/Model_predictive_control) (MPC) where different sub-modules (e.g., weather forecast, energy management, real-time control), with different time constants, have to be coordinated. This framework allows parallelization using the `multiprocessing` module in Python.
+
+*Please note that the FMLC package and especially the examples are still under development. Please open an issue for specific questions*
+
+## Getting Started
+The following link permits users to clone the source directory containing the [FMLC](https://github.com/LBNL-ETA/FMLC) package.
+
+The package depends on external modules which can be installed from pypi with `pip install -r requirements.txt`.
+
+This [file](https://github.com/LBNL-ETA/FMLC/blob/master/documentation/baseclass.md) contains a detailed documentation of how to use `baseclasses.py` to create controller objects.   
+The `stackedclasses.py` is a Python script to handle the parallelization, timing/triggering, data logging, and error handling of multiple controller modules. Its detailed documentation can be found [here](https://github.com/LBNL-ETA/FMLC/blob/master/documentation/stackedclasses.md).    
+A complete example can be found [here](https://github.com/LBNL-ETA/FMLC/blob/master/examples/Test.ipynb).   
+
+## Example
+To illustrate and test its functionality, each module executes some tests, when called as `main`.
+
+The `python triggering.py` command provides an example of the interal triggering of modules, while the `python baseclasses.py` command provides a simple example of a single controller.
+
+Further, and example Jupyter notebook can be found [here](https://github.com/LBNL-ETA/FMLC/tree/master/examples) where a full controller stack, with different time constants, is illustrated. Please note that in order to work properly on Windows, the notebook must be exported to Python code.
+
+Another application example can be found [here](https://github.com/LBNL-ETA/DOPER) where FMLC is used to coordiante MPC controls on three differernt time domains:
+* Day-ahead control: invoked once per day; complex model
+* Supervisory energy management: invoked every 5 minutes with a 24 hour horizon
+* Fast-acting control: invoked every second with an hourly horizon 
+
+## License
+Framework for Multi Layer Control in Python (FMLC) Copyright (c) 2019, The Regents of the University of California, through Lawrence Berkeley National Laboratory (subject to receipt of any required approvals from the U.S. Dept. of Energy).  All rights reserved.
+
+If you have questions about your rights to use or distribute this software, please contact Berkeley Lab's Intellectual Property Office at IPO@lbl.gov.
+
+NOTICE.  This Software was developed under funding from the U.S. Department of Energy and the U.S. Government consequently retains certain rights.  As such, the U.S. Government has been granted for itself and others acting on its behalf a paid-up, nonexclusive, irrevocable, worldwide license in the Software to reproduce, distribute copies to the public, prepare derivative works, and perform publicly and display publicly, and to permit other to do so.
+
+## Cite
+To cite the FMLC package, please use:
+
+*Gehbauer, Christoph, Müller, J., Swenson, T. and Vrettos, E. 2019. Photovoltaic and Behind-the-Meter Battery Storage: Advanced Smart Inverter Controls and Field Demonstration. California Energy Commission.*
```

### Comparing `FMLC-1.2.1/fmlc/pythonDB/pythonDB.py` & `FMLC-1.2.2/fmlc/pythonDB/pythonDB.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-#! /usr/bin/env python
-
-'''
-This module is part of the FMLC package.
-https://github.com/LBNL-ETA/FMLC
-'''
-
-try:
-    # For Python 3.0 and later
-    from socketserver import TCPServer
-except ImportError:
-    # Fall back to Python 2
-    from SocketServer import TCPServer
-    
-try:
-    # For Python 3.0 and later
-    from http.server import BaseHTTPRequestHandler
-except ImportError:
-    # Fall back to Python 2
-    from BaseHTTPServer import BaseHTTPRequestHandler
-
-from json import dumps, loads
-from datetime import datetime
-from os import path
-import csv
-import sys
-from time import sleep, time, gmtime, mktime
-
-def status(self):
-	self.send_response(200)
-	self.send_header("Content-type", "text/html")
-	self.end_headers()
-	
-	temp = {}
-	temp['dev_status'] = db['dev_status']
-	temp['dev_time'] = db['dev_time']
-	temp['dev_debug'] = str(db['dev_debug'])
-	temp['dev_nodename'] = db['dev_nodename']
-	temp['dev_error'] = db['dev_error']
-	json_file = dumps(temp, sort_keys=True, separators=(',', ': ')).encode()
-	self.wfile.write(json_file)
-	
-def write(self, new=True, store=True):
-	if new:
-		self.send_response(200)
-		self.send_header("Content-type", "text/html")
-		self.end_headers()
-		#read new data and update dict
-		try:
-			# python 3        
-			length = int(self.headers['Content-Length'])
-		except:
-			# python 2
-			length = int(self.headers.getheader('content-length'))
-		dict = loads(self.rfile.read(length))
-		db.update(dict)
-	#store in csv file
-	if store:
-		with open(db_name, 'wb') as f:
-			for key in sorted(db.keys()):
-				csv.writer(f).writerow([key, db[key]])
-	
-def read(self):
-	self.send_response(200)
-	self.send_header("Content-type", "text/html")
-	self.end_headers()
-	#print 'Header', time()
-	#send full db as json file
-	json_file = dumps(db, sort_keys=True, separators=(',', ': ')).encode()
-	self.wfile.write(json_file)
-	#print 'Payload', time()
-	
-class MyHandler(BaseHTTPRequestHandler):
-	def log_message(self, format, *args):
-		if db['dev_debug']:
-			sys.stderr.write("%s - - [%s] %s\n" %
-						 (self.address_string(),
-						  self.log_date_time_string(),
-						  format%args))
-		else: pass
-	def do_GET(self):
-		#print 'Receive', time()
-		db['dev_time'] = datetime.now().strftime(format)
-		if self.path == '/read':
-			read(self)
-		elif self.path == '/status':
-			status(self)			
-		else:
-			if db['dev_debug']: self.send_error(404)
-			else: pass
-		write(self, new=False, store=False)
-	def do_PUT(self):
-		db['dev_time'] = datetime.now().strftime(format)
-		if self.path == '/write':
-			write(self, store=False)
-		else:
-			if db['dev_debug']: self.send_error(404)
-			else: pass
-
-if __name__ == '__main__':
-    #load database
-    db = {}
-    db['dev_nodename'] = sys.argv[1]
-    db_name = db['dev_nodename']+'.csv'
-    format = '%Y-%m-%d %H:%M:%S'
-    if len(sys.argv) > 3: db_name = sys.argv[3]+'/'+db_name
-    if path.isfile(db_name):
-        with open(db_name, 'rb') as f:
-            for row in csv.reader(f):
-                try: db[row[0]] = row[1]
-                except: pass
-    db['dev_nodename'] = sys.argv[1]
-    db['dev_port'] = sys.argv[2]
-    db['dev_debug'] = False
-    db['dev_status'] = "starting"
-    db['dev_error'] = 'NA'
-    db['timezone'] = int(int(mktime(gmtime())-time())/60/60)*-1
-    print("Starting Python_db for "+db['dev_nodename']+' on port '+str(db['dev_port'])+'...')
-    httpd = TCPServer(("", int(db['dev_port'])), MyHandler)
-    db['dev_status'] = "ok"
-    print(db['dev_status'])
-    db['dev_time'] = datetime.now().strftime(format)
-    httpd.serve_forever()
+#! /usr/bin/env python
+
+'''
+This module is part of the FMLC package.
+https://github.com/LBNL-ETA/FMLC
+'''
+
+try:
+    # For Python 3.0 and later
+    from socketserver import TCPServer
+except ImportError:
+    # Fall back to Python 2
+    from SocketServer import TCPServer
+    
+try:
+    # For Python 3.0 and later
+    from http.server import BaseHTTPRequestHandler
+except ImportError:
+    # Fall back to Python 2
+    from BaseHTTPServer import BaseHTTPRequestHandler
+
+from json import dumps, loads
+from datetime import datetime
+from os import path
+import csv
+import sys
+from time import sleep, time, gmtime, mktime
+
+def status(self):
+	self.send_response(200)
+	self.send_header("Content-type", "text/html")
+	self.end_headers()
+	
+	temp = {}
+	temp['dev_status'] = db['dev_status']
+	temp['dev_time'] = db['dev_time']
+	temp['dev_debug'] = str(db['dev_debug'])
+	temp['dev_nodename'] = db['dev_nodename']
+	temp['dev_error'] = db['dev_error']
+	json_file = dumps(temp, sort_keys=True, separators=(',', ': ')).encode()
+	self.wfile.write(json_file)
+	
+def write(self, new=True, store=True):
+	if new:
+		self.send_response(200)
+		self.send_header("Content-type", "text/html")
+		self.end_headers()
+		#read new data and update dict
+		try:
+			# python 3        
+			length = int(self.headers['Content-Length'])
+		except:
+			# python 2
+			length = int(self.headers.getheader('content-length'))
+		dict = loads(self.rfile.read(length))
+		db.update(dict)
+	#store in csv file
+	if store:
+		with open(db_name, 'wb') as f:
+			for key in sorted(db.keys()):
+				csv.writer(f).writerow([key, db[key]])
+	
+def read(self):
+	self.send_response(200)
+	self.send_header("Content-type", "text/html")
+	self.end_headers()
+	#print 'Header', time()
+	#send full db as json file
+	json_file = dumps(db, sort_keys=True, separators=(',', ': ')).encode()
+	self.wfile.write(json_file)
+	#print 'Payload', time()
+	
+class MyHandler(BaseHTTPRequestHandler):
+	def log_message(self, format, *args):
+		if db['dev_debug']:
+			sys.stderr.write("%s - - [%s] %s\n" %
+						 (self.address_string(),
+						  self.log_date_time_string(),
+						  format%args))
+		else: pass
+	def do_GET(self):
+		#print 'Receive', time()
+		db['dev_time'] = datetime.now().strftime(format)
+		if self.path == '/read':
+			read(self)
+		elif self.path == '/status':
+			status(self)			
+		else:
+			if db['dev_debug']: self.send_error(404)
+			else: pass
+		write(self, new=False, store=False)
+	def do_PUT(self):
+		db['dev_time'] = datetime.now().strftime(format)
+		if self.path == '/write':
+			write(self, store=False)
+		else:
+			if db['dev_debug']: self.send_error(404)
+			else: pass
+
+if __name__ == '__main__':
+    #load database
+    db = {}
+    db['dev_nodename'] = sys.argv[1]
+    db_name = db['dev_nodename']+'.csv'
+    format = '%Y-%m-%d %H:%M:%S'
+    if len(sys.argv) > 3: db_name = sys.argv[3]+'/'+db_name
+    if path.isfile(db_name):
+        with open(db_name, 'rb') as f:
+            for row in csv.reader(f):
+                try: db[row[0]] = row[1]
+                except: pass
+    db['dev_nodename'] = sys.argv[1]
+    db['dev_port'] = sys.argv[2]
+    db['dev_debug'] = False
+    db['dev_status'] = "starting"
+    db['dev_error'] = 'NA'
+    db['timezone'] = int(int(mktime(gmtime())-time())/60/60)*-1
+    print("Starting Python_db for "+db['dev_nodename']+' on port '+str(db['dev_port'])+'...')
+    httpd = TCPServer(("", int(db['dev_port'])), MyHandler)
+    db['dev_status'] = "ok"
+    print(db['dev_status'])
+    db['dev_time'] = datetime.now().strftime(format)
+    httpd.serve_forever()
```

### Comparing `FMLC-1.2.1/fmlc/pythonDB/utility.py` & `FMLC-1.2.2/fmlc/pythonDB/utility.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,92 +1,97 @@
-#! /usr/bin/env python
-
-'''
-This module is part of the FMLC package.
-https://github.com/LBNL-ETA/FMLC
-'''
-
-try:
-    # For Python 3.0 and later
-    from urllib.request import urlopen
-except ImportError:
-    # Fall back to Python 2's urllib2
-    from urllib2 import urlopen
-import os
-import signal
-from time import sleep
-import subprocess as sp
-import random
-import requests
-import json
-
-def write_db(dict, add_db):
-    try:
-        return requests.put('http://'+add_db+'/write', data=str(json.dumps(dict, sort_keys=True, separators=(',', ': '))))
-    except Exception as e:
-        return f'ERROR: {e}'
-
-def read_db(add_db):
-    try:
-        return json.loads(requests.get('http://'+add_db+'/read', verify=False).text.encode('ascii','ignore'))
-    except Exception as e:
-        return f'ERROR: {e}'
-    
-class PythonDB_wrapper(object):
-    def __init__ (self, name, mode='pythonDB', path=''):
-        self.root_dir = os.path.dirname(os.path.realpath(__file__))
-        self.name = name
-        self.mode = mode
-        self.filepath = path
-        self.error = ''
-        self.start_db()
-        self.test_db()
-
-    def start_db(self):
-        # Determine Python command
-        for pcmd in ['python', 'python3', 'python2']:
-            try:
-                sp.call([pcmd, '-c', 'exit()'])
-                break
-            except:
-                pass
-        i = 0		
-        while i < 4:
-            self.port = random.randint(10000,60000)
-            sp.Popen('{} {}.py {} {} {}'.format(pcmd, self.root_dir+'/'+self.mode, self.name, str(self.port), self.filepath), shell=True)
-            sleep(2)
-            i += self.test_db()
-        if self.test_db() != 999:
-            self.port = 0
-            self.error += 'Cannot find open port for '+self.name
-
-    def test_db(self):
-        try:
-            response = urlopen('http://127.0.0.1:'+str(self.port)+'/status', timeout=1).read()
-            if 'ok' in str(response):
-                return 999
-            else:
-                return 1
-        except:
-            return 1
-
-    def kill_db(self):
-        # Works only on Linux environment
-        pids = sp.Popen("ps aux | grep '"+self.name+"' | awk '{print $2, $13}'", shell=True, stdout=sp.PIPE)
-        out, err = pids.communicate()
-        for line in out.splitlines():
-            line = line.split(b' ')
-            if line[1].decode() == self.name:
-                sp.call(f'echo "Closing {self.mode} for {self.name}."', shell=True)
-                os.kill(int(line[0]), signal.SIGKILL)
-
-if __name__ == '__main__':
-    from time import time
-    name = 'Zone1_db_test'
-    mode = 'pythonDB'
-    testdb = PythonDB_wrapper(name, mode)
-    print(testdb.port)
-    time_st = time()
-    print('Request', time())
-    response = urlopen('http://127.0.0.1:'+str(testdb.port)+'/read', timeout=10).read()
-    print('Latency:', time()-time_st)
-    testdb.kill_db()
+#! /usr/bin/env python
+
+'''
+This module is part of the FMLC package.
+https://github.com/LBNL-ETA/FMLC
+'''
+
+try:
+    # For Python 3.0 and later
+    from urllib.request import urlopen
+except ImportError:
+    # Fall back to Python 2's urllib2
+    from urllib2 import urlopen
+import os
+import signal
+from time import sleep
+import subprocess as sp
+import random
+import requests
+import json
+import traceback
+
+SLEEP_TIME = 2   # seconds
+MAX_ATTEMPTS = 4 # max attempts to start database
+
+def write_db(dict, add_db):
+    try:
+        return requests.put('http://'+add_db+'/write', data=str(json.dumps(dict, sort_keys=True, separators=(',', ': '))))
+    except Exception as e:
+        return f'ERROR: {e}.\n\n{traceback.format_exc()}'
+
+def read_db(add_db):
+    try:
+        return json.loads(requests.get('http://'+add_db+'/read', verify=False).text.encode('ascii','ignore'))
+    except Exception as e:
+        return f'ERROR: {e}'
+    
+class PythonDB_wrapper(object):
+    def __init__ (self, name, mode='pythonDB', path=''):
+        self.root_dir = os.path.dirname(os.path.realpath(__file__))
+        self.name = name
+        self.mode = mode
+        self.filepath = path
+        self.error = ''
+        self.start_db()
+
+    def start_db(self):
+        # Determine Python command
+        for pcmd in ['python', 'python3', 'python2']:
+            try:
+                sp.call([pcmd, '-c', 'exit()'])
+                break
+            except:
+                pass
+        i = 0		
+        while i < MAX_ATTEMPTS:
+            self.port = random.randint(10000, 60000)
+            sp.Popen('{} {}.py {} {} {}'.format(pcmd, self.root_dir+'/'+self.mode, self.name, str(self.port), self.filepath), shell=True)
+            sleep(SLEEP_TIME)
+            i += self.test_db()
+        sleep(SLEEP_TIME/2)
+        if self.test_db() != 999:
+            self.port = 0
+            self.error += 'Cannot find open port for '+self.name
+
+    def test_db(self):
+        try:
+            response = urlopen('http://127.0.0.1:'+str(self.port)+'/status', timeout=1).read()
+            response = json.loads(response)
+            if response['dev_nodename'] == self.name:
+                return 999
+            else:
+                return 1
+        except:
+            return 1
+
+    def kill_db(self):
+        # Works only on Linux environment
+        pids = sp.Popen("ps aux | grep '"+self.name+"' | awk '{print $2, $13}'", shell=True, stdout=sp.PIPE)
+        out, err = pids.communicate()
+        for line in out.splitlines():
+            line = line.split(b' ')
+            if line[1].decode() == self.name:
+                sp.call(f'echo "Closing {self.mode} for {self.name}."', shell=True)
+                os.kill(int(line[0]), signal.SIGKILL)
+
+if __name__ == '__main__':
+    from time import time
+    name = 'Zone1_db_test'
+    mode = 'pythonDB'
+    testdb = PythonDB_wrapper(name, mode)
+    print(testdb.port)
+    time_st = time()
+    print('Request', time())
+    response = urlopen('http://127.0.0.1:'+str(testdb.port)+'/read', timeout=10).read()
+    print('Latency:', time()-time_st)
+    testdb.kill_db()
```

### Comparing `FMLC-1.2.1/fmlc/triggering.py` & `FMLC-1.2.2/fmlc/triggering.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-#! /usr/bin/env python
-
-'''
-This module is part of the FMLC package.
-https://github.com/LBNL-ETA/FMLC
-'''
-
-import time
-
-class triggering(object):
-    '''
-    Class to handle internal triggering of models.
-    '''
-    def __init__(self, ts, init_now=False):
-        '''
-        Input
-        -----
-        ts (dict): Timesteps for triggering with timestep in seconds.
-        init_now (bool): Initialize with current timestep. This is not 
-            recommended as timesteps are not aligned. Good for testing and 
-            debugging. (Default = False)
-        '''
-        self.ts = ts
-        self.init_now = init_now
-        self._initialize_all_trigger() 
-
-    def _initialize_all_trigger(self):
-        '''
-        Initializaiton of all triggers.        
-        '''
-        now = time.time()
-        self.trigger = {}
-        mode = 'prev' if self.init_now else 'next'
-        for k in self.ts.keys():
-            self.trigger[k] = self._get_trigger(self.ts[k], now, mode=mode,
-                                                integer=(self.ts[k]%1) == 0)
-
-    def refresh_trigger(self, name, now=time.time()):
-        '''
-        Refresh the trigger.
-        
-        Input
-        -----
-        name (str): Name of the trigger.
-        now (time.time): Current time to refresh. (Default = time.time())
-        '''
-        self.trigger[name] = self._get_trigger(self.ts[name], now, mode='next',
-                                               integer=(self.ts[name]%1) == 0)
-
-    def _get_trigger(self, ts, now=time.time(), mode='next', integer=False):
-        '''
-        Get the current trigger value.
-        
-        Input
-        -----
-        ts (float): The timestep of the trigger.
-        now (time.time): Current time to refresh. (Default = time.time())
-        mode (str): Mode of calculation, either "next" or "prev".
-            (Default = "next")
-        integer (bool): Round seconds to full integer.
-            Recommended when ts > 10 s. (Defualt = False)
-            
-        Return
-        ------
-        trigger (float): Next trigger as timestamp.
-        '''
-        trigger = round(now/ts) * ts
-        if integer:
-            trigger = int(trigger)
-        if mode == 'next':
-            trigger = trigger + ts
-        elif mode == 'prev':
-            trigger = trigger - ts
-        else:
-            print('ERROR: "mode" must be "next" or "prev"')
-        return trigger
-        
-if __name__ == '__main__':
-    ts = {} 
-    ts['main'] = 0.5 # seconds
-    ts['print'] = 1
-    print('"Main" should be triggered every {} s.'.format(ts['main']))
-    print('"Print" should be triggered every {} s.'.format(ts['print']))
-    trigger_test = triggering(ts)
-    now_init = time.time()
-    now = now_init
-    while now < now_init+3:
-        now = time.time()
-        if now >= trigger_test.trigger['main']:
-            print('Main triggered\t{}'.format(round(now, 2)))
-            trigger_test.refresh_trigger('main', now)
-        if now >= trigger_test.trigger['print']:
-            print('Print triggered\t{}'.format(round(now, 2)))
+#! /usr/bin/env python
+
+'''
+This module is part of the FMLC package.
+https://github.com/LBNL-ETA/FMLC
+'''
+
+import time
+
+class triggering(object):
+    '''
+    Class to handle internal triggering of models.
+    '''
+    def __init__(self, ts, init_now=False):
+        '''
+        Input
+        -----
+        ts (dict): Timesteps for triggering with timestep in seconds.
+        init_now (bool): Initialize with current timestep. This is not 
+            recommended as timesteps are not aligned. Good for testing and 
+            debugging. (Default = False)
+        '''
+        self.ts = ts
+        self.init_now = init_now
+        self._initialize_all_trigger() 
+
+    def _initialize_all_trigger(self):
+        '''
+        Initializaiton of all triggers.        
+        '''
+        now = time.time()
+        self.trigger = {}
+        mode = 'prev' if self.init_now else 'next'
+        for k in self.ts.keys():
+            self.trigger[k] = self._get_trigger(self.ts[k], now, mode=mode,
+                                                integer=(self.ts[k]%1) == 0)
+
+    def refresh_trigger(self, name, now=time.time()):
+        '''
+        Refresh the trigger.
+        
+        Input
+        -----
+        name (str): Name of the trigger.
+        now (time.time): Current time to refresh. (Default = time.time())
+        '''
+        self.trigger[name] = self._get_trigger(self.ts[name], now, mode='next',
+                                               integer=(self.ts[name]%1) == 0)
+
+    def _get_trigger(self, ts, now=time.time(), mode='next', integer=False):
+        '''
+        Get the current trigger value.
+        
+        Input
+        -----
+        ts (float): The timestep of the trigger.
+        now (time.time): Current time to refresh. (Default = time.time())
+        mode (str): Mode of calculation, either "next" or "prev".
+            (Default = "next")
+        integer (bool): Round seconds to full integer.
+            Recommended when ts > 10 s. (Defualt = False)
+            
+        Return
+        ------
+        trigger (float): Next trigger as timestamp.
+        '''
+        trigger = round(now/ts) * ts
+        if integer:
+            trigger = int(trigger)
+        if mode == 'next':
+            trigger = trigger + ts
+        elif mode == 'prev':
+            trigger = trigger - ts
+        else:
+            print('ERROR: "mode" must be "next" or "prev"')
+        return trigger
+        
+if __name__ == '__main__':
+    ts = {} 
+    ts['main'] = 0.5 # seconds
+    ts['print'] = 1
+    print('"Main" should be triggered every {} s.'.format(ts['main']))
+    print('"Print" should be triggered every {} s.'.format(ts['print']))
+    trigger_test = triggering(ts)
+    now_init = time.time()
+    now = now_init
+    while now < now_init+3:
+        now = time.time()
+        if now >= trigger_test.trigger['main']:
+            print('Main triggered\t{}'.format(round(now, 2)))
+            trigger_test.refresh_trigger('main', now)
+        if now >= trigger_test.trigger['print']:
+            print('Print triggered\t{}'.format(round(now, 2)))
             trigger_test.refresh_trigger('print', now)
```

### Comparing `FMLC-1.2.1/test/test_others.py` & `FMLC-1.2.2/test/test_others.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-import sys
-import time
-from os import path
-
-sys.path.append(path.dirname(path.dirname(path.abspath(__file__))))
-from fmlc.triggering import triggering
-from fmlc.baseclasses import eFMU
-from fmlc.stackedclasses import controller_stack
-
-class testcontroller1(eFMU):
-    def __init__(self):
-        self.input = {'a': None, 'b': None}
-        self.output = {'c': None}
-        self.init = True
-    def compute(self):
-        self.init= False
-        self.output['c'] = self.input['a'] * self.input['b']
-        return 'testcontroller1 did a computation!'
-
-
-class testcontroller2(eFMU):
-    def __init__(self):
-        self.input = {'a': None, 'b': None}
-        self.output = {'c': None}
-        self.init = True
-
-    def compute(self):
-        self.init = False
-        self.output['c'] = self.input['a'] * self.input['b']
-        time.sleep(0.2)
-        return 'testcontroller2 did a computation!'
-
-class testcontroller3(eFMU):
-    def __init__(self):
-        self.input = {'a': None, 'b': None}
-        self.output = {'c': None}
-        self.init = True
-
-    def compute(self):
-        self.init = False
-        self.output['c'] = self.input['a'] * self.input['b']
-        time.sleep(1)
-        return 'testcontroller3 did a computation!'
-
-class testcontroller4(eFMU):
-    def __init__(self):
-        self.input = {'a': None, 'b': None}
-        self.output = {'c': None}
-        self.init = True
-
-    def compute(self):
-        self.init = False
-        self.output['c'] = self.input['a'] * self.input['b']
-        time.sleep(10)
-        return 'testcontroller4 did a computation!'
-
-def test_input_errors():
-    ##CASE1: not all inputs are set.
-    controller = {}
-    controller['forecast1'] = {'function':testcontroller1, 'sampletime':0}
-    controller['mpc1'] = {'function':testcontroller2, 'sampletime':'forecast1'}
-    controller['control1'] = {'function':testcontroller1, 'sampletime':'mpc1'}
-    controller['forecast2'] = {'function':testcontroller3, 'sampletime':0}
-    controller['forecast3'] = {'function':testcontroller1, 'sampletime':0}
-
-    mapping = {}
-    mapping['forecast1_a'] = 10
-    mapping['forecast1_b'] = 4
-    mapping['forecast2_a'] = 20
-    mapping['forecast2_b'] = 4
-    mapping['forecast3_a'] = 30
-    mapping['forecast3_b'] = 4
-    mapping['mpc1_b'] = 'forecast1_a'
-    mapping['control1_a'] = 'mpc1_c'
-    try:
-        controller = controller_stack(controller, mapping, tz=-8, debug=True, parallel=True, timeout=2)
-        AssertionError
-    except KeyError as e:
-        assert 'mapping' in str(e)
-    except:
-        AssertionError
-
-    ##CASE1: not all given inputs are valid inputs (extra inputs)
-    controller = {}
-    controller['forecast1'] = {'function':testcontroller1, 'sampletime':0}
-    controller['mpc1'] = {'function':testcontroller2, 'sampletime':'forecast1'}
-    controller['control1'] = {'function':testcontroller1, 'sampletime':'mpc1'}
-    controller['forecast2'] = {'function':testcontroller3, 'sampletime':0}
-    controller['forecast3'] = {'function':testcontroller1, 'sampletime':0}
-
-    mapping = {}
-    mapping['forecast1_d'] = 10
-    mapping['forecast1_a'] = 10
-    mapping['forecast1_b'] = 4
-    mapping['forecast2_a'] = 20
-    mapping['forecast2_b'] = 4
-    mapping['forecast3_a'] = 30
-    mapping['forecast3_b'] = 4
-    mapping['mpc1_a'] = 'forecast1_c'
-    mapping['mpc1_b'] = 'forecast1_a'
-    mapping['control1_a'] = 'mpc1_c'
-    mapping['control1_b'] = 'mpc1_a'
-    try:
-        controller = controller_stack(controller, mapping, tz=-8, debug=True, parallel=True, timeout=2)
-        AssertionError
-    except KeyError as e:
-        assert 'parameter' in str(e)
-    except:
-        AssertionError
-
-def test_init_once():
-    controller = {}
-    controller['forecast1'] = {'function':testcontroller1, 'sampletime':0}
-
-    mapping = {}
-    mapping['forecast1_a'] = 10
-    mapping['forecast1_b'] = 4
-    controller = controller_stack(controller, mapping, tz=-8, debug=True, parallel=True, timeout=2)
-
-    obj = controller.controller_objects['forecast1']
-    for i in range(3):
-        controller.query_control(time.time())
-        assert controller.controller_objects['forecast1'] is obj
+import sys
+import time
+from os import path
+
+sys.path.append(path.dirname(path.dirname(path.abspath(__file__))))
+from fmlc.triggering import triggering
+from fmlc.baseclasses import eFMU
+from fmlc.stackedclasses import controller_stack
+
+class testcontroller1(eFMU):
+    def __init__(self):
+        self.input = {'a': None, 'b': None}
+        self.output = {'c': None}
+        self.init = True
+    def compute(self):
+        self.init= False
+        self.output['c'] = self.input['a'] * self.input['b']
+        return 'testcontroller1 did a computation!'
+
+
+class testcontroller2(eFMU):
+    def __init__(self):
+        self.input = {'a': None, 'b': None}
+        self.output = {'c': None}
+        self.init = True
+
+    def compute(self):
+        self.init = False
+        self.output['c'] = self.input['a'] * self.input['b']
+        time.sleep(0.2)
+        return 'testcontroller2 did a computation!'
+
+class testcontroller3(eFMU):
+    def __init__(self):
+        self.input = {'a': None, 'b': None}
+        self.output = {'c': None}
+        self.init = True
+
+    def compute(self):
+        self.init = False
+        self.output['c'] = self.input['a'] * self.input['b']
+        time.sleep(1)
+        return 'testcontroller3 did a computation!'
+
+class testcontroller4(eFMU):
+    def __init__(self):
+        self.input = {'a': None, 'b': None}
+        self.output = {'c': None}
+        self.init = True
+
+    def compute(self):
+        self.init = False
+        self.output['c'] = self.input['a'] * self.input['b']
+        time.sleep(10)
+        return 'testcontroller4 did a computation!'
+
+def test_input_errors():
+    ##CASE1: not all inputs are set.
+    controller = {}
+    controller['forecast1'] = {'function':testcontroller1, 'sampletime':0}
+    controller['mpc1'] = {'function':testcontroller2, 'sampletime':'forecast1'}
+    controller['control1'] = {'function':testcontroller1, 'sampletime':'mpc1'}
+    controller['forecast2'] = {'function':testcontroller3, 'sampletime':0}
+    controller['forecast3'] = {'function':testcontroller1, 'sampletime':0}
+
+    mapping = {}
+    mapping['forecast1_a'] = 10
+    mapping['forecast1_b'] = 4
+    mapping['forecast2_a'] = 20
+    mapping['forecast2_b'] = 4
+    mapping['forecast3_a'] = 30
+    mapping['forecast3_b'] = 4
+    mapping['mpc1_b'] = 'forecast1_a'
+    mapping['control1_a'] = 'mpc1_c'
+    try:
+        controller = controller_stack(controller, mapping, tz=-8, debug=True, parallel=True, timeout=2)
+        AssertionError
+    except KeyError as e:
+        assert 'mapping' in str(e)
+    except:
+        AssertionError
+
+    ##CASE1: not all given inputs are valid inputs (extra inputs)
+    controller = {}
+    controller['forecast1'] = {'function':testcontroller1, 'sampletime':0}
+    controller['mpc1'] = {'function':testcontroller2, 'sampletime':'forecast1'}
+    controller['control1'] = {'function':testcontroller1, 'sampletime':'mpc1'}
+    controller['forecast2'] = {'function':testcontroller3, 'sampletime':0}
+    controller['forecast3'] = {'function':testcontroller1, 'sampletime':0}
+
+    mapping = {}
+    mapping['forecast1_d'] = 10
+    mapping['forecast1_a'] = 10
+    mapping['forecast1_b'] = 4
+    mapping['forecast2_a'] = 20
+    mapping['forecast2_b'] = 4
+    mapping['forecast3_a'] = 30
+    mapping['forecast3_b'] = 4
+    mapping['mpc1_a'] = 'forecast1_c'
+    mapping['mpc1_b'] = 'forecast1_a'
+    mapping['control1_a'] = 'mpc1_c'
+    mapping['control1_b'] = 'mpc1_a'
+    try:
+        controller = controller_stack(controller, mapping, tz=-8, debug=True, parallel=True, timeout=2)
+        AssertionError
+    except KeyError as e:
+        assert 'parameter' in str(e)
+    except:
+        AssertionError
+
+def test_init_once():
+    controller = {}
+    controller['forecast1'] = {'function':testcontroller1, 'sampletime':0}
+
+    mapping = {}
+    mapping['forecast1_a'] = 10
+    mapping['forecast1_b'] = 4
+    controller = controller_stack(controller, mapping, tz=-8, debug=True, parallel=True, timeout=2)
+
+    obj = controller.controller_objects['forecast1']
+    for i in range(3):
+        controller.query_control(time.time())
+        assert controller.controller_objects['forecast1'] is obj
```

### Comparing `FMLC-1.2.1/test/test_query_control.py` & `FMLC-1.2.2/test/test_query_control.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,364 +1,364 @@
-import sys
-import time
-import math
-import warnings
-import numpy as np
-import pandas as pd
-from os import path
-
-sys.path.append(path.dirname(path.dirname(path.abspath(__file__))))
-from fmlc.triggering import triggering
-from fmlc.baseclasses import eFMU
-from fmlc.stackedclasses import controller_stack
-
-class testcontroller1(eFMU):
-    def __init__(self):
-        self.input = {'a': None, 'b': None}
-        self.output = {'c': None}
-        self.init = True
-    def compute(self):
-        self.init= False
-        self.output['c'] = self.input['a'] * self.input['b']
-        return 'testcontroller1 did a computation!'
-
-class testcontroller2(eFMU):
-    def __init__(self):
-        self.input = {'a': None, 'b': None}
-        self.output = {'c': None}
-        self.init = True
-
-    def compute(self):
-        self.init = False
-        self.output['c'] = self.input['a'] * self.input['b']
-        time.sleep(0.2)
-        return 'testcontroller2 did a computation!'
-
-class testcontroller3(eFMU):
-    def __init__(self):
-        self.input = {'a': None, 'b': None}
-        self.output = {'c': None}
-        self.init = True
-
-    def compute(self):
-        self.init = False
-        self.output['c'] = self.input['a'] * self.input['b']
-        time.sleep(1)
-        return 'testcontroller3 did a computation!'
-
-class testcontroller4(eFMU):
-    def __init__(self):
-        self.input = {'a': None, 'b': None}
-        self.output = {'c': None}
-        self.init = True
-
-    def compute(self):
-        self.init = False
-        self.output['c'] = self.input['a'] * self.input['b']
-        time.sleep(10)
-        return 'testcontroller4 did a computation!'
-        
-def test_sampletime():
-    '''This tests if the sample time is working properly'''
-    controller = {}
-    controller['forecast1'] = {'function': testcontroller1, 'sampletime': 3}
-    mapping = {}
-    mapping['forecast1_a'] = 10
-    mapping['forecast1_b'] = 4
-    controller = controller_stack(controller, mapping, tz=-8, debug=True, parallel=True)
-    now = time.time()
-    controller.run_query_control_for(10)
-    df = pd.DataFrame(controller.log_to_df()['forecast1'])
-    assert df.shape[0] == 5
-
-    for i in (np.diff(df.index) / np.timedelta64(1, 's'))[1:]:
-        assert(math.isclose(i, 3, rel_tol=0.01))
-
-def test_normal():
-    controller = {}
-    controller['forecast1'] = {'function':testcontroller1, 'sampletime':1}
-    controller['mpc1'] = {'function':testcontroller2, 'sampletime':'forecast1'}
-    controller['control1'] = {'function':testcontroller1, 'sampletime':'mpc1'}
-    controller['forecast2'] = {'function':testcontroller3, 'sampletime':2}
-    controller['forecast3'] = {'function':testcontroller1, 'sampletime': 1}
-
-    mapping = {}
-    mapping['forecast1_a'] = 10
-    mapping['forecast1_b'] = 4
-    mapping['forecast2_a'] = 20
-    mapping['forecast2_b'] = 4
-    mapping['forecast3_a'] = 30
-    mapping['forecast3_b'] = 4
-    mapping['mpc1_a'] = 'forecast1_c'
-    mapping['mpc1_b'] = 'forecast1_a'
-    mapping['control1_a'] = 'mpc1_c'
-    mapping['control1_b'] = 'mpc1_a'
-    controller = controller_stack(controller, mapping, tz=-8, debug=True, parallel=True, timeout=2, workers=100)
-
-    controller.run_query_control_for(5)
-    
-    df1 = pd.DataFrame(controller.log_to_df()['forecast1'])
-    df2 = pd.DataFrame(controller.log_to_df()['forecast2'])
-    df3 = pd.DataFrame(controller.log_to_df()['forecast3'])
-    df4 = pd.DataFrame(controller.log_to_df()['mpc1'])
-    df5 = pd.DataFrame(controller.log_to_df()['control1'])
-
-    #print(df1)
-    #print(df2)
-    #print(df3)
-    #print(df4)
-    #print(df5)
-    
-    # Check number of records
-    assert df1.shape[0] == 7
-    assert df2.shape[0] == 4
-    assert df3.shape[0] == 7
-    assert df4.shape[0] == 7
-    assert df5.shape[0] == 7
-
-    # Check contents of records
-    assert pd.isna(df1['a'][0])
-    assert pd.isna(df1['b'][0])
-    assert pd.isna(df1['c'][0])
-    assert pd.isna(df2['a'][0])
-    assert pd.isna(df2['b'][0])
-    assert pd.isna(df2['c'][0])
-    assert pd.isna(df3['a'][0])
-    assert pd.isna(df3['b'][0])
-    assert pd.isna(df3['c'][0])
-    assert pd.isna(df4['a'][0])
-    assert pd.isna(df4['b'][0])
-    assert pd.isna(df4['c'][0])
-    assert pd.isna(df5['a'][0])
-    assert pd.isna(df5['b'][0])
-    assert pd.isna(df5['c'][0])
-    assert list(df1['a'])[1:] == [10.0, 10.0, 10.0, 10.0, 10.0, 10.0]
-    assert list(df1['b'])[1:] == [4.0, 4.0, 4.0, 4.0, 4.0, 4.0]
-    assert list(df1['c'])[1:] == [40.0, 40.0, 40.0, 40.0, 40.0, 40.0]
-    assert list(df2['a'])[1:] == [20.0, 20.0, 20.0]
-    assert list(df2['b'])[1:] == [4.0, 4.0, 4.0]
-    assert list(df2['c'])[1:] == [80.0, 80.0, 80.0]
-    assert list(df3['a'])[1:] == [30.0, 30.0, 30.0, 30.0, 30.0, 30.0]
-    assert list(df3['b'])[1:] == [4.0, 4.0, 4.0, 4.0, 4.0, 4.0]
-    assert list(df3['c'])[1:] == [120.0, 120.0, 120.0, 120.0, 120.0, 120.0]
-    assert list(df4['a'])[1:] == [40.0, 40.0, 40.0, 40.0, 40.0, 40.0]
-    assert list(df4['b'])[1:] == [10.0, 10.0, 10.0, 10.0, 10.0, 10.0]
-    assert list(df4['c'])[1:] == [400.0, 400.0, 400.0, 400.0, 400.0, 400.0]
-    assert list(df5['a'])[1:] == [400.0, 400.0, 400.0, 400.0, 400.0, 400.0]
-    assert list(df5['b'])[1:] == [40.0, 40.0, 40.0, 40.0, 40.0, 40.0]
-    assert list(df5['c'])[1:] == [16000.0, 16000.0, 16000.0, 16000.0, 16000.0, 16000.0]
-    assert list(df1['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
-    assert list(df2['logging']) == ['Initialize', 'testcontroller3 did a computation!', 'testcontroller3 did a computation!', 'testcontroller3 did a computation!']
-    assert list(df3['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
-    assert list(df4['logging']) == ['Initialize', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!']
-    assert list(df5['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
-
-def test_stuckController():
-    '''This tests if the timeout controllers can be caught'''
-    ## CASE1: mpc1 stuck
-    controller = {}
-    controller['forecast1'] = {'function':testcontroller1, 'sampletime':1}
-    controller['mpc1'] = {'function':testcontroller4, 'sampletime':'forecast1'}
-    controller['control1'] = {'function':testcontroller1, 'sampletime':'mpc1'}
-    controller['forecast2'] = {'function':testcontroller1, 'sampletime':1}
-    controller['forecast3'] = {'function':testcontroller1, 'sampletime':1}
-
-    mapping = {}
-    mapping['forecast1_a'] = 10
-    mapping['forecast1_b'] = 4
-    mapping['forecast2_a'] = 20
-    mapping['forecast2_b'] = 4
-    mapping['forecast3_a'] = 30
-    mapping['forecast3_b'] = 4
-    mapping['mpc1_a'] = 'forecast1_c'
-    mapping['mpc1_b'] = 'forecast1_a'
-    mapping['control1_a'] = 'mpc1_c'
-    mapping['control1_b'] = 'mpc1_a'
-    controller = controller_stack(controller, mapping, tz=-8, debug=True, parallel=True, timeout=0.5, workers=100)
-    
-    # Catch warning.
-    with warnings.catch_warnings(record=True) as w:
-        warnings.simplefilter("always")
-        controller.run_query_control_for(2)
-        #assert len(w) == 3
-        for m in w:
-            assert "TimeoutError" in str(m.message)
-            
-    df1 = pd.DataFrame(controller.log_to_df()['forecast1'])
-    df2 = pd.DataFrame(controller.log_to_df()['forecast2'])
-    df3 = pd.DataFrame(controller.log_to_df()['forecast3'])
-    df4 = pd.DataFrame(controller.log_to_df()['mpc1'])
-    df5 = pd.DataFrame(controller.log_to_df()['control1'])
-
-    # Check number of records
-    assert df1.shape[0] == 4
-    assert df2.shape[0] == 4
-    assert df3.shape[0] == 4
-    #assert df4.shape[0] == 1
-    assert df5.shape[0] == 1
-    #assert len(df4.columns) == 1
-    assert len(df5.columns) == 1
-    # Check contents of records
-    assert pd.isna(df1['a'][0])
-    assert pd.isna(df1['b'][0])
-    assert pd.isna(df1['c'][0])
-    assert pd.isna(df2['a'][0])
-    assert pd.isna(df2['b'][0])
-    assert pd.isna(df2['c'][0])
-    assert pd.isna(df3['a'][0])
-    assert pd.isna(df3['b'][0])
-    assert pd.isna(df3['c'][0])
-    assert list(df1['a'])[1:] == [10.0, 10.0, 10.0]
-    assert list(df1['b'])[1:] == [4.0, 4.0, 4.0]
-    assert list(df1['c'])[1:] == [40.0, 40.0, 40.0]
-    assert list(df2['a'])[1:] == [20.0, 20.0, 20.0]
-    assert list(df2['b'])[1:] == [4.0, 4.0, 4.0]
-    assert list(df2['c'])[1:] == [80.0, 80.0, 80.0]
-    assert list(df3['a'])[1:] == [30.0, 30.0, 30.0]
-    assert list(df3['b'])[1:] == [4.0, 4.0, 4.0]
-    assert list(df3['c'])[1:] == [120.0, 120.0, 120.0]
-    assert list(df1['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
-    assert list(df2['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
-    assert list(df3['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
-    #assert list(df4['logging']) == ['Initialize']
-    assert list(df5['logging']) == ['Initialize']
-    
-
-    ##CASE2: mpc1 and forcast2 stuck
-    controller = {}
-    controller['forecast1'] = {'function':testcontroller1, 'sampletime':1}
-    controller['mpc1'] = {'function':testcontroller3, 'sampletime':'forecast1'}
-    controller['control1'] = {'function':testcontroller1, 'sampletime':'mpc1'}
-    controller['forecast2'] = {'function':testcontroller3, 'sampletime':1}
-    controller['forecast3'] = {'function':testcontroller1, 'sampletime':1}
-
-    mapping = {}
-    mapping['forecast1_a'] = 10
-    mapping['forecast1_b'] = 4
-    mapping['forecast2_a'] = 20
-    mapping['forecast2_b'] = 4
-    mapping['forecast3_a'] = 30
-    mapping['forecast3_b'] = 4
-    mapping['mpc1_a'] = 'forecast1_c'
-    mapping['mpc1_b'] = 'forecast1_a'
-    mapping['control1_a'] = 'mpc1_c'
-    mapping['control1_b'] = 'mpc1_a'
-    controller = controller_stack(controller, mapping, tz=-8, debug=True, parallel=True, timeout=0.8, workers=100)
-    
-    #Catch Warnings
-    with warnings.catch_warnings(record=True) as w:
-        warnings.simplefilter("always")
-        controller.run_query_control_for(5)
-        #assert len(w) == 12
-        for m in w:
-            assert "TimeoutError" in str(m.message)
-
-    df1 = pd.DataFrame(controller.log_to_df()['forecast1'])
-    df2 = pd.DataFrame(controller.log_to_df()['forecast2'])
-    df3 = pd.DataFrame(controller.log_to_df()['forecast3'])
-    df4 = pd.DataFrame(controller.log_to_df()['mpc1'])
-    df5 = pd.DataFrame(controller.log_to_df()['control1'])
-
-    # Check number of records
-    #print(df1)
-    assert df1.shape[0] == 7 
-    #assert df2.shape[0] == 1
-    assert df3.shape[0] == 7
-    #print(df3)
-    #assert df4.shape[0] == 1
-    assert df5.shape[0] == 1
-    #assert len(df2.columns) == 1
-    #assert len(df4.columns) == 1
-    assert len(df5.columns) == 1
-    # Check contents of records
-    assert pd.isna(df1['a'][0])
-    assert pd.isna(df1['b'][0])
-    assert pd.isna(df1['c'][0])
-    assert pd.isna(df3['a'][0])
-    assert pd.isna(df3['b'][0])
-    assert pd.isna(df3['c'][0])
-    assert list(df1['a'])[1:] == [10.0, 10.0, 10.0, 10.0, 10.0, 10.0]
-    assert list(df1['b'])[1:] == [4.0, 4.0, 4.0, 4.0, 4.0, 4.0]
-    assert list(df1['c'])[1:] == [40.0, 40.0, 40.0, 40.0, 40.0, 40.0]
-    assert list(df3['a'])[1:] == [30.0, 30.0, 30.0, 30.0, 30.0, 30.0]
-    assert list(df3['b'])[1:] == [4.0, 4.0, 4.0, 4.0, 4.0, 4.0]
-    assert list(df3['c'])[1:] == [120.0, 120.0, 120.0, 120.0, 120.0, 120.0]
-    assert list(df1['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
-    #assert list(df2['logging']) == ['Initialize']
-    assert list(df3['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
-    #assert list(df4['logging']) == ['Initialize']
-    assert list(df5['logging']) == ['Initialize']
-
-def test_serial():
-    controller = {}
-    controller['forecast1'] = {'function':testcontroller1, 'sampletime':1}
-    controller['mpc1'] = {'function':testcontroller2, 'sampletime':'forecast1'}
-    controller['control1'] = {'function':testcontroller1, 'sampletime':'mpc1'}
-    controller['forecast2'] = {'function':testcontroller3, 'sampletime':1}
-    controller['forecast3'] = {'function':testcontroller1, 'sampletime':1}
-
-    mapping = {}
-    mapping['forecast1_a'] = 10
-    mapping['forecast1_b'] = 4
-    mapping['forecast2_a'] = 20
-    mapping['forecast2_b'] = 4
-    mapping['forecast3_a'] = 30
-    mapping['forecast3_b'] = 4
-    mapping['mpc1_a'] = 'forecast1_c'
-    mapping['mpc1_b'] = 'forecast1_a'
-    mapping['control1_a'] = 'mpc1_c'
-    mapping['control1_b'] = 'mpc1_a'
-    controller = controller_stack(controller, mapping, tz=-8, debug=True, parallel=False, timeout=2)
-
-    for i in range(6):
-        controller.query_control(time.time())
-        time.sleep(1.5)
-    
-    df1 = pd.DataFrame(controller.log_to_df()['forecast1'])
-    df2 = pd.DataFrame(controller.log_to_df()['forecast2'])
-    df3 = pd.DataFrame(controller.log_to_df()['forecast3'])
-    df4 = pd.DataFrame(controller.log_to_df()['mpc1'])
-    df5 = pd.DataFrame(controller.log_to_df()['control1'])
-    
-    # Check number of records
-    assert df1.shape[0] == 7
-    assert df2.shape[0] == 7
-    assert df3.shape[0] == 7
-    assert df4.shape[0] == 7
-    assert df5.shape[0] == 7
-
-    # Check contents of records
-    assert pd.isna(df1['a'][0])
-    assert pd.isna(df1['b'][0])
-    assert pd.isna(df1['c'][0])
-    assert pd.isna(df2['a'][0])
-    assert pd.isna(df2['b'][0])
-    assert pd.isna(df2['c'][0])
-    assert pd.isna(df3['a'][0])
-    assert pd.isna(df3['b'][0])
-    assert pd.isna(df3['c'][0])
-    assert pd.isna(df4['a'][0])
-    assert pd.isna(df4['b'][0])
-    assert pd.isna(df4['c'][0])
-    assert pd.isna(df5['a'][0])
-    assert pd.isna(df5['b'][0])
-    assert pd.isna(df5['c'][0])
-    assert list(df1['a'])[1:] == [10.0, 10.0, 10.0, 10.0, 10.0, 10.0]
-    assert list(df1['b'])[1:] == [4.0, 4.0, 4.0, 4.0, 4.0, 4.0]
-    assert list(df1['c'])[1:] == [40.0, 40.0, 40.0, 40.0, 40.0, 40.0]
-    assert list(df2['a'])[1:] == [20.0, 20.0, 20.0, 20.0, 20.0, 20.0]
-    assert list(df2['b'])[1:] == [4.0, 4.0, 4.0, 4.0, 4.0, 4.0]
-    assert list(df2['c'])[1:] == [80.0, 80.0, 80.0, 80.0, 80.0, 80.0]
-    assert list(df3['a'])[1:] == [30.0, 30.0, 30.0, 30.0, 30.0, 30.0]
-    assert list(df3['b'])[1:] == [4.0, 4.0, 4.0, 4.0, 4.0, 4.0]
-    assert list(df3['c'])[1:] == [120.0, 120.0, 120.0, 120.0, 120.0, 120.0]
-    assert list(df4['a'])[1:] == [40.0, 40.0, 40.0, 40.0, 40.0, 40.0]
-    assert list(df4['b'])[1:] == [10.0, 10.0, 10.0, 10.0, 10.0, 10.0]
-    assert list(df4['c'])[1:] == [400.0, 400.0, 400.0, 400.0, 400.0, 400.0]
-    assert list(df5['a'])[1:] == [400.0, 400.0, 400.0, 400.0, 400.0, 400.0]
-    assert list(df5['b'])[1:] == [40.0, 40.0, 40.0, 40.0, 40.0, 40.0]
-    assert list(df5['c'])[1:] == [16000.0, 16000.0, 16000.0, 16000.0, 16000.0, 16000.0]
-    assert list(df1['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
-    assert list(df2['logging']) == ['Initialize', 'testcontroller3 did a computation!', 'testcontroller3 did a computation!', 'testcontroller3 did a computation!', 'testcontroller3 did a computation!', 'testcontroller3 did a computation!', 'testcontroller3 did a computation!']
-    assert list(df3['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
-    assert list(df4['logging']) == ['Initialize', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!']
-    assert list(df5['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
+import sys
+import time
+import math
+import warnings
+import numpy as np
+import pandas as pd
+from os import path
+
+sys.path.append(path.dirname(path.dirname(path.abspath(__file__))))
+from fmlc.triggering import triggering
+from fmlc.baseclasses import eFMU
+from fmlc.stackedclasses import controller_stack
+
+class testcontroller1(eFMU):
+    def __init__(self):
+        self.input = {'a': None, 'b': None}
+        self.output = {'c': None}
+        self.init = True
+    def compute(self):
+        self.init= False
+        self.output['c'] = self.input['a'] * self.input['b']
+        return 'testcontroller1 did a computation!'
+
+class testcontroller2(eFMU):
+    def __init__(self):
+        self.input = {'a': None, 'b': None}
+        self.output = {'c': None}
+        self.init = True
+
+    def compute(self):
+        self.init = False
+        self.output['c'] = self.input['a'] * self.input['b']
+        time.sleep(0.2)
+        return 'testcontroller2 did a computation!'
+
+class testcontroller3(eFMU):
+    def __init__(self):
+        self.input = {'a': None, 'b': None}
+        self.output = {'c': None}
+        self.init = True
+
+    def compute(self):
+        self.init = False
+        self.output['c'] = self.input['a'] * self.input['b']
+        time.sleep(1)
+        return 'testcontroller3 did a computation!'
+
+class testcontroller4(eFMU):
+    def __init__(self):
+        self.input = {'a': None, 'b': None}
+        self.output = {'c': None}
+        self.init = True
+
+    def compute(self):
+        self.init = False
+        self.output['c'] = self.input['a'] * self.input['b']
+        time.sleep(10)
+        return 'testcontroller4 did a computation!'
+        
+def test_sampletime():
+    '''This tests if the sample time is working properly'''
+    controller = {}
+    controller['forecast1'] = {'function': testcontroller1, 'sampletime': 3}
+    mapping = {}
+    mapping['forecast1_a'] = 10
+    mapping['forecast1_b'] = 4
+    controller = controller_stack(controller, mapping, tz=-8, debug=True, parallel=True)
+    now = time.time()
+    controller.run_query_control_for(10)
+    df = pd.DataFrame(controller.log_to_df()['forecast1'])
+    assert df.shape[0] == 5
+
+    for i in (np.diff(df.index) / np.timedelta64(1, 's'))[1:]:
+        assert(math.isclose(i, 3, rel_tol=0.01))
+
+def test_normal():
+    controller = {}
+    controller['forecast1'] = {'function':testcontroller1, 'sampletime':1}
+    controller['mpc1'] = {'function':testcontroller2, 'sampletime':'forecast1'}
+    controller['control1'] = {'function':testcontroller1, 'sampletime':'mpc1'}
+    controller['forecast2'] = {'function':testcontroller3, 'sampletime':2}
+    controller['forecast3'] = {'function':testcontroller1, 'sampletime': 1}
+
+    mapping = {}
+    mapping['forecast1_a'] = 10
+    mapping['forecast1_b'] = 4
+    mapping['forecast2_a'] = 20
+    mapping['forecast2_b'] = 4
+    mapping['forecast3_a'] = 30
+    mapping['forecast3_b'] = 4
+    mapping['mpc1_a'] = 'forecast1_c'
+    mapping['mpc1_b'] = 'forecast1_a'
+    mapping['control1_a'] = 'mpc1_c'
+    mapping['control1_b'] = 'mpc1_a'
+    controller = controller_stack(controller, mapping, tz=-8, debug=True, parallel=True, timeout=2, workers=100)
+
+    controller.run_query_control_for(5)
+    
+    df1 = pd.DataFrame(controller.log_to_df()['forecast1'])
+    df2 = pd.DataFrame(controller.log_to_df()['forecast2'])
+    df3 = pd.DataFrame(controller.log_to_df()['forecast3'])
+    df4 = pd.DataFrame(controller.log_to_df()['mpc1'])
+    df5 = pd.DataFrame(controller.log_to_df()['control1'])
+
+    #print(df1)
+    #print(df2)
+    #print(df3)
+    #print(df4)
+    #print(df5)
+    
+    # Check number of records
+    assert df1.shape[0] == 7
+    assert df2.shape[0] == 4
+    assert df3.shape[0] == 7
+    assert df4.shape[0] == 7
+    assert df5.shape[0] == 7
+
+    # Check contents of records
+    assert pd.isna(df1['a'][0])
+    assert pd.isna(df1['b'][0])
+    assert pd.isna(df1['c'][0])
+    assert pd.isna(df2['a'][0])
+    assert pd.isna(df2['b'][0])
+    assert pd.isna(df2['c'][0])
+    assert pd.isna(df3['a'][0])
+    assert pd.isna(df3['b'][0])
+    assert pd.isna(df3['c'][0])
+    assert pd.isna(df4['a'][0])
+    assert pd.isna(df4['b'][0])
+    assert pd.isna(df4['c'][0])
+    assert pd.isna(df5['a'][0])
+    assert pd.isna(df5['b'][0])
+    assert pd.isna(df5['c'][0])
+    assert list(df1['a'])[1:] == [10.0, 10.0, 10.0, 10.0, 10.0, 10.0]
+    assert list(df1['b'])[1:] == [4.0, 4.0, 4.0, 4.0, 4.0, 4.0]
+    assert list(df1['c'])[1:] == [40.0, 40.0, 40.0, 40.0, 40.0, 40.0]
+    assert list(df2['a'])[1:] == [20.0, 20.0, 20.0]
+    assert list(df2['b'])[1:] == [4.0, 4.0, 4.0]
+    assert list(df2['c'])[1:] == [80.0, 80.0, 80.0]
+    assert list(df3['a'])[1:] == [30.0, 30.0, 30.0, 30.0, 30.0, 30.0]
+    assert list(df3['b'])[1:] == [4.0, 4.0, 4.0, 4.0, 4.0, 4.0]
+    assert list(df3['c'])[1:] == [120.0, 120.0, 120.0, 120.0, 120.0, 120.0]
+    assert list(df4['a'])[1:] == [40.0, 40.0, 40.0, 40.0, 40.0, 40.0]
+    assert list(df4['b'])[1:] == [10.0, 10.0, 10.0, 10.0, 10.0, 10.0]
+    assert list(df4['c'])[1:] == [400.0, 400.0, 400.0, 400.0, 400.0, 400.0]
+    assert list(df5['a'])[1:] == [400.0, 400.0, 400.0, 400.0, 400.0, 400.0]
+    assert list(df5['b'])[1:] == [40.0, 40.0, 40.0, 40.0, 40.0, 40.0]
+    assert list(df5['c'])[1:] == [16000.0, 16000.0, 16000.0, 16000.0, 16000.0, 16000.0]
+    assert list(df1['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
+    assert list(df2['logging']) == ['Initialize', 'testcontroller3 did a computation!', 'testcontroller3 did a computation!', 'testcontroller3 did a computation!']
+    assert list(df3['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
+    assert list(df4['logging']) == ['Initialize', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!']
+    assert list(df5['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
+
+def test_stuckController():
+    '''This tests if the timeout controllers can be caught'''
+    ## CASE1: mpc1 stuck
+    controller = {}
+    controller['forecast1'] = {'function':testcontroller1, 'sampletime':1}
+    controller['mpc1'] = {'function':testcontroller4, 'sampletime':'forecast1'}
+    controller['control1'] = {'function':testcontroller1, 'sampletime':'mpc1'}
+    controller['forecast2'] = {'function':testcontroller1, 'sampletime':1}
+    controller['forecast3'] = {'function':testcontroller1, 'sampletime':1}
+
+    mapping = {}
+    mapping['forecast1_a'] = 10
+    mapping['forecast1_b'] = 4
+    mapping['forecast2_a'] = 20
+    mapping['forecast2_b'] = 4
+    mapping['forecast3_a'] = 30
+    mapping['forecast3_b'] = 4
+    mapping['mpc1_a'] = 'forecast1_c'
+    mapping['mpc1_b'] = 'forecast1_a'
+    mapping['control1_a'] = 'mpc1_c'
+    mapping['control1_b'] = 'mpc1_a'
+    controller = controller_stack(controller, mapping, tz=-8, debug=True, parallel=True, timeout=0.5, workers=100)
+    
+    # Catch warning.
+    with warnings.catch_warnings(record=True) as w:
+        warnings.simplefilter("always")
+        controller.run_query_control_for(2)
+        #assert len(w) == 3
+        for m in w:
+            assert "TimeoutError" in str(m.message)
+            
+    df1 = pd.DataFrame(controller.log_to_df()['forecast1'])
+    df2 = pd.DataFrame(controller.log_to_df()['forecast2'])
+    df3 = pd.DataFrame(controller.log_to_df()['forecast3'])
+    df4 = pd.DataFrame(controller.log_to_df()['mpc1'])
+    df5 = pd.DataFrame(controller.log_to_df()['control1'])
+
+    # Check number of records
+    assert df1.shape[0] == 4
+    assert df2.shape[0] == 4
+    assert df3.shape[0] == 4
+    #assert df4.shape[0] == 1
+    assert df5.shape[0] == 1
+    #assert len(df4.columns) == 1
+    assert len(df5.columns) == 1
+    # Check contents of records
+    assert pd.isna(df1['a'][0])
+    assert pd.isna(df1['b'][0])
+    assert pd.isna(df1['c'][0])
+    assert pd.isna(df2['a'][0])
+    assert pd.isna(df2['b'][0])
+    assert pd.isna(df2['c'][0])
+    assert pd.isna(df3['a'][0])
+    assert pd.isna(df3['b'][0])
+    assert pd.isna(df3['c'][0])
+    assert list(df1['a'])[1:] == [10.0, 10.0, 10.0]
+    assert list(df1['b'])[1:] == [4.0, 4.0, 4.0]
+    assert list(df1['c'])[1:] == [40.0, 40.0, 40.0]
+    assert list(df2['a'])[1:] == [20.0, 20.0, 20.0]
+    assert list(df2['b'])[1:] == [4.0, 4.0, 4.0]
+    assert list(df2['c'])[1:] == [80.0, 80.0, 80.0]
+    assert list(df3['a'])[1:] == [30.0, 30.0, 30.0]
+    assert list(df3['b'])[1:] == [4.0, 4.0, 4.0]
+    assert list(df3['c'])[1:] == [120.0, 120.0, 120.0]
+    assert list(df1['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
+    assert list(df2['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
+    assert list(df3['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
+    #assert list(df4['logging']) == ['Initialize']
+    assert list(df5['logging']) == ['Initialize']
+    
+
+    ##CASE2: mpc1 and forcast2 stuck
+    controller = {}
+    controller['forecast1'] = {'function':testcontroller1, 'sampletime':1}
+    controller['mpc1'] = {'function':testcontroller3, 'sampletime':'forecast1'}
+    controller['control1'] = {'function':testcontroller1, 'sampletime':'mpc1'}
+    controller['forecast2'] = {'function':testcontroller3, 'sampletime':1}
+    controller['forecast3'] = {'function':testcontroller1, 'sampletime':1}
+
+    mapping = {}
+    mapping['forecast1_a'] = 10
+    mapping['forecast1_b'] = 4
+    mapping['forecast2_a'] = 20
+    mapping['forecast2_b'] = 4
+    mapping['forecast3_a'] = 30
+    mapping['forecast3_b'] = 4
+    mapping['mpc1_a'] = 'forecast1_c'
+    mapping['mpc1_b'] = 'forecast1_a'
+    mapping['control1_a'] = 'mpc1_c'
+    mapping['control1_b'] = 'mpc1_a'
+    controller = controller_stack(controller, mapping, tz=-8, debug=True, parallel=True, timeout=0.8, workers=100)
+    
+    #Catch Warnings
+    with warnings.catch_warnings(record=True) as w:
+        warnings.simplefilter("always")
+        controller.run_query_control_for(5)
+        #assert len(w) == 12
+        for m in w:
+            assert "TimeoutError" in str(m.message)
+
+    df1 = pd.DataFrame(controller.log_to_df()['forecast1'])
+    df2 = pd.DataFrame(controller.log_to_df()['forecast2'])
+    df3 = pd.DataFrame(controller.log_to_df()['forecast3'])
+    df4 = pd.DataFrame(controller.log_to_df()['mpc1'])
+    df5 = pd.DataFrame(controller.log_to_df()['control1'])
+
+    # Check number of records
+    #print(df1)
+    assert df1.shape[0] == 7 
+    #assert df2.shape[0] == 1
+    assert df3.shape[0] == 7
+    #print(df3)
+    #assert df4.shape[0] == 1
+    assert df5.shape[0] == 1
+    #assert len(df2.columns) == 1
+    #assert len(df4.columns) == 1
+    assert len(df5.columns) == 1
+    # Check contents of records
+    assert pd.isna(df1['a'][0])
+    assert pd.isna(df1['b'][0])
+    assert pd.isna(df1['c'][0])
+    assert pd.isna(df3['a'][0])
+    assert pd.isna(df3['b'][0])
+    assert pd.isna(df3['c'][0])
+    assert list(df1['a'])[1:] == [10.0, 10.0, 10.0, 10.0, 10.0, 10.0]
+    assert list(df1['b'])[1:] == [4.0, 4.0, 4.0, 4.0, 4.0, 4.0]
+    assert list(df1['c'])[1:] == [40.0, 40.0, 40.0, 40.0, 40.0, 40.0]
+    assert list(df3['a'])[1:] == [30.0, 30.0, 30.0, 30.0, 30.0, 30.0]
+    assert list(df3['b'])[1:] == [4.0, 4.0, 4.0, 4.0, 4.0, 4.0]
+    assert list(df3['c'])[1:] == [120.0, 120.0, 120.0, 120.0, 120.0, 120.0]
+    assert list(df1['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
+    #assert list(df2['logging']) == ['Initialize']
+    assert list(df3['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
+    #assert list(df4['logging']) == ['Initialize']
+    assert list(df5['logging']) == ['Initialize']
+
+def test_serial():
+    controller = {}
+    controller['forecast1'] = {'function':testcontroller1, 'sampletime':1}
+    controller['mpc1'] = {'function':testcontroller2, 'sampletime':'forecast1'}
+    controller['control1'] = {'function':testcontroller1, 'sampletime':'mpc1'}
+    controller['forecast2'] = {'function':testcontroller3, 'sampletime':1}
+    controller['forecast3'] = {'function':testcontroller1, 'sampletime':1}
+
+    mapping = {}
+    mapping['forecast1_a'] = 10
+    mapping['forecast1_b'] = 4
+    mapping['forecast2_a'] = 20
+    mapping['forecast2_b'] = 4
+    mapping['forecast3_a'] = 30
+    mapping['forecast3_b'] = 4
+    mapping['mpc1_a'] = 'forecast1_c'
+    mapping['mpc1_b'] = 'forecast1_a'
+    mapping['control1_a'] = 'mpc1_c'
+    mapping['control1_b'] = 'mpc1_a'
+    controller = controller_stack(controller, mapping, tz=-8, debug=True, parallel=False, timeout=2)
+
+    for i in range(6):
+        controller.query_control(time.time())
+        time.sleep(1.5)
+    
+    df1 = pd.DataFrame(controller.log_to_df()['forecast1'])
+    df2 = pd.DataFrame(controller.log_to_df()['forecast2'])
+    df3 = pd.DataFrame(controller.log_to_df()['forecast3'])
+    df4 = pd.DataFrame(controller.log_to_df()['mpc1'])
+    df5 = pd.DataFrame(controller.log_to_df()['control1'])
+    
+    # Check number of records
+    assert df1.shape[0] == 7
+    assert df2.shape[0] == 7
+    assert df3.shape[0] == 7
+    assert df4.shape[0] == 7
+    assert df5.shape[0] == 7
+
+    # Check contents of records
+    assert pd.isna(df1['a'][0])
+    assert pd.isna(df1['b'][0])
+    assert pd.isna(df1['c'][0])
+    assert pd.isna(df2['a'][0])
+    assert pd.isna(df2['b'][0])
+    assert pd.isna(df2['c'][0])
+    assert pd.isna(df3['a'][0])
+    assert pd.isna(df3['b'][0])
+    assert pd.isna(df3['c'][0])
+    assert pd.isna(df4['a'][0])
+    assert pd.isna(df4['b'][0])
+    assert pd.isna(df4['c'][0])
+    assert pd.isna(df5['a'][0])
+    assert pd.isna(df5['b'][0])
+    assert pd.isna(df5['c'][0])
+    assert list(df1['a'])[1:] == [10.0, 10.0, 10.0, 10.0, 10.0, 10.0]
+    assert list(df1['b'])[1:] == [4.0, 4.0, 4.0, 4.0, 4.0, 4.0]
+    assert list(df1['c'])[1:] == [40.0, 40.0, 40.0, 40.0, 40.0, 40.0]
+    assert list(df2['a'])[1:] == [20.0, 20.0, 20.0, 20.0, 20.0, 20.0]
+    assert list(df2['b'])[1:] == [4.0, 4.0, 4.0, 4.0, 4.0, 4.0]
+    assert list(df2['c'])[1:] == [80.0, 80.0, 80.0, 80.0, 80.0, 80.0]
+    assert list(df3['a'])[1:] == [30.0, 30.0, 30.0, 30.0, 30.0, 30.0]
+    assert list(df3['b'])[1:] == [4.0, 4.0, 4.0, 4.0, 4.0, 4.0]
+    assert list(df3['c'])[1:] == [120.0, 120.0, 120.0, 120.0, 120.0, 120.0]
+    assert list(df4['a'])[1:] == [40.0, 40.0, 40.0, 40.0, 40.0, 40.0]
+    assert list(df4['b'])[1:] == [10.0, 10.0, 10.0, 10.0, 10.0, 10.0]
+    assert list(df4['c'])[1:] == [400.0, 400.0, 400.0, 400.0, 400.0, 400.0]
+    assert list(df5['a'])[1:] == [400.0, 400.0, 400.0, 400.0, 400.0, 400.0]
+    assert list(df5['b'])[1:] == [40.0, 40.0, 40.0, 40.0, 40.0, 40.0]
+    assert list(df5['c'])[1:] == [16000.0, 16000.0, 16000.0, 16000.0, 16000.0, 16000.0]
+    assert list(df1['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
+    assert list(df2['logging']) == ['Initialize', 'testcontroller3 did a computation!', 'testcontroller3 did a computation!', 'testcontroller3 did a computation!', 'testcontroller3 did a computation!', 'testcontroller3 did a computation!', 'testcontroller3 did a computation!']
+    assert list(df3['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
+    assert list(df4['logging']) == ['Initialize', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!', 'testcontroller2 did a computation!']
+    assert list(df5['logging']) == ['Initialize', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!', 'testcontroller1 did a computation!']
```

