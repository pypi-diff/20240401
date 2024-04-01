# Comparing `tmp/Xodia24-0.0.3.tar.gz` & `tmp/Xodia24-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Xodia24-0.0.3.tar", last modified: Mon Apr  1 14:43:17 2024, max compression
+gzip compressed data, was "Xodia24-0.0.4.tar", last modified: Mon Apr  1 14:49:53 2024, max compression
```

## Comparing `Xodia24-0.0.3.tar` & `Xodia24-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 14:43:17.702555 Xodia24-0.0.3/
--rw-rw-rw-   0        0        0     1088 2024-04-01 14:18:58.000000 Xodia24-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     6232 2024-04-01 14:43:17.694486 Xodia24-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5485 2024-04-01 14:43:01.000000 Xodia24-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 14:43:17.694486 Xodia24-0.0.3/Xodia24.egg-info/
--rw-rw-rw-   0        0        0     6232 2024-04-01 14:43:16.000000 Xodia24-0.0.3/Xodia24.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2024-04-01 14:43:17.000000 Xodia24-0.0.3/Xodia24.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 14:43:16.000000 Xodia24-0.0.3/Xodia24.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-01 14:43:16.000000 Xodia24-0.0.3/Xodia24.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 14:43:16.000000 Xodia24-0.0.3/Xodia24.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 14:43:17.702555 Xodia24-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1200 2024-04-01 14:43:12.000000 Xodia24-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:49:53.044259 Xodia24-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2024-04-01 14:18:58.000000 Xodia24-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     6226 2024-04-01 14:49:53.039207 Xodia24-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5481 2024-04-01 14:49:23.000000 Xodia24-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 14:49:53.037164 Xodia24-0.0.4/Xodia24.egg-info/
+-rw-rw-rw-   0        0        0     6226 2024-04-01 14:49:52.000000 Xodia24-0.0.4/Xodia24.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2024-04-01 14:49:52.000000 Xodia24-0.0.4/Xodia24.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 14:49:52.000000 Xodia24-0.0.4/Xodia24.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-01 14:49:52.000000 Xodia24-0.0.4/Xodia24.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 14:49:52.000000 Xodia24-0.0.4/Xodia24.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 14:49:53.044259 Xodia24-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1200 2024-04-01 14:49:46.000000 Xodia24-0.0.4/setup.py
```

### Comparing `Xodia24-0.0.3/LICENSE` & `Xodia24-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Xodia24-0.0.3/PKG-INFO` & `Xodia24-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xodia24
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package providing a custom environment for simulating tank battles
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,reinforcement-learning,tank-battle
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -100,15 +100,15 @@
 
 # Example usage:
 if __name__ == "__main__":
     # Instantiate the environment with the custom reward function
     env = CustomPocketTank()
 
     # Optionally, you can train your RL model using this environment
-
+```
 
 ### Action Space
 
 The action space in the Xodia24 PocketTank environment refers to the set of possible actions that the reinforcement learning (RL) agent can take at each time step. In the tank battle scenario, the agent controls one of the tanks and has several actions available to it, including adjusting the power and angle of the tank's cannon and moving the tank across the 2D grid.
 
 #### Available Actions:
 - **Adjust Power**: The agent can adjust the power setting of the tank's cannon, determining the force with which the projectile is fired.
@@ -125,9 +125,7 @@
 - **Tank Positions**: The coordinates of both the agent-controlled tank and the opponent tank on the 2D grid.
 - **Terrain Information**: Information about the terrain features, such as obstacles or cover, that may affect the trajectory of the projectile.
 - **Projectile Position**: The current position of the projectile fired by the tanks.
 
 The observation space can be represented as a vector, matrix, or other data structure depending on the complexity of the environment and the information that needs to be conveyed to the agent.
 
 
-```
-
```

### Comparing `Xodia24-0.0.3/README.md` & `Xodia24-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 # Example usage:
 if __name__ == "__main__":
     # Instantiate the environment with the custom reward function
     env = CustomPocketTank()
 
     # Optionally, you can train your RL model using this environment
-
+```
 
 ### Action Space
 
 The action space in the Xodia24 PocketTank environment refers to the set of possible actions that the reinforcement learning (RL) agent can take at each time step. In the tank battle scenario, the agent controls one of the tanks and has several actions available to it, including adjusting the power and angle of the tank's cannon and moving the tank across the 2D grid.
 
 #### Available Actions:
 - **Adjust Power**: The agent can adjust the power setting of the tank's cannon, determining the force with which the projectile is fired.
@@ -107,9 +107,7 @@
 - **Tank Positions**: The coordinates of both the agent-controlled tank and the opponent tank on the 2D grid.
 - **Terrain Information**: Information about the terrain features, such as obstacles or cover, that may affect the trajectory of the projectile.
 - **Projectile Position**: The current position of the projectile fired by the tanks.
 
 The observation space can be represented as a vector, matrix, or other data structure depending on the complexity of the environment and the information that needs to be conveyed to the agent.
 
 
-```
-
```

### Comparing `Xodia24-0.0.3/Xodia24.egg-info/PKG-INFO` & `Xodia24-0.0.4/Xodia24.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xodia24
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package providing a custom environment for simulating tank battles
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,reinforcement-learning,tank-battle
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -100,15 +100,15 @@
 
 # Example usage:
 if __name__ == "__main__":
     # Instantiate the environment with the custom reward function
     env = CustomPocketTank()
 
     # Optionally, you can train your RL model using this environment
-
+```
 
 ### Action Space
 
 The action space in the Xodia24 PocketTank environment refers to the set of possible actions that the reinforcement learning (RL) agent can take at each time step. In the tank battle scenario, the agent controls one of the tanks and has several actions available to it, including adjusting the power and angle of the tank's cannon and moving the tank across the 2D grid.
 
 #### Available Actions:
 - **Adjust Power**: The agent can adjust the power setting of the tank's cannon, determining the force with which the projectile is fired.
@@ -125,9 +125,7 @@
 - **Tank Positions**: The coordinates of both the agent-controlled tank and the opponent tank on the 2D grid.
 - **Terrain Information**: Information about the terrain features, such as obstacles or cover, that may affect the trajectory of the projectile.
 - **Projectile Position**: The current position of the projectile fired by the tanks.
 
 The observation space can be represented as a vector, matrix, or other data structure depending on the complexity of the environment and the information that needs to be conveyed to the agent.
 
 
-```
-
```

### Comparing `Xodia24-0.0.3/setup.py` & `Xodia24-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'Python package providing a custom environment for simulating tank battles'
 LONG_DESCRIPTION = 'Xodia24 is a Python package providing a custom environment for simulating a tank battle scenario where two tanks are positioned on a 2D grid.'
 
 # Setting up
 setup(
     name="Xodia24",
     version=VERSION,
```

