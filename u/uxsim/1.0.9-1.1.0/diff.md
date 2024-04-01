# Comparing `tmp/uxsim-1.0.9.tar.gz` & `tmp/uxsim-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uxsim-1.0.9.tar", last modified: Tue Mar 26 07:36:35 2024, max compression
+gzip compressed data, was "uxsim-1.1.0.tar", last modified: Mon Apr  1 12:21:14 2024, max compression
```

## Comparing `uxsim-1.0.9.tar` & `uxsim-1.1.0.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 07:36:35.314672 uxsim-1.0.9/
--rw-rw-rw-   0        0        0     1086 2023-08-01 08:45:01.000000 uxsim-1.0.9/LICENSE
--rw-rw-rw-   0        0        0       21 2024-03-26 06:39:30.000000 uxsim-1.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0    13467 2024-03-26 07:36:35.310672 uxsim-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0    12566 2024-03-22 06:04:06.000000 uxsim-1.0.9/README.md
--rw-rw-rw-   0        0        0     1132 2024-03-26 07:35:12.000000 uxsim-1.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-26 07:36:35.314672 uxsim-1.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-26 07:36:35.267674 uxsim-1.0.9/tests/
--rw-rw-rw-   0        0        0     1523 2024-03-26 07:35:12.000000 uxsim-1.0.9/tests/test_examples.py
--rw-rw-rw-   0        0        0     1682 2024-03-26 03:14:04.000000 uxsim-1.0.9/tests/test_result_gui_viewer.py
--rw-rw-rw-   0        0        0     3326 2024-03-26 04:14:08.000000 uxsim-1.0.9/tests/test_verification_exceptional.py
--rw-rw-rw-   0        0        0    40619 2024-03-22 02:43:13.000000 uxsim-1.0.9/tests/test_verification_node.py
--rw-rw-rw-   0        0        0    22315 2024-03-22 02:43:13.000000 uxsim-1.0.9/tests/test_verification_route_choice.py
--rw-rw-rw-   0        0        0     3784 2024-03-22 02:43:13.000000 uxsim-1.0.9/tests/test_verification_sioux_falls.py
--rw-rw-rw-   0        0        0    39162 2024-03-26 04:14:43.000000 uxsim-1.0.9/tests/test_verification_straight_road.py
-drwxrwxrwx   0        0        0        0 2024-03-26 07:36:35.271671 uxsim-1.0.9/uxsim/
-drwxrwxrwx   0        0        0        0 2024-03-26 07:36:35.297673 uxsim-1.0.9/uxsim/OSMImporter/
--rw-rw-rw-   0        0        0    14794 2024-03-25 07:21:53.000000 uxsim-1.0.9/uxsim/OSMImporter/OSMImporter.py
--rw-rw-rw-   0        0        0       26 2024-03-26 02:31:54.000000 uxsim-1.0.9/uxsim/OSMImporter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 07:36:35.300673 uxsim-1.0.9/uxsim/ResultGUIViewer/
--rw-rw-rw-   0        0        0    17647 2024-03-26 04:06:25.000000 uxsim-1.0.9/uxsim/ResultGUIViewer/ResultGUIViewer.py
--rw-rw-rw-   0        0        0       30 2024-03-25 09:10:21.000000 uxsim-1.0.9/uxsim/ResultGUIViewer/__init__.py
--rw-rw-rw-   0        0        0      168 2024-03-26 07:14:06.000000 uxsim-1.0.9/uxsim/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 07:36:35.304672 uxsim-1.0.9/uxsim/files/
--rw-rw-rw-   0        0        0    58464 2024-03-26 07:35:12.000000 uxsim-1.0.9/uxsim/files/Inconsolata.otf
--rw-rw-rw-   0        0        0     4486 2024-03-26 07:35:12.000000 uxsim-1.0.9/uxsim/files/Licence_of_Inconsolata.otf.txt
--rw-rw-rw-   0        0        0       47 2024-03-26 07:35:12.000000 uxsim-1.0.9/uxsim/files/README.md
--rw-rw-rw-   0        0        0        0 2024-03-26 07:35:12.000000 uxsim-1.0.9/uxsim/files/__init__.py
--rw-rw-rw-   0        0        0     3093 2024-03-22 02:43:13.000000 uxsim-1.0.9/uxsim/utils.py
--rw-rw-rw-   0        0        0   123682 2024-03-26 07:35:12.000000 uxsim-1.0.9/uxsim/uxsim.py
-drwxrwxrwx   0        0        0        0 2024-03-26 07:36:35.308672 uxsim-1.0.9/uxsim.egg-info/
--rw-rw-rw-   0        0        0    13467 2024-03-26 07:36:35.000000 uxsim-1.0.9/uxsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2024-03-26 07:36:35.000000 uxsim-1.0.9/uxsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 07:36:35.000000 uxsim-1.0.9/uxsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2024-03-26 07:36:35.000000 uxsim-1.0.9/uxsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-26 07:36:35.000000 uxsim-1.0.9/uxsim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 12:21:14.674981 uxsim-1.1.0/
+-rw-rw-rw-   0        0        0     1086 2023-08-01 08:45:01.000000 uxsim-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       21 2024-03-26 06:39:30.000000 uxsim-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    14009 2024-04-01 12:21:14.673967 uxsim-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13108 2024-04-01 11:09:22.000000 uxsim-1.1.0/README.md
+-rw-rw-rw-   0        0        0     1132 2024-03-26 09:57:16.000000 uxsim-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 12:21:14.674981 uxsim-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 12:21:14.609380 uxsim-1.1.0/tests/
+-rw-rw-rw-   0        0        0     1523 2024-03-26 09:57:16.000000 uxsim-1.1.0/tests/test_examples.py
+-rw-rw-rw-   0        0        0     1682 2024-03-26 03:14:04.000000 uxsim-1.1.0/tests/test_result_gui_viewer.py
+-rw-rw-rw-   0        0        0     3326 2024-03-26 04:14:08.000000 uxsim-1.1.0/tests/test_verification_exceptional.py
+-rw-rw-rw-   0        0        0    69316 2024-04-01 11:10:22.000000 uxsim-1.1.0/tests/test_verification_multilane.py
+-rw-rw-rw-   0        0        0    42414 2024-03-29 08:55:07.000000 uxsim-1.1.0/tests/test_verification_node.py
+-rw-rw-rw-   0        0        0    22326 2024-03-31 13:21:16.000000 uxsim-1.1.0/tests/test_verification_route_choice.py
+-rw-rw-rw-   0        0        0     3784 2024-03-22 02:43:13.000000 uxsim-1.1.0/tests/test_verification_sioux_falls.py
+-rw-rw-rw-   0        0        0    39162 2024-03-26 04:14:43.000000 uxsim-1.1.0/tests/test_verification_straight_road.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:21:14.614969 uxsim-1.1.0/uxsim/
+drwxrwxrwx   0        0        0        0 2024-04-01 12:21:14.642968 uxsim-1.1.0/uxsim/OSMImporter/
+-rw-rw-rw-   0        0        0    16170 2024-04-01 09:24:47.000000 uxsim-1.1.0/uxsim/OSMImporter/OSMImporter.py
+-rw-rw-rw-   0        0        0       26 2024-03-26 02:31:54.000000 uxsim-1.1.0/uxsim/OSMImporter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:21:14.646971 uxsim-1.1.0/uxsim/ResultGUIViewer/
+-rw-rw-rw-   0        0        0    17979 2024-03-27 03:42:24.000000 uxsim-1.1.0/uxsim/ResultGUIViewer/ResultGUIViewer.py
+-rw-rw-rw-   0        0        0       30 2024-03-25 09:10:21.000000 uxsim-1.1.0/uxsim/ResultGUIViewer/__init__.py
+-rw-rw-rw-   0        0        0      193 2024-04-01 07:03:19.000000 uxsim-1.1.0/uxsim/__init__.py
+-rw-rw-rw-   0        0        0    53987 2024-03-29 05:21:02.000000 uxsim-1.1.0/uxsim/analyzer.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:21:14.671935 uxsim-1.1.0/uxsim/files/
+-rw-rw-rw-   0        0        0 10695124 2023-05-03 08:50:59.000000 uxsim-1.1.0/uxsim/files/HackGen-Regular.ttf
+-rw-rw-rw-   0        0        0    58464 2024-03-26 09:57:16.000000 uxsim-1.1.0/uxsim/files/Inconsolata.otf
+-rw-rw-rw-   0        0        0     5826 2024-03-27 03:00:30.000000 uxsim-1.1.0/uxsim/files/LICENSE_of_HackGen-Regular
+-rw-rw-rw-   0        0        0     4486 2024-03-26 09:57:16.000000 uxsim-1.1.0/uxsim/files/Licence_of_Inconsolata.otf.txt
+-rw-rw-rw-   0        0        0       47 2024-03-26 09:57:16.000000 uxsim-1.1.0/uxsim/files/README.md
+-rw-rw-rw-   0        0        0        0 2024-03-26 09:57:16.000000 uxsim-1.1.0/uxsim/files/__init__.py
+-rw-rw-rw-   0        0        0     3093 2024-03-22 02:43:13.000000 uxsim-1.1.0/uxsim/utils.py
+-rw-rw-rw-   0        0        0    77449 2024-04-01 10:29:15.000000 uxsim-1.1.0/uxsim/uxsim.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:21:14.672953 uxsim-1.1.0/uxsim.egg-info/
+-rw-rw-rw-   0        0        0    14009 2024-04-01 12:21:14.000000 uxsim-1.1.0/uxsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2024-04-01 12:21:14.000000 uxsim-1.1.0/uxsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 12:21:14.000000 uxsim-1.1.0/uxsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2024-04-01 12:21:14.000000 uxsim-1.1.0/uxsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-01 12:21:14.000000 uxsim-1.1.0/uxsim.egg-info/top_level.txt
```

### Comparing `uxsim-1.0.9/LICENSE` & `uxsim-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uxsim-1.0.9/PKG-INFO` & `uxsim-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uxsim
-Version: 1.0.9
+Version: 1.1.0
 Summary: UXsim: traffic flow simulator
 Author-email: Toru Seo <seo.t.aa@m.titech.ac.jp>
 License: MIT License
 Project-URL: Homepage, https://github.com/toruseo/UXsim
 Project-URL: Download, https://github.com/toruseo/UXsim
 Project-URL: Bug Tracker, https://github.com/toruseo/UXsim/issues
 Classifier: Intended Audience :: Science/Research
