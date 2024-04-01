# Comparing `tmp/jsbgym-0.3.1.tar.gz` & `tmp/jsbgym-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsbgym-0.3.1.tar", last modified: Mon Dec 11 12:48:50 2023, max compression
+gzip compressed data, was "jsbgym-0.3.2.tar", last modified: Mon Apr  1 11:43:35 2024, max compression
```

## Comparing `jsbgym-0.3.1.tar` & `jsbgym-0.3.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 12:48:50.403756 jsbgym-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-12-11 12:48:42.000000 jsbgym-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 12:48:42.000000 jsbgym-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2023-12-11 12:48:50.403756 jsbgym-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2023-12-11 12:48:42.000000 jsbgym-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 12:48:50.399757 jsbgym-0.3.1/jsbgym/
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 12:48:50.399757 jsbgym-0.3.1/jsbgym/agents/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/agents/agents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/aircraft.py
--rw-r--r--   0 runner    (1001) docker     (127)     8691 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/assessors.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/basic_ic.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/flightgear.xml
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/minimal_ic.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    11941 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/rewards.py
--rw-r--r--   0 runner    (1001) docker     (127)     9595 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    19494 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 12:48:50.399757 jsbgym-0.3.1/jsbgym/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6730 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/tests/manual_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8547 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/tests/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/tests/test_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)    12703 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/tests/test_assessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8783 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/tests/test_geodetic_position.py
--rw-r--r--   0 runner    (1001) docker     (127)    17121 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/tests/test_rewards.py
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    25487 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/tests/test_visualiser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15266 2023-12-11 12:48:42.000000 jsbgym-0.3.1/jsbgym/visualiser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 12:48:50.399757 jsbgym-0.3.1/jsbgym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2023-12-11 12:48:50.000000 jsbgym-0.3.1/jsbgym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      888 2023-12-11 12:48:50.000000 jsbgym-0.3.1/jsbgym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 12:48:50.000000 jsbgym-0.3.1/jsbgym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 12:48:50.000000 jsbgym-0.3.1/jsbgym.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-11 12:48:50.000000 jsbgym-0.3.1/jsbgym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-11 12:48:50.000000 jsbgym-0.3.1/jsbgym.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2023-12-11 12:48:42.000000 jsbgym-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 12:48:50.403756 jsbgym-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:43:35.597670 jsbgym-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-01 11:43:31.000000 jsbgym-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 11:43:31.000000 jsbgym-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-04-01 11:43:35.597670 jsbgym-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-04-01 11:43:31.000000 jsbgym-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:43:35.589671 jsbgym-0.3.2/jsbgym/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:43:35.593670 jsbgym-0.3.2/jsbgym/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/agents/agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/aircraft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8691 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/assessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/basic_ic.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/flightgear.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/minimal_ic.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11921 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19485 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:43:35.593670 jsbgym-0.3.2/jsbgym/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/tests/manual_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8547 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/tests/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/tests/test_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12703 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/tests/test_assessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/tests/test_geodetic_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17112 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/tests/test_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25487 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/tests/test_visualiser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-04-01 11:43:31.000000 jsbgym-0.3.2/jsbgym/visualiser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:43:35.593670 jsbgym-0.3.2/jsbgym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-04-01 11:43:35.000000 jsbgym-0.3.2/jsbgym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-01 11:43:35.000000 jsbgym-0.3.2/jsbgym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:43:35.000000 jsbgym-0.3.2/jsbgym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:43:35.000000 jsbgym-0.3.2/jsbgym.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-01 11:43:35.000000 jsbgym-0.3.2/jsbgym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 11:43:35.000000 jsbgym-0.3.2/jsbgym.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-01 11:43:31.000000 jsbgym-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 11:43:35.597670 jsbgym-0.3.2/setup.cfg
```

### Comparing `jsbgym-0.3.1/LICENSE` & `jsbgym-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/PKG-INFO` & `jsbgym-0.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,91 @@
 Metadata-Version: 2.1
 Name: jsbgym
