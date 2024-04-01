# Comparing `tmp/Xodia24-0.0.2.tar.gz` & `tmp/Xodia24-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Xodia24-0.0.2.tar", last modified: Mon Apr  1 14:42:11 2024, max compression
+gzip compressed data, was "Xodia24-0.0.3.tar", last modified: Mon Apr  1 14:43:17 2024, max compression
```

## Comparing `Xodia24-0.0.2.tar` & `Xodia24-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 14:42:11.869027 Xodia24-0.0.2/
--rw-rw-rw-   0        0        0     1088 2024-04-01 14:18:58.000000 Xodia24-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     6219 2024-04-01 14:42:11.865513 Xodia24-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5472 2024-04-01 14:13:06.000000 Xodia24-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 14:42:11.862864 Xodia24-0.0.2/Xodia24.egg-info/
--rw-rw-rw-   0        0        0     6219 2024-04-01 14:42:11.000000 Xodia24-0.0.2/Xodia24.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2024-04-01 14:42:11.000000 Xodia24-0.0.2/Xodia24.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 14:42:11.000000 Xodia24-0.0.2/Xodia24.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-01 14:42:11.000000 Xodia24-0.0.2/Xodia24.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 14:42:11.000000 Xodia24-0.0.2/Xodia24.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 14:42:11.872552 Xodia24-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1200 2024-04-01 14:41:46.000000 Xodia24-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:43:17.702555 Xodia24-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2024-04-01 14:18:58.000000 Xodia24-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     6232 2024-04-01 14:43:17.694486 Xodia24-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5485 2024-04-01 14:43:01.000000 Xodia24-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 14:43:17.694486 Xodia24-0.0.3/Xodia24.egg-info/
+-rw-rw-rw-   0        0        0     6232 2024-04-01 14:43:16.000000 Xodia24-0.0.3/Xodia24.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2024-04-01 14:43:17.000000 Xodia24-0.0.3/Xodia24.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 14:43:16.000000 Xodia24-0.0.3/Xodia24.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-01 14:43:16.000000 Xodia24-0.0.3/Xodia24.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 14:43:16.000000 Xodia24-0.0.3/Xodia24.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 14:43:17.702555 Xodia24-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1200 2024-04-01 14:43:12.000000 Xodia24-0.0.3/setup.py
```

### Comparing `Xodia24-0.0.2/LICENSE` & `Xodia24-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Xodia24-0.0.2/PKG-INFO` & `Xodia24-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xodia24
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package providing a custom environment for simulating tank battles
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,reinforcement-learning,tank-battle
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -14,16 +14,16 @@
 License-File: LICENSE
 Requires-Dist: gymnasium
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 
 # Xodia24: PocketTank Environment
 
- <p  align="center">
-<img src="https://i.ibb.co/P4nyZNv/Xodia-Logo-removebg-preview.png" alt="Xodia-Logo-removebg-preview" border="0">
+<p  align="center">
+<img src="https://i.ibb.co/P4nyZNv/Xodia-Logo-removebg-preview.png" alt="Xodia-Logo-removebg-preview" border="0" width="400px">
 </p>
   
 
 Xodia24 is a Python package providing a custom environment for simulating a tank battle scenario where two tanks are positioned on a 2D grid. The objective is to train a Reinforcement Learning (RL) agent to effectively control one of the tanks and shoot at the other tank using different actions such as adjusting power, angle, and moving the tank.
 
 ## Installation
```

### Comparing `Xodia24-0.0.2/README.md` & `Xodia24-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Xodia24: PocketTank Environment
 
- <p  align="center">
-<img src="https://i.ibb.co/P4nyZNv/Xodia-Logo-removebg-preview.png" alt="Xodia-Logo-removebg-preview" border="0">
+<p  align="center">
+<img src="https://i.ibb.co/P4nyZNv/Xodia-Logo-removebg-preview.png" alt="Xodia-Logo-removebg-preview" border="0" width="400px">
 </p>
   
 
 Xodia24 is a Python package providing a custom environment for simulating a tank battle scenario where two tanks are positioned on a 2D grid. The objective is to train a Reinforcement Learning (RL) agent to effectively control one of the tanks and shoot at the other tank using different actions such as adjusting power, angle, and moving the tank.
 
 ## Installation
```

### Comparing `Xodia24-0.0.2/Xodia24.egg-info/PKG-INFO` & `Xodia24-0.0.3/Xodia24.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xodia24
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package providing a custom environment for simulating tank battles
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,reinforcement-learning,tank-battle
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -14,16 +14,16 @@
 License-File: LICENSE
 Requires-Dist: gymnasium
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 
 # Xodia24: PocketTank Environment
 
- <p  align="center">
-<img src="https://i.ibb.co/P4nyZNv/Xodia-Logo-removebg-preview.png" alt="Xodia-Logo-removebg-preview" border="0">
+<p  align="center">
+<img src="https://i.ibb.co/P4nyZNv/Xodia-Logo-removebg-preview.png" alt="Xodia-Logo-removebg-preview" border="0" width="400px">
 </p>
   
 
 Xodia24 is a Python package providing a custom environment for simulating a tank battle scenario where two tanks are positioned on a 2D grid. The objective is to train a Reinforcement Learning (RL) agent to effectively control one of the tanks and shoot at the other tank using different actions such as adjusting power, angle, and moving the tank.
 
 ## Installation
```

### Comparing `Xodia24-0.0.2/setup.py` & `Xodia24-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'Python package providing a custom environment for simulating tank battles'
 LONG_DESCRIPTION = 'Xodia24 is a Python package providing a custom environment for simulating a tank battle scenario where two tanks are positioned on a 2D grid.'
 
 # Setting up
 setup(
     name="Xodia24",
     version=VERSION,
```