@@ -42,18 +42,19 @@
 
 - [Jupyter Notebook](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_01en.ipynb) or [Google Colab](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb): Interactive demonstrations and tutorials
 - [Technical Documentation](https://toruseo.jp/UXsim/docs/index.html): Detailed documents on tutorials, simulation mechanism, and specifications of modules/functions
 
 ## Main Features
 
 - Simple, lightweight, and easy-to-use Python implementation of the modern standard models of dynamic network traffic flow.
-- Traffic flow simulation with a given network and time-dependent OD demand (dynamic traffic assignment).
+- Macroscopic traffic simulation: Simulating over 60000 vehicles in 30 seconds in a city.
+- Dynamic traffic assignment: Traffic flow simulation with a given network and time-dependent OD demand.
 - Implementation of traffic control/management schemes such as traffic signals and road pricing.
 - Basic analysis of simulation results and their export to pandas.DataFrame and CSV files.
-- Visualization of simulation results including animation.
+- Visualization of simulation results using matplotlib. Interactive GUI is available.
 - Flexible and customizable thanks to pure Python implementation. Can also be directly integrated with other Python-based frameworks, such as PyTorch for deep reinforcement learning traffic control.
 
 ## Simulation Examples
 
 ### Large-scale scenario
 
 Belows are simulation result where approximately 60000 vehicles pass through a 10km x 10km grid network in 2 hours. The computation time was about 30 seconds on a standard desktop PC.
@@ -75,14 +76,18 @@
 [Jupyter Notebook of this example](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_03en_pytorch.ipynb) is available.
 
 <p float="left">
 <img src="https://github.com/toruseo/UXsim/blob/images/anim_network1_0.22_nocontrol.gif" width="400"/>
 <img src="https://github.com/toruseo/UXsim/blob/images/anim_network1_0.22_DQL.gif" width="400"/>
 </p>
 
+### Interactive GUI for exploring a simulation result
+
+https://github.com/toruseo/UXsim/assets/34780089/ec780a33-d9ba-4068-a005-0b06127196d9
+
 ## Install
 
 ### Using pip
 
 The simplest way is using pip to install from PyPI.
 
 ```
@@ -109,18 +114,16 @@
 	
 ### Manual install
 
 Download the `uxsim` directory from this Github repo or [the latest release](https://github.com/toruseo/UXsim/releases/latest/download/uxsim.zip) and place it to your local directory as follows:
 ```
 your_project_directory/
 ├── uxsim/ 	# The uxsim directory
-│ ├── utils/ 	# Utility files of UXsim
 │ ├── uxsim.py 	# The main code of UXsim. You can customize this as you wish
-│ ├── utils.py 	# Utility funcsions of UXsim
-│ └── ... 	# Other files in uxsim
+│ └── ... 	# Other files and directories in uxsim
 ├── your_simulation_code.py 		# Your code if nessesary
 ├── your_simulation_notebook.ipynb 	# Your Jupyter notebook if nessesary
 ├── ... 	# Other files if nessesary
 ```
 In this way, you can flexibly customize UXsim by your own.
 
 </details>
@@ -152,69 +155,74 @@
 )
 
 # Define the scenario
 W.addNode("orig1", 0, 0) # Create a node
 W.addNode("orig2", 0, 2)
 W.addNode("merge", 1, 1)
 W.addNode("dest", 2, 1)
-W.addLink("link1", "orig1", "merge", length=1000, free_flow_speed=20, jam_density=0.2, merge_priority=0.5) # Create a link
-W.addLink("link2", "orig2", "merge", length=1000, free_flow_speed=20, jam_density=0.2, merge_priority=2)
-W.addLink("link3", "merge", "dest", length=1000, free_flow_speed=20, jam_density=0.2)
-W.adddemand("orig1", "dest", 0, 1000, 0.4) # Create OD traffic demand
-W.adddemand("orig2", "dest", 500, 1000, 0.6)
+W.addLink("link1", "orig1", "merge", length=1000, free_flow_speed=20) # Create a link
+W.addLink("link2", "orig2", "merge", length=1000, free_flow_speed=20)
+W.addLink("link3", "merge", "dest", length=1000, free_flow_speed=20)
+W.adddemand("orig1", "dest", 0, 1000, 0.45) # Create OD traffic demand
+W.adddemand("orig2", "dest", 400, 1000, 0.6)
 
 # Run the simulation to the end
 W.exec_simulation()
 
 # Print summary of simulation result
 W.analyzer.print_simple_stats()
 
 # Visualize snapshots of network traffic state for several timesteps
-W.analyzer.network(0, detailed=1, network_font_size=0)
-W.analyzer.network(500, detailed=1, network_font_size=0)
-W.analyzer.network(1000, detailed=1, network_font_size=0)
+W.analyzer.network(100, detailed=1, network_font_size=12)
+W.analyzer.network(600, detailed=1, network_font_size=12)
+W.analyzer.network(800, detailed=1, network_font_size=12)
 ```
 
 It would output text to the terminal and images to `out` directory like below:
 ```
 simulation setting:
  scenario name:
  simulation duration:    1200 s
- number of vehicles:     700 veh
+ number of vehicles:     810 veh
  total road length:      3000 m
  time discret. width:    5 s
  platoon size:           5 veh
  number of timesteps:    240
- number of platoons:     140
+ number of platoons:     162
  number of links:        3
  number of nodes:        4
  setup time:             0.00 s
 simulating...
       time| # of vehicles| ave speed| computation time
        0 s|        0 vehs|   0.0 m/s|     0.00 s
-     600 s|      100 vehs|  17.5 m/s|     0.03 s
-    1195 s|       25 vehs|  20.0 m/s|     0.05 s
+     600 s|      130 vehs|  13.7 m/s|     0.03 s
+    1195 s|       75 vehs|  12.3 m/s|     0.06 s
  simulation finished
 results:
- average speed:  13.8 m/s
- number of completed trips:      675 / 700
- average travel time of trips:   142.7 s
- average delay of trips:         42.7 s
- delay ratio:                    0.299
+ average speed:  11.6 m/s
+ number of completed trips:      735 / 810
+ average travel time of trips:   162.6 s
+ average delay of trips:         62.6 s
+ delay ratio:                    0.385
 ```
 <p float="left">
-<img src="https://github.com/toruseo/UXsim/blob/images/simple_example_network1_1000.png" width="400"/>
+<img src="https://github.com/toruseo/UXsim/blob/images/network1_100.png" width="250"/>
+<img src="https://github.com/toruseo/UXsim/blob/images/network1_600.png" width="250"/>
+<img src="https://github.com/toruseo/UXsim/blob/images/network1_800.png" width="250"/>
 </p>
 
 ## Main Files
 
 - `uxsim` directory: UXsim main package
 	- `uxsim/uxsim.py`: UXsim main code
+	- `uxsim/analyzer.py`: Simulation result analysis code
 	- `uxsim/utils.py`: UXsim utilities code
- 	- `uxsim/utils` directory:  UXsim utilities files
+	- `uxsim/ResultGUIViewer/ResultGUIViewer.py`: Submodule on GUI for visualizing simulation results
+	- `uxsim/OSMImporter/OSMImporter.py`: Submodule on road network import from OpenStreetMap (experimental)
+ 	- `uxsim/files` directory: UXsim utilities files
 - `demos_and_examples` directory: Tutorials and examples of UXsim
 - `dat` directory: Sample scenario files
 - `tests`, `.github` directories: Development-related files
 
 ## Further Reading
 
 If you want to know the details of UXsim, please see
@@ -236,27 +244,27 @@
 ## Contributing and Discussion
 
 Contribution is welcome!
 For minor changes including bug fixes, please submit a pull request.
 Please make sure that your codes pass the automatic tests in Github Action.
 If you want a major change, please start a discussion at [Issues](https://github.com/toruseo/UXsim/issues) page first.
 
-If you have any questions or suggestions, please start a discussion at [Issues](https://github.com/toruseo/UXsim/issues) page (in English or Japanese).
+If you have any questions or suggestions, please start a discussion at [Discussions](https://github.com/toruseo/UXsim/discussions) page (in English or Japanese).
 
 I (Toru Seo) work on this project in my spare time. Please understand that my response may be delayed.
 
 ## Acknowledgments
 
 UXsim is based on various works in traffic flow theory and related fields. We would like to acknowledge the contributions of the research community in advancing this field.
 Especially, UXsim directly uses the following works:
 
 - [Newell's simplified car-following model](https://doi.org/10.1016/S0191-2615(00)00044-8) and its extention [X-model](https://doi.org/10.1016/j.trb.2013.02.008)
 - [Incremental Node Model](https://doi.org/10.1016/j.trb.2011.04.001) and its [mesoscopic version](https://ubiquitypress.com/site/chapters/e/10.5334/baw.50/)
 - [Dynamic User Optimum](https://doi.org/10.1016/S0191-2615(00)00005-9)-type Route Choice Model
 
 ## Related Links
 
-- [Toru Seo (Author)](https://toruseo.jp/)
+- [Toru Seo (Author)](https://toruseo.jp/index_en.html)
 - [Collection of related simulators by Seo](https://toruseo.jp/uxsim/index_en.html)
 - Japanese book "[Macroscopic Traffic Simulation: Fundamental Mathematical Theory and Python Implementation](https://www.coronasha.co.jp/np/isbn/9784339052794/)" (Author: [Toru Seo](https://toruseo.jp/), Publisher: [Corona Publishing Co., Ltd.](https://www.coronasha.co.jp/)): UXsim is a significant expansion of the traffic flow simulator *UroborosX* described in this book.
-- [Seo Laboratory, Tokyo Institute of Technology](http://seo.cv.ens.titech.ac.jp/)
+- [Seo Laboratory, Tokyo Institute of Technology](http://seo.cv.ens.titech.ac.jp/en/)
 - [Interactive Traffic Flow Simulator that Runs on a Web Browser](http://seo.cv.ens.titech.ac.jp/traffic-flow-demo/bottleneck.html): Play with the same link traffic flow model used in this simulator interactively, and learn the basics of traffic flow and its simulation.
```

### Comparing `uxsim-1.0.9/README.md` & `uxsim-1.1.0/uxsim.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: uxsim
+Version: 1.1.0
+Summary: UXsim: traffic flow simulator
+Author-email: Toru Seo <seo.t.aa@m.titech.ac.jp>
+License: MIT License
+Project-URL: Homepage, https://github.com/toruseo/UXsim
+Project-URL: Download, https://github.com/toruseo/UXsim
+Project-URL: Bug Tracker, https://github.com/toruseo/UXsim/issues
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.21.5
+Requires-Dist: matplotlib>=3.5.2
+Requires-Dist: pillow>=9.2.0
+Requires-Dist: tqdm>=4.64.1
+Requires-Dist: scipy>=1.9.1
+Requires-Dist: pandas>=1.4.4
+Requires-Dist: PyQt5>=5.15.7
+
 # UXsim: Network traffic flow simulator in pure Python
 
 [![PyPi](https://img.shields.io/pypi/v/uxsim.svg)](https://pypi.python.org/pypi/uxsim)
 [![](https://tokei.rs/b1/github/toruseo/UXsim?style=flat&category=code&color=dddd22)](https://github.com/toruseo/UXsim)
 [![](https://tokei.rs/b1/github/toruseo/UXsim?category=comments&style=flat&color=44cc44)](https://github.com/toruseo/UXsim/)
 [![Demo in Colab](https://colab.research.google.com/assets/colab-badge.svg)](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb)
 [![arXiv](https://img.shields.io/badge/arXiv-2309.17114-b31b1b.svg)](http://dx.doi.org/10.48550/arXiv.2309.17114)
@@ -17,18 +42,19 @@
 
 - [Jupyter Notebook](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_01en.ipynb) or [Google Colab](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb): Interactive demonstrations and tutorials
 - [Technical Documentation](https://toruseo.jp/UXsim/docs/index.html): Detailed documents on tutorials, simulation mechanism, and specifications of modules/functions
 
 ## Main Features
 
 - Simple, lightweight, and easy-to-use Python implementation of the modern standard models of dynamic network traffic flow.
-- Traffic flow simulation with a given network and time-dependent OD demand (dynamic traffic assignment).
+- Macroscopic traffic simulation: Simulating over 60000 vehicles in 30 seconds in a city.
+- Dynamic traffic assignment: Traffic flow simulation with a given network and time-dependent OD demand.
 - Implementation of traffic control/management schemes such as traffic signals and road pricing.
 - Basic analysis of simulation results and their export to pandas.DataFrame and CSV files.
-- Visualization of simulation results including animation.
+- Visualization of simulation results using matplotlib. Interactive GUI is available.
 - Flexible and customizable thanks to pure Python implementation. Can also be directly integrated with other Python-based frameworks, such as PyTorch for deep reinforcement learning traffic control.
 
 ## Simulation Examples
 
 ### Large-scale scenario
 
 Belows are simulation result where approximately 60000 vehicles pass through a 10km x 10km grid network in 2 hours. The computation time was about 30 seconds on a standard desktop PC.
@@ -50,14 +76,18 @@
 [Jupyter Notebook of this example](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_03en_pytorch.ipynb) is available.
 
 <p float="left">
 <img src="https://github.com/toruseo/UXsim/blob/images/anim_network1_0.22_nocontrol.gif" width="400"/>
 <img src="https://github.com/toruseo/UXsim/blob/images/anim_network1_0.22_DQL.gif" width="400"/>
 </p>
 
+### Interactive GUI for exploring a simulation result
+
+https://github.com/toruseo/UXsim/assets/34780089/ec780a33-d9ba-4068-a005-0b06127196d9
+
 ## Install
 
 ### Using pip
 
 The simplest way is using pip to install from PyPI.
 
 ```
@@ -84,18 +114,16 @@
 	
 ### Manual install
 
 Download the `uxsim` directory from this Github repo or [the latest release](https://github.com/toruseo/UXsim/releases/latest/download/uxsim.zip) and place it to your local directory as follows:
 ```
 your_project_directory/
 ├── uxsim/ 	# The uxsim directory
-│ ├── utils/ 	# Utility files of UXsim
 │ ├── uxsim.py 	# The main code of UXsim. You can customize this as you wish
-│ ├── utils.py 	# Utility funcsions of UXsim
-│ └── ... 	# Other files in uxsim
+│ └── ... 	# Other files and directories in uxsim
 ├── your_simulation_code.py 		# Your code if nessesary
 ├── your_simulation_notebook.ipynb 	# Your Jupyter notebook if nessesary
 ├── ... 	# Other files if nessesary
 ```
 In this way, you can flexibly customize UXsim by your own.
 
 </details>
@@ -127,69 +155,74 @@
 )
 
 # Define the scenario
 W.addNode("orig1", 0, 0) # Create a node
 W.addNode("orig2", 0, 2)
 W.addNode("merge", 1, 1)
 W.addNode("dest", 2, 1)
-W.addLink("link1", "orig1", "merge", length=1000, free_flow_speed=20, jam_density=0.2, merge_priority=0.5) # Create a link
-W.addLink("link2", "orig2", "merge", length=1000, free_flow_speed=20, jam_density=0.2, merge_priority=2)
-W.addLink("link3", "merge", "dest", length=1000, free_flow_speed=20, jam_density=0.2)
-W.adddemand("orig1", "dest", 0, 1000, 0.4) # Create OD traffic demand
-W.adddemand("orig2", "dest", 500, 1000, 0.6)
+W.addLink("link1", "orig1", "merge", length=1000, free_flow_speed=20) # Create a link
+W.addLink("link2", "orig2", "merge", length=1000, free_flow_speed=20)
+W.addLink("link3", "merge", "dest", length=1000, free_flow_speed=20)
+W.adddemand("orig1", "dest", 0, 1000, 0.45) # Create OD traffic demand
+W.adddemand("orig2", "dest", 400, 1000, 0.6)
 
 # Run the simulation to the end
 W.exec_simulation()
 
 # Print summary of simulation result
 W.analyzer.print_simple_stats()
 
 # Visualize snapshots of network traffic state for several timesteps
-W.analyzer.network(0, detailed=1, network_font_size=0)
-W.analyzer.network(500, detailed=1, network_font_size=0)
-W.analyzer.network(1000, detailed=1, network_font_size=0)
+W.analyzer.network(100, detailed=1, network_font_size=12)
+W.analyzer.network(600, detailed=1, network_font_size=12)
+W.analyzer.network(800, detailed=1, network_font_size=12)
 ```
 
 It would output text to the terminal and images to `out` directory like below:
 ```
 simulation setting:
  scenario name:
  simulation duration:    1200 s
- number of vehicles:     700 veh
+ number of vehicles:     810 veh
  total road length:      3000 m
  time discret. width:    5 s
  platoon size:           5 veh
  number of timesteps:    240
- number of platoons:     140
+ number of platoons:     162
  number of links:        3
  number of nodes:        4
  setup time:             0.00 s
 simulating...
       time| # of vehicles| ave speed| computation time
        0 s|        0 vehs|   0.0 m/s|     0.00 s
-     600 s|      100 vehs|  17.5 m/s|     0.03 s
-    1195 s|       25 vehs|  20.0 m/s|     0.05 s
+     600 s|      130 vehs|  13.7 m/s|     0.03 s
+    1195 s|       75 vehs|  12.3 m/s|     0.06 s
  simulation finished
 results:
- average speed:  13.8 m/s
- number of completed trips:      675 / 700
- average travel time of trips:   142.7 s
- average delay of trips:         42.7 s
- delay ratio:                    0.299
+ average speed:  11.6 m/s
+ number of completed trips:      735 / 810
+ average travel time of trips:   162.6 s
+ average delay of trips:         62.6 s
+ delay ratio:                    0.385
 ```
 <p float="left">
-<img src="https://github.com/toruseo/UXsim/blob/images/simple_example_network1_1000.png" width="400"/>
+<img src="https://github.com/toruseo/UXsim/blob/images/network1_100.png" width="250"/>
+<img src="https://github.com/toruseo/UXsim/blob/images/network1_600.png" width="250"/>
+<img src="https://github.com/toruseo/UXsim/blob/images/network1_800.png" width="250"/>
 </p>
 
 ## Main Files
 
 - `uxsim` directory: UXsim main package
 	- `uxsim/uxsim.py`: UXsim main code
+	- `uxsim/analyzer.py`: Simulation result analysis code
 	- `uxsim/utils.py`: UXsim utilities code
- 	- `uxsim/utils` directory:  UXsim utilities files
+	- `uxsim/ResultGUIViewer/ResultGUIViewer.py`: Submodule on GUI for visualizing simulation results
+	- `uxsim/OSMImporter/OSMImporter.py`: Submodule on road network import from OpenStreetMap (experimental)
+ 	- `uxsim/files` directory: UXsim utilities files
 - `demos_and_examples` directory: Tutorials and examples of UXsim
 - `dat` directory: Sample scenario files
 - `tests`, `.github` directories: Development-related files
 
 ## Further Reading
 
 If you want to know the details of UXsim, please see
@@ -211,27 +244,27 @@
 ## Contributing and Discussion
 
 Contribution is welcome!
 For minor changes including bug fixes, please submit a pull request.
 Please make sure that your codes pass the automatic tests in Github Action.
 If you want a major change, please start a discussion at [Issues](https://github.com/toruseo/UXsim/issues) page first.
 
-If you have any questions or suggestions, please start a discussion at [Issues](https://github.com/toruseo/UXsim/issues) page (in English or Japanese).
+If you have any questions or suggestions, please start a discussion at [Discussions](https://github.com/toruseo/UXsim/discussions) page (in English or Japanese).
 
 I (Toru Seo) work on this project in my spare time. Please understand that my response may be delayed.
 
 ## Acknowledgments
 
 UXsim is based on various works in traffic flow theory and related fields. We would like to acknowledge the contributions of the research community in advancing this field.
 Especially, UXsim directly uses the following works:
 
 - [Newell's simplified car-following model](https://doi.org/10.1016/S0191-2615(00)00044-8) and its extention [X-model](https://doi.org/10.1016/j.trb.2013.02.008)
 - [Incremental Node Model](https://doi.org/10.1016/j.trb.2011.04.001) and its [mesoscopic version](https://ubiquitypress.com/site/chapters/e/10.5334/baw.50/)
 - [Dynamic User Optimum](https://doi.org/10.1016/S0191-2615(00)00005-9)-type Route Choice Model
 
 ## Related Links
 
-- [Toru Seo (Author)](https://toruseo.jp/)
+- [Toru Seo (Author)](https://toruseo.jp/index_en.html)
 - [Collection of related simulators by Seo](https://toruseo.jp/uxsim/index_en.html)
 - Japanese book "[Macroscopic Traffic Simulation: Fundamental Mathematical Theory and Python Implementation](https://www.coronasha.co.jp/np/isbn/9784339052794/)" (Author: [Toru Seo](https://toruseo.jp/), Publisher: [Corona Publishing Co., Ltd.](https://www.coronasha.co.jp/)): UXsim is a significant expansion of the traffic flow simulator *UroborosX* described in this book.
-- [Seo Laboratory, Tokyo Institute of Technology](http://seo.cv.ens.titech.ac.jp/)
+- [Seo Laboratory, Tokyo Institute of Technology](http://seo.cv.ens.titech.ac.jp/en/)
 - [Interactive Traffic Flow Simulator that Runs on a Web Browser](http://seo.cv.ens.titech.ac.jp/traffic-flow-demo/bottleneck.html): Play with the same link traffic flow model used in this simulator interactively, and learn the basics of traffic flow and its simulation.
```

### Comparing `uxsim-1.0.9/pyproject.toml` & `uxsim-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uxsim-1.0.9/tests/test_examples.py` & `uxsim-1.1.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.0.9/tests/test_result_gui_viewer.py` & `uxsim-1.1.0/tests/test_result_gui_viewer.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.0.9/tests/test_verification_exceptional.py` & `uxsim-1.1.0/tests/test_verification_exceptional.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.0.9/tests/test_verification_node.py` & `uxsim-1.1.0/tests/test_verification_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 import pandas as pd
 
 def equal_tolerance(val, check, rel_tol=0.1, abs_tol=0.0):
     if check == 0 and abs_tol == 0:
         abs_tol = 0.1
     return abs(val - check) <= abs(check*rel_tol) + abs_tol
 
+def q2k_cong(q, link):
+    return -(q-link.kappa*link.w)/link.w
+
 @pytest.mark.flaky(reruns=5)
 def test_merge_fair_nocongestion():
     tt1s = []
     tt2s = []
     tt3s = []
     vol1s = []
     vol2s = []
@@ -543,14 +546,67 @@
     print(f"{q1 = }\n{q2 = }\n{q3 = }\n{v2 = }")
 
     assert equal_tolerance(q1, 0.2)
     assert equal_tolerance(q2, 0.6)
     assert equal_tolerance(q3, 0.8)
     assert equal_tolerance(v2, 20, rel_tol=0.2)
 
+
+@pytest.mark.flaky(reruns=5)
+def test_diverge_flowcheck():
+    q1s = []
+    k1s = []
+    v1s = []
+    q2s = []
+    k2s = []
+    q3s = []
+    k3s = []
+    for i in range(5):
+        W = World(
+            name="",
+            deltan=5,
+            tmax=1000,
+            print_mode=0, save_mode=0, show_mode=1,
+            random_seed=None
+        )
+
+        W.addNode("orig", 0, 0)
+        W.addNode("mid", 0, 0)
+        W.addNode("dest1", 2, 1)
+        W.addNode("dest2", 2, 1)
+        link1 = W.addLink("link1", "orig", "mid", length=1000, free_flow_speed=20, jam_density=0.2,   number_of_lanes=1)
+        link2 = W.addLink("link2", "mid", "dest1", length=1000, free_flow_speed=20, jam_density=0.2,  number_of_lanes=1, capacity_in=0.4)
+        link3 = W.addLink("link3", "mid", "dest2",  length=1000, free_flow_speed=20, jam_density=0.2, number_of_lanes=1, capacity_in=0.4)
+        t1 = 1000
+        flow1 = 0.8*2/3
+        t2 = 1000
+        flow2 = 0.8*1/3
+        W.adddemand("orig", "dest1", 0, t1, flow1)
+        W.adddemand("orig", "dest2", 0, t2, flow2)
+
+        W.exec_simulation()
+        W.analyzer.print_simple_stats()
+
+        W.analyzer.compute_edie_state()
+        q1s.append(link1.q_mat[5:,6:8].mean())
+        k1s.append(link1.k_mat[5:,6:8].mean())
+        v1s.append(link1.v_mat[5:,6:8].mean())
+        q2s.append(link2.q_mat[5:,6:8].mean())
+        k2s.append(link2.k_mat[5:,6:8].mean())
+        q3s.append(link3.q_mat[5:,6:8].mean())
+        k3s.append(link3.k_mat[5:,6:8].mean())
+
+    print(np.average(q1s), 0.6) 
+    print(np.average(k1s), q2k_cong(0.6, link1))
+    print(np.average(v1s), 0.6/q2k_cong(0.6, link1))
+    print(np.average(q2s), 0.4)
+    print(np.average(k2s), 0.02)
+    print(np.average(q3s), 0.2) 
+    print(np.average(k3s), 0.01)
+
 @pytest.mark.flaky(reruns=5)
 def test_2to2_no_flow_to_one_dest():
     tt1s = []
     tt2s = []
     tt3s = []
     tt4s = []
     vol1s = []
@@ -992,9 +1048,7 @@
     # avt = df_mean["average_travel_time"].values
 
     avt = df["average_travel_time"].values
     print(avt)
     referemce_avt = [41.40449658, 65.77142857, 41.56507937, 41.41644018, 41.30793651, 65.97619048, 49.7849498, 49.15555556, 69.54444444, 49.11051701, 70.71428571, 48.62857143]
     for i in range(len(avt)):
         assert equal_tolerance(avt[i], referemce_avt[i])
-                                                     
-#TODO: add tests later, check flow values
```

### Comparing `uxsim-1.0.9/tests/test_verification_route_choice.py` & `uxsim-1.1.0/tests/test_verification_route_choice.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,17 +461,16 @@
     print(f"{np.average(vol1_es) = }\n{np.average(vol1_ls) = }\n{np.average(vol2_es) = }\n{np.average(vol2_ls) = }")
     assert equal_tolerance(np.average(vol1_es), 340, abs_tol=100)
     assert equal_tolerance(np.average(vol1_ls), 0)
     assert equal_tolerance(np.average(vol2_es), 0, abs_tol=100)
     assert equal_tolerance(np.average(vol2_ls), 750)
 
 
-
 @pytest.mark.flaky(reruns=5)
-def test_4route_congestion_avoidance():
+def test_route_choice_4route_congestion_avoidance():
     tt1s = []
     tt2s = []
     tt3s = []
     tt4s = []
     vol1s = []
     vol2s = []
     vol3s = []
```

### Comparing `uxsim-1.0.9/tests/test_verification_sioux_falls.py` & `uxsim-1.1.0/tests/test_verification_sioux_falls.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.0.9/tests/test_verification_straight_road.py` & `uxsim-1.1.0/tests/test_verification_straight_road.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.0.9/uxsim/OSMImporter/OSMImporter.py` & `uxsim-1.1.0/uxsim/OSMImporter/OSMImporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+"""
+OpenStreetMap importer using OSMnx.
+Work in progress. Import from OSM is experimental and may not work as expected. It is functional but may produce inappropriate networks for simulation, such as too many nodes, too many deadends, fragmented networks.
+
+
+Examples
+--------
+Import highway in Tokyo:
+    >>> from uxsim.OSMImporter import OSMImporter
+    >>> ... #define World object W
+    >>> nodes, links = OSMImporter.import_osm_data(north=35.817, south=35.570, east=139.881, west=139.583, custom_filter='["highway"~"motorway"]')
+    >>> nodes, links = OSMImporter.osm_network_postprocessing(nodes, links, node_merge_threshold=0.005, node_merge_iteration=5, >>> enforce_bidirectional=True)  # merge threshold distance: 0.005 degree ~= 500 m. `enforce_bidirectional` makes all links bidirectional, so >>> that network is not fragmented (but the original network topology is not preserved rigorously).
+    >>> OSMImporter.osm_network_visualize(nodes, links, show_link_name=0)
+    >>> OSMImporter.osm_network_to_World(W, nodes, links, default_jam_density=0.2, coef_degree_to_meter=111000)
+    >>> ... #add demand
+    >>> W.exec_simulation()
+"""
+
 
 import matplotlib.pyplot as plt
 import math
 import warnings
 
 class OSMImporter:
     """
@@ -100,14 +118,16 @@
                             lanes = default_number_of_lanes_residential
                         elif "tertiary" in road_type:
                             lanes = default_number_of_lanes_tertiary
                         else:
                             lanes = default_number_of_lanes_others
                     except:
                         lanes = default_number_of_lanes_others
+                    if lanes < 1:
+                        lanes = 1
                 try:
                     maxspeed = float(ed["maxspeed"])/3.6
                 except:
                     try:
                         if "mortorway" in road_type:
                             maxspeed = default_maxspeed_mortorway/3.6
                         elif "trunk" in road_type:
@@ -123,14 +143,15 @@
                         else:
                             maxspeed = default_maxspeed_others/3.6
                     except:
                         maxspeed = default_maxspeed_others/3.6
             
 
                 links.append([name, e[0], e[1], lanes, maxspeed]) # name, from, to, number_of_lanes, maxspeed
+                #links.append([name, e[0], e[1], 1, maxspeed]) # name, from, to, number_of_lanes, maxspeed
                 nodes[e[0]] = node_dict[e[0]]
                 nodes[e[1]] = node_dict[e[1]]
 
         nodes = list(nodes.values())
         
         print("imported network size:")
         print(" number of links:", len(links))
@@ -314,8 +335,8 @@
             if nname in [n.name for n in W.NODES]:
                 nname + f"_osm{i}"
             W.addNode(str(node[0]), x=node[1], y=node[2], auto_rename=True)
         for i, link in enumerate(links):
             lname = str(link[0])
             if lname in [l.name for l in W.LINKS]:
                 lname + f"_osm{i}"
-            W.addLink(lname, str(link[1]), str(link[2]), length=link[5]*coef_degree_to_meter, free_flow_speed=link[4], jam_density=default_jam_density, auto_rename=True)
+            W.addLink(lname, str(link[1]), str(link[2]), length=link[5]*coef_degree_to_meter, free_flow_speed=link[4], jam_density_per_lane=default_jam_density, number_of_lanes=link[3], auto_rename=True)
```

### Comparing `uxsim-1.0.9/uxsim/ResultGUIViewer/ResultGUIViewer.py` & `uxsim-1.1.0/uxsim/ResultGUIViewer/ResultGUIViewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 """
 Interactive viewer for UXsim simulation results using PyQt5.
+After running the simulation, you can launch this viewer to visualize the simulation results interactively.
 GUI part was mainly written by Claude 3 Opus under supervision of Toru Seo.
+
+Examples
+--------
+Usage:
+    >>> ... #define the World object W
+    >>> W.exec_simulation()     #you run the simulation.
+    >>> from uxsim.ResultGUIViewer import launch_World_viewer
+    >>> launch_World_viewer(W)
 """
 
 import sys
 import numpy as np
 from matplotlib import colormaps
 from PyQt5.QtWidgets import QApplication, QMainWindow, QGraphicsView, QGraphicsScene, QGraphicsItem, QMenu, QSlider, QVBoxLayout, QWidget, QHBoxLayout, QLabel, QPushButton
 from PyQt5.QtGui import QPen, QColor, QPainter, QPainterPath
```

### Comparing `uxsim-1.0.9/uxsim/files/Inconsolata.otf` & `uxsim-1.1.0/uxsim/files/Inconsolata.otf`

 * *Files identical despite different names*

### Comparing `uxsim-1.0.9/uxsim/files/Licence_of_Inconsolata.otf.txt` & `uxsim-1.1.0/uxsim/files/Licence_of_Inconsolata.otf.txt`

 * *Files identical despite different names*

### Comparing `uxsim-1.0.9/uxsim/utils.py` & `uxsim-1.1.0/uxsim/utils.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.0.9/uxsim.egg-info/PKG-INFO` & `uxsim-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: uxsim
-Version: 1.0.9
-Summary: UXsim: traffic flow simulator
-Author-email: Toru Seo <seo.t.aa@m.titech.ac.jp>
-License: MIT License
-Project-URL: Homepage, https://github.com/toruseo/UXsim
-Project-URL: Download, https://github.com/toruseo/UXsim
-Project-URL: Bug Tracker, https://github.com/toruseo/UXsim/issues
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.21.5
-Requires-Dist: matplotlib>=3.5.2
-Requires-Dist: pillow>=9.2.0
-Requires-Dist: tqdm>=4.64.1
-Requires-Dist: scipy>=1.9.1
-Requires-Dist: pandas>=1.4.4
-Requires-Dist: PyQt5>=5.15.7
-
 # UXsim: Network traffic flow simulator in pure Python
 
 [![PyPi](https://img.shields.io/pypi/v/uxsim.svg)](https://pypi.python.org/pypi/uxsim)
 [![](https://tokei.rs/b1/github/toruseo/UXsim?style=flat&category=code&color=dddd22)](https://github.com/toruseo/UXsim)
 [![](https://tokei.rs/b1/github/toruseo/UXsim?category=comments&style=flat&color=44cc44)](https://github.com/toruseo/UXsim/)
 [![Demo in Colab](https://colab.research.google.com/assets/colab-badge.svg)](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb)
 [![arXiv](https://img.shields.io/badge/arXiv-2309.17114-b31b1b.svg)](http://dx.doi.org/10.48550/arXiv.2309.17114)
@@ -42,18 +17,19 @@
 
 - [Jupyter Notebook](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_01en.ipynb) or [Google Colab](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb): Interactive demonstrations and tutorials
 - [Technical Documentation](https://toruseo.jp/UXsim/docs/index.html): Detailed documents on tutorials, simulation mechanism, and specifications of modules/functions
 
 ## Main Features
 
 - Simple, lightweight, and easy-to-use Python implementation of the modern standard models of dynamic network traffic flow.
-- Traffic flow simulation with a given network and time-dependent OD demand (dynamic traffic assignment).
+- Macroscopic traffic simulation: Simulating over 60000 vehicles in 30 seconds in a city.
+- Dynamic traffic assignment: Traffic flow simulation with a given network and time-dependent OD demand.
 - Implementation of traffic control/management schemes such as traffic signals and road pricing.
 - Basic analysis of simulation results and their export to pandas.DataFrame and CSV files.
-- Visualization of simulation results including animation.
+- Visualization of simulation results using matplotlib. Interactive GUI is available.
 - Flexible and customizable thanks to pure Python implementation. Can also be directly integrated with other Python-based frameworks, such as PyTorch for deep reinforcement learning traffic control.
 
 ## Simulation Examples
 
 ### Large-scale scenario
 
 Belows are simulation result where approximately 60000 vehicles pass through a 10km x 10km grid network in 2 hours. The computation time was about 30 seconds on a standard desktop PC.
@@ -75,14 +51,18 @@
 [Jupyter Notebook of this example](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_03en_pytorch.ipynb) is available.
 
 <p float="left">
 <img src="https://github.com/toruseo/UXsim/blob/images/anim_network1_0.22_nocontrol.gif" width="400"/>
 <img src="https://github.com/toruseo/UXsim/blob/images/anim_network1_0.22_DQL.gif" width="400"/>
 </p>
 
+### Interactive GUI for exploring a simulation result
+
+https://github.com/toruseo/UXsim/assets/34780089/ec780a33-d9ba-4068-a005-0b06127196d9
+
 ## Install
 
 ### Using pip
 
 The simplest way is using pip to install from PyPI.
 
 ```
@@ -109,18 +89,16 @@
 	
 ### Manual install
 
 Download the `uxsim` directory from this Github repo or [the latest release](https://github.com/toruseo/UXsim/releases/latest/download/uxsim.zip) and place it to your local directory as follows:
 ```
 your_project_directory/
 ├── uxsim/ 	# The uxsim directory
-│ ├── utils/ 	# Utility files of UXsim
 │ ├── uxsim.py 	# The main code of UXsim. You can customize this as you wish
-│ ├── utils.py 	# Utility funcsions of UXsim
-│ └── ... 	# Other files in uxsim
+│ └── ... 	# Other files and directories in uxsim
 ├── your_simulation_code.py 		# Your code if nessesary
 ├── your_simulation_notebook.ipynb 	# Your Jupyter notebook if nessesary
 ├── ... 	# Other files if nessesary
 ```
 In this way, you can flexibly customize UXsim by your own.
 
 </details>
@@ -152,69 +130,74 @@
 )
 
 # Define the scenario
 W.addNode("orig1", 0, 0) # Create a node
 W.addNode("orig2", 0, 2)
 W.addNode("merge", 1, 1)
 W.addNode("dest", 2, 1)
-W.addLink("link1", "orig1", "merge", length=1000, free_flow_speed=20, jam_density=0.2, merge_priority=0.5) # Create a link
-W.addLink("link2", "orig2", "merge", length=1000, free_flow_speed=20, jam_density=0.2, merge_priority=2)
-W.addLink("link3", "merge", "dest", length=1000, free_flow_speed=20, jam_density=0.2)
-W.adddemand("orig1", "dest", 0, 1000, 0.4) # Create OD traffic demand
-W.adddemand("orig2", "dest", 500, 1000, 0.6)
+W.addLink("link1", "orig1", "merge", length=1000, free_flow_speed=20) # Create a link
+W.addLink("link2", "orig2", "merge", length=1000, free_flow_speed=20)
+W.addLink("link3", "merge", "dest", length=1000, free_flow_speed=20)
+W.adddemand("orig1", "dest", 0, 1000, 0.45) # Create OD traffic demand
+W.adddemand("orig2", "dest", 400, 1000, 0.6)
 
 # Run the simulation to the end
 W.exec_simulation()
 
 # Print summary of simulation result
 W.analyzer.print_simple_stats()
 
 # Visualize snapshots of network traffic state for several timesteps
-W.analyzer.network(0, detailed=1, network_font_size=0)
-W.analyzer.network(500, detailed=1, network_font_size=0)
-W.analyzer.network(1000, detailed=1, network_font_size=0)
+W.analyzer.network(100, detailed=1, network_font_size=12)
+W.analyzer.network(600, detailed=1, network_font_size=12)
+W.analyzer.network(800, detailed=1, network_font_size=12)
 ```
 
 It would output text to the terminal and images to `out` directory like below:
 ```
 simulation setting:
  scenario name:
  simulation duration:    1200 s
- number of vehicles:     700 veh
+ number of vehicles:     810 veh
  total road length:      3000 m
  time discret. width:    5 s
  platoon size:           5 veh
  number of timesteps:    240
- number of platoons:     140
+ number of platoons:     162
  number of links:        3
  number of nodes:        4
  setup time:             0.00 s
 simulating...
       time| # of vehicles| ave speed| computation time
        0 s|        0 vehs|   0.0 m/s|     0.00 s
-     600 s|      100 vehs|  17.5 m/s|     0.03 s
-    1195 s|       25 vehs|  20.0 m/s|     0.05 s
+     600 s|      130 vehs|  13.7 m/s|     0.03 s
+    1195 s|       75 vehs|  12.3 m/s|     0.06 s
  simulation finished
 results:
- average speed:  13.8 m/s
- number of completed trips:      675 / 700
- average travel time of trips:   142.7 s
- average delay of trips:         42.7 s
- delay ratio:                    0.299
+ average speed:  11.6 m/s
+ number of completed trips:      735 / 810
+ average travel time of trips:   162.6 s
+ average delay of trips:         62.6 s
+ delay ratio:                    0.385
 ```
 <p float="left">
-<img src="https://github.com/toruseo/UXsim/blob/images/simple_example_network1_1000.png" width="400"/>
+<img src="https://github.com/toruseo/UXsim/blob/images/network1_100.png" width="250"/>
+<img src="https://github.com/toruseo/UXsim/blob/images/network1_600.png" width="250"/>
+<img src="https://github.com/toruseo/UXsim/blob/images/network1_800.png" width="250"/>
 </p>
 
 ## Main Files
 
 - `uxsim` directory: UXsim main package
 	- `uxsim/uxsim.py`: UXsim main code
+	- `uxsim/analyzer.py`: Simulation result analysis code
 	- `uxsim/utils.py`: UXsim utilities code
- 	- `uxsim/utils` directory:  UXsim utilities files
+	- `uxsim/ResultGUIViewer/ResultGUIViewer.py`: Submodule on GUI for visualizing simulation results
+	- `uxsim/OSMImporter/OSMImporter.py`: Submodule on road network import from OpenStreetMap (experimental)
+ 	- `uxsim/files` directory: UXsim utilities files
 - `demos_and_examples` directory: Tutorials and examples of UXsim
 - `dat` directory: Sample scenario files
 - `tests`, `.github` directories: Development-related files
 
 ## Further Reading
 
 If you want to know the details of UXsim, please see
@@ -236,27 +219,27 @@
 ## Contributing and Discussion
 
 Contribution is welcome!
 For minor changes including bug fixes, please submit a pull request.
 Please make sure that your codes pass the automatic tests in Github Action.
 If you want a major change, please start a discussion at [Issues](https://github.com/toruseo/UXsim/issues) page first.
 
-If you have any questions or suggestions, please start a discussion at [Issues](https://github.com/toruseo/UXsim/issues) page (in English or Japanese).
+If you have any questions or suggestions, please start a discussion at [Discussions](https://github.com/toruseo/UXsim/discussions) page (in English or Japanese).
 
 I (Toru Seo) work on this project in my spare time. Please understand that my response may be delayed.
 
 ## Acknowledgments
 
 UXsim is based on various works in traffic flow theory and related fields. We would like to acknowledge the contributions of the research community in advancing this field.
 Especially, UXsim directly uses the following works:
 
 - [Newell's simplified car-following model](https://doi.org/10.1016/S0191-2615(00)00044-8) and its extention [X-model](https://doi.org/10.1016/j.trb.2013.02.008)
 - [Incremental Node Model](https://doi.org/10.1016/j.trb.2011.04.001) and its [mesoscopic version](https://ubiquitypress.com/site/chapters/e/10.5334/baw.50/)
 - [Dynamic User Optimum](https://doi.org/10.1016/S0191-2615(00)00005-9)-type Route Choice Model
 
 ## Related Links
 
-- [Toru Seo (Author)](https://toruseo.jp/)
+- [Toru Seo (Author)](https://toruseo.jp/index_en.html)
 - [Collection of related simulators by Seo](https://toruseo.jp/uxsim/index_en.html)
 - Japanese book "[Macroscopic Traffic Simulation: Fundamental Mathematical Theory and Python Implementation](https://www.coronasha.co.jp/np/isbn/9784339052794/)" (Author: [Toru Seo](https://toruseo.jp/), Publisher: [Corona Publishing Co., Ltd.](https://www.coronasha.co.jp/)): UXsim is a significant expansion of the traffic flow simulator *UroborosX* described in this book.
-- [Seo Laboratory, Tokyo Institute of Technology](http://seo.cv.ens.titech.ac.jp/)
+- [Seo Laboratory, Tokyo Institute of Technology](http://seo.cv.ens.titech.ac.jp/en/)
 - [Interactive Traffic Flow Simulator that Runs on a Web Browser](http://seo.cv.ens.titech.ac.jp/traffic-flow-demo/bottleneck.html): Play with the same link traffic flow model used in this simulator interactively, and learn the basics of traffic flow and its simulation.
```

### Comparing `uxsim-1.0.9/uxsim.egg-info/SOURCES.txt` & `uxsim-1.1.0/uxsim.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 tests/test_examples.py
 tests/test_result_gui_viewer.py
 tests/test_verification_exceptional.py
+tests/test_verification_multilane.py
 tests/test_verification_node.py
 tests/test_verification_route_choice.py
 tests/test_verification_sioux_falls.py
 tests/test_verification_straight_road.py
 uxsim/__init__.py
+uxsim/analyzer.py
 uxsim/utils.py
 uxsim/uxsim.py
 uxsim.egg-info/PKG-INFO
 uxsim.egg-info/SOURCES.txt
 uxsim.egg-info/dependency_links.txt
 uxsim.egg-info/requires.txt
 uxsim.egg-info/top_level.txt
 uxsim/OSMImporter/OSMImporter.py
 uxsim/OSMImporter/__init__.py
 uxsim/ResultGUIViewer/ResultGUIViewer.py
 uxsim/ResultGUIViewer/__init__.py
+uxsim/files/HackGen-Regular.ttf
 uxsim/files/Inconsolata.otf
+uxsim/files/LICENSE_of_HackGen-Regular
 uxsim/files/Licence_of_Inconsolata.otf.txt
 uxsim/files/README.md
 uxsim/files/__init__.py
```