-Version: 0.3.1
+Version: 0.3.2
 Summary: A package of reinforcement learning environments for flight control using the JSBSim flight dynamics model.
 Author: sryu1
 License: MIT
 Project-URL: Homepage, https://github.com/sryu1/jsbgym
 Project-URL: Repository, https://github.com/sryu1/jsbgym
 Project-URL: Bug Tracker, https://github.com/sryu1/jsbgym/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: gymnasium
 Requires-Dist: jsbsim
 Requires-Dist: matplotlib
 
 # JSBGym
 
 [![Python: 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
 [![PyPI Version](https://img.shields.io/pypi/v/jsbgym)](https://pypi.org/project/jsbgym)
-[![PyPI downloads](https://img.shields.io/pypi/dm/jsbgym.svg)](https://pypistats.org/packages/jsbgym)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/jsbgym)](https://pypistats.org/packages/jsbgym)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 JSBGym provides reinforcement learning environments for the control of fixed-wing aircraft using the JSBSim flight dynamics model. The package's environments implement the Farama-Foundation's Gymnasium interface allowing environments to be created and interacted with.
 
 ![Example](https://github.com/sryu1/jsbgym/blob/main/docs/J3.gif?raw=true)
 
 Pretrained models can be found [here](https://huggingface.co/sryu1/jsbgym_models)
 
 ## Setup
 
-Open a terminal and install jsbgym:
+### Windows
+
+Open a terminal and install jsbgym via pip:
+
+```console
+pip install jsbgym
+```
+
+To render the environment with FlightGear, download and install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`) and if not already existant, add a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`).
+
+If there are aircraft installed in a different location, add the folder to the `FG_AIRCRAFT` system variable.
+3D visualisation requires installation of the FlightGear simulator. Confirm FlightGear is runnable from terminal with:
+
+```console
+fgfs --version
+```
+
+### Linux
+
+Open a terminal and install jsbgym via pip:
 
 ```console
 pip install jsbgym
 ```
 
-For Linux systems, rendering with some modes will require an additional package:
+Rendering with some modes will require an additional package:
 
 ```console
 sudo apt-get install python3-tk
 ```
 
-To render the environment with FlightGear, dowloand and install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`) and if not already existant, add a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`). For Linux, rename the AppImage file to fgfs.AppImage and place it in /usr/local/bin/fgfs. The data file must also be downloaded from [here](https://sourceforge.net/projects/flightgear/files/release-2020.3/) (approximately 2 GB) then in terminal, enter
+Rename the AppImage file to `fgfs` and place it in `/usr/local/bin`:
+
+```console
+sudo mv fgfs /usr/local/bin
+```
+
+The data files must also be downloaded from [here](https://sourceforge.net/projects/flightgear/files/release-2020.3/) (approximately 2 GB) then in terminal, enter
 
 ```console
-export FG_ROOT=/path/to/folder
+export FG_ROOT=/path/to/datafolder
 ```
 
 If there are aircraft installed in a different location, add the folder to the `FG_AIRCRAFT` system variable.
-3D visualisation requires installation of the FlightGear simulator. Confirm it is runnable from terminal with:
+3D visualisation requires installation of the FlightGear simulator. Confirm FlightGear is runnable from terminal with:
 
 ```console
 fgfs --version
 ```
 
 ## Getting Started
```

### Comparing `jsbgym-0.3.1/README.md` & `jsbgym-0.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,67 @@
 # JSBGym
 
 [![Python: 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
 [![PyPI Version](https://img.shields.io/pypi/v/jsbgym)](https://pypi.org/project/jsbgym)
-[![PyPI downloads](https://img.shields.io/pypi/dm/jsbgym.svg)](https://pypistats.org/packages/jsbgym)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/jsbgym)](https://pypistats.org/packages/jsbgym)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 JSBGym provides reinforcement learning environments for the control of fixed-wing aircraft using the JSBSim flight dynamics model. The package's environments implement the Farama-Foundation's Gymnasium interface allowing environments to be created and interacted with.
 
 ![Example](https://github.com/sryu1/jsbgym/blob/main/docs/J3.gif?raw=true)
 
 Pretrained models can be found [here](https://huggingface.co/sryu1/jsbgym_models)
 
 ## Setup
 
-Open a terminal and install jsbgym:
+### Windows
+
+Open a terminal and install jsbgym via pip:
+
+```console
+pip install jsbgym
+```
+
+To render the environment with FlightGear, download and install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`) and if not already existant, add a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`).
+
+If there are aircraft installed in a different location, add the folder to the `FG_AIRCRAFT` system variable.
+3D visualisation requires installation of the FlightGear simulator. Confirm FlightGear is runnable from terminal with:
+
+```console
+fgfs --version
+```
+
+### Linux
+
+Open a terminal and install jsbgym via pip:
 
 ```console
 pip install jsbgym
 ```
 
-For Linux systems, rendering with some modes will require an additional package:
+Rendering with some modes will require an additional package:
 
 ```console
 sudo apt-get install python3-tk
 ```
 
-To render the environment with FlightGear, dowloand and install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`) and if not already existant, add a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`). For Linux, rename the AppImage file to fgfs.AppImage and place it in /usr/local/bin/fgfs. The data file must also be downloaded from [here](https://sourceforge.net/projects/flightgear/files/release-2020.3/) (approximately 2 GB) then in terminal, enter
+Rename the AppImage file to `fgfs` and place it in `/usr/local/bin`:
+
+```console
+sudo mv fgfs /usr/local/bin
+```
+
+The data files must also be downloaded from [here](https://sourceforge.net/projects/flightgear/files/release-2020.3/) (approximately 2 GB) then in terminal, enter
 
 ```console
-export FG_ROOT=/path/to/folder
+export FG_ROOT=/path/to/datafolder
 ```
 
 If there are aircraft installed in a different location, add the folder to the `FG_AIRCRAFT` system variable.
-3D visualisation requires installation of the FlightGear simulator. Confirm it is runnable from terminal with:
+3D visualisation requires installation of the FlightGear simulator. Confirm FlightGear is runnable from terminal with:
 
 ```console
 fgfs --version
 ```
 
 ## Getting Started
```

### Comparing `jsbgym-0.3.1/jsbgym/agents/agents.py` & `jsbgym-0.3.2/jsbgym/agents/agents.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 import numpy as np
 from typing import List
 from abc import ABC, abstractmethod
 
 
 class Agent(ABC):
     @abstractmethod
-    def act(self, state) -> np.ndarray:
-        ...
+    def act(self, state) -> np.ndarray: ...
 
     @abstractmethod
-    def observe(self, state, action, reward, terminated):
-        ...
+    def observe(self, state, action, reward, terminated): ...
 
 
 class RandomAgent(Agent):
     """An agent that selects random actions.
 
     The Random object making selection is gym.np_random used by the
     Space.sample() method. Its seed is set by gym.
```

### Comparing `jsbgym-0.3.1/jsbgym/aircraft.py` & `jsbgym-0.3.2/jsbgym/aircraft.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/jsbgym/assessors.py` & `jsbgym-0.3.2/jsbgym/assessors.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/jsbgym/basic_ic.xml` & `jsbgym-0.3.2/jsbgym/basic_ic.xml`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/jsbgym/environment.py` & `jsbgym-0.3.2/jsbgym/environment.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/jsbgym/flightgear.xml` & `jsbgym-0.3.2/jsbgym/flightgear.xml`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/jsbgym/properties.py` & `jsbgym-0.3.2/jsbgym/properties.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/jsbgym/rewards.py` & `jsbgym-0.3.2/jsbgym/rewards.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,28 +40,26 @@
         return bool(self.shaping_reward_elements)
 
 
 class RewardComponent(ABC):
     """Interface for RewardComponent, an object which calculates one component value of a Reward"""
 
     @abstractmethod
-    def calculate(self, state: State, last_state: State, is_terminal: bool) -> float:
-        ...
+    def calculate(
+        self, state: State, last_state: State, is_terminal: bool
+    ) -> float: ...
 
     @abstractmethod
-    def get_name(self) -> str:
-        ...
+    def get_name(self) -> str: ...
 
     @abstractmethod
-    def get_potential(self, state: State, is_terminal) -> float:
-        ...
+    def get_potential(self, state: State, is_terminal) -> float: ...
 
     @abstractmethod
-    def is_potential_difference_based(self) -> bool:
-        ...
+    def is_potential_difference_based(self) -> bool: ...
 
 
 class NormalisedComponent(RewardComponent, ABC):
     """
     Base implementation of a RewardComponent implementing common methods.
 
     All potentials of subclasses should be normalised in [0.0, 1.0]
```

### Comparing `jsbgym-0.3.1/jsbgym/simulation.py` & `jsbgym-0.3.2/jsbgym/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def __init__(
         self,
         sim_frequency_hz: float = 60.0,
         aircraft: Aircraft = c172,
         init_conditions: Dict[prp.Property, float] = None,
         allow_flightgear_output: bool = True,
     ):
-        """
+        r"""
         Constructor. Creates an instance of JSBSim and sets initial conditions.
 
         :param sim_frequency_hz: the JSBSim integration frequency in Hz.
         :param aircraft_model_name: name of aircraft to be loaded.
             JSBSim looks for file \model_name\model_name.xml from root dir.
         :param init_conditions: dict mapping properties to their initial values.
             Defaults to None, causing a default set of initial props to be used.
```

### Comparing `jsbgym-0.3.1/jsbgym/tasks.py` & `jsbgym-0.3.2/jsbgym/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,16 +226,15 @@
         By default it simply starts the aircraft engines.
         """
         sim.start_engines()
         sim.raise_landing_gear()
         self._store_reward(RewardStub(1.0, 1.0), sim)
 
     @abstractmethod
-    def get_initial_conditions(self) -> Dict[Property, float]:
-        ...
+    def get_initial_conditions(self) -> Dict[Property, float]: ...
 
     def get_state_space(self) -> gym.Space:
         state_lows = np.array([state_var.min for state_var in self.state_variables])
         state_highs = np.array([state_var.max for state_var in self.state_variables])
         return gym.spaces.Box(low=state_lows, high=state_highs, dtype=np.float64)
 
     def get_action_space(self) -> gym.Space:
```

### Comparing `jsbgym-0.3.1/jsbgym/tests/manual_tests.py` & `jsbgym-0.3.2/jsbgym/tests/manual_tests.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/jsbgym/tests/stubs.py` & `jsbgym-0.3.2/jsbgym/tests/stubs.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/jsbgym/tests/test_agents.py` & `jsbgym-0.3.2/jsbgym/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/jsbgym/tests/test_assessors.py` & `jsbgym-0.3.2/jsbgym/tests/test_assessors.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/jsbgym/tests/test_environment.py` & `jsbgym-0.3.2/jsbgym/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/jsbgym/tests/test_functional.py` & `jsbgym-0.3.2/jsbgym/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/jsbgym/tests/test_geodetic_position.py` & `jsbgym-0.3.2/jsbgym/tests/test_geodetic_position.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/jsbgym/tests/test_rewards.py` & `jsbgym-0.3.2/jsbgym/tests/test_rewards.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,16 +87,15 @@
     default_name = "test_component"
     extra_kwargs = dict()
 
     def setUp(self):
         self.COT = self.get_class_under_test()
 
     @abstractmethod
-    def get_class_under_test(self) -> Type[ErrorComponent]:
-        ...
+    def get_class_under_test(self) -> Type[ErrorComponent]: ...
 
     def get_default_perfect_state(self):
         """Returns a state where the controlled property matches the target exactly"""
         return self.dummy_task.get_state(
             self.default_target_value, self.default_target_value
         )
```

### Comparing `jsbgym-0.3.1/jsbgym/tests/test_simulation.py` & `jsbgym-0.3.2/jsbgym/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/jsbgym/tests/test_tasks.py` & `jsbgym-0.3.2/jsbgym/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/jsbgym/tests/test_visualiser.py` & `jsbgym-0.3.2/jsbgym/tests/test_visualiser.py`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/jsbgym/utils.py` & `jsbgym-0.3.2/jsbgym/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class AttributeFormatter(object):
     """
     Replaces characters that would be illegal in an attribute name
 
     Used through its static method, translate()
     """
 
-    ILLEGAL_CHARS = "\-/."
+    ILLEGAL_CHARS = r"\-/."
     TRANSLATE_TO = "_" * len(ILLEGAL_CHARS)
     TRANSLATION_TABLE = str.maketrans(ILLEGAL_CHARS, TRANSLATE_TO)
 
     @staticmethod
     def translate(string: str):
         return string.translate(AttributeFormatter.TRANSLATION_TABLE)
```

### Comparing `jsbgym-0.3.1/jsbgym/visualiser.py` & `jsbgym-0.3.2/jsbgym/visualiser.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,15 +378,15 @@
             "--native-fdm=" + f"{FlightGearVisualiser.TYPE},"
             f"{FlightGearVisualiser.DIRECTION},"
             f"{FlightGearVisualiser.RATE},"
             f"{FlightGearVisualiser.SERVER},"
             f"{FlightGearVisualiser.PORT},"
             f"{FlightGearVisualiser.PROTOCOL}"
         )
-        flight_model_type_arg = "--fdm=" + "external"
+        flight_model_type_arg = "--fdm=" + "null"
         disable_ai_arg = "--disable-ai-traffic"
         disable_live_weather_arg = "--disable-real-weather-fetch"
         time_of_day_arg = "--timeofday=" + FlightGearVisualiser.TIME
         return (
             flightgear_cmd,
             aircraft_arg,
             flight_model_arg,
```

### Comparing `jsbgym-0.3.1/jsbgym.egg-info/PKG-INFO` & `jsbgym-0.3.2/jsbgym.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,91 @@
 Metadata-Version: 2.1
 Name: jsbgym
-Version: 0.3.1
+Version: 0.3.2
 Summary: A package of reinforcement learning environments for flight control using the JSBSim flight dynamics model.
 Author: sryu1
 License: MIT
 Project-URL: Homepage, https://github.com/sryu1/jsbgym
 Project-URL: Repository, https://github.com/sryu1/jsbgym
 Project-URL: Bug Tracker, https://github.com/sryu1/jsbgym/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: gymnasium
 Requires-Dist: jsbsim
 Requires-Dist: matplotlib
 
 # JSBGym
 
 [![Python: 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
 [![PyPI Version](https://img.shields.io/pypi/v/jsbgym)](https://pypi.org/project/jsbgym)
-[![PyPI downloads](https://img.shields.io/pypi/dm/jsbgym.svg)](https://pypistats.org/packages/jsbgym)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/jsbgym)](https://pypistats.org/packages/jsbgym)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 JSBGym provides reinforcement learning environments for the control of fixed-wing aircraft using the JSBSim flight dynamics model. The package's environments implement the Farama-Foundation's Gymnasium interface allowing environments to be created and interacted with.
 
 ![Example](https://github.com/sryu1/jsbgym/blob/main/docs/J3.gif?raw=true)
 
 Pretrained models can be found [here](https://huggingface.co/sryu1/jsbgym_models)
 
 ## Setup
 
-Open a terminal and install jsbgym:
+### Windows
+
+Open a terminal and install jsbgym via pip:
+
+```console
+pip install jsbgym
+```
+
+To render the environment with FlightGear, download and install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`) and if not already existant, add a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`).
+
+If there are aircraft installed in a different location, add the folder to the `FG_AIRCRAFT` system variable.
+3D visualisation requires installation of the FlightGear simulator. Confirm FlightGear is runnable from terminal with:
+
+```console
+fgfs --version
+```
+
+### Linux
+
+Open a terminal and install jsbgym via pip:
 
 ```console
 pip install jsbgym
 ```
 
-For Linux systems, rendering with some modes will require an additional package:
+Rendering with some modes will require an additional package:
 
 ```console
 sudo apt-get install python3-tk
 ```
 
-To render the environment with FlightGear, dowloand and install it from [here](https://sourceforge.net/projects/flightgear/). Make sure the FlightGear bin directory is in PATH (Usually `C:\Program Files\FlightGear 2020.3\bin`) and if not already existant, add a system variable called `FG_ROOT` with the FG data folder as it's value (Usually `C:\Program Files\FlightGear 2020.3\data`). For Linux, rename the AppImage file to fgfs.AppImage and place it in /usr/local/bin/fgfs. The data file must also be downloaded from [here](https://sourceforge.net/projects/flightgear/files/release-2020.3/) (approximately 2 GB) then in terminal, enter
+Rename the AppImage file to `fgfs` and place it in `/usr/local/bin`:
+
+```console
+sudo mv fgfs /usr/local/bin
+```
+
+The data files must also be downloaded from [here](https://sourceforge.net/projects/flightgear/files/release-2020.3/) (approximately 2 GB) then in terminal, enter
 
 ```console
-export FG_ROOT=/path/to/folder
+export FG_ROOT=/path/to/datafolder
 ```
 
 If there are aircraft installed in a different location, add the folder to the `FG_AIRCRAFT` system variable.
-3D visualisation requires installation of the FlightGear simulator. Confirm it is runnable from terminal with:
+3D visualisation requires installation of the FlightGear simulator. Confirm FlightGear is runnable from terminal with:
 
 ```console
 fgfs --version
 ```
 
 ## Getting Started
```

### Comparing `jsbgym-0.3.1/jsbgym.egg-info/SOURCES.txt` & `jsbgym-0.3.2/jsbgym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsbgym-0.3.1/pyproject.toml` & `jsbgym-0.3.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsbgym"
-version = "0.3.1"
+version = "0.3.2"
 authors = [{ name = "sryu1" }]
 readme = "README.md"
 license = { text = "MIT" }
 description = "A package of reinforcement learning environments for flight control using the JSBSim flight dynamics model."
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 
 requires-python = ">=3.8"
 dependencies = ["numpy", "gymnasium", "jsbsim", "matplotlib"]
 
 [project.urls]
```

