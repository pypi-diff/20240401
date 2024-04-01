# Comparing `tmp/NxTransit-0.1.20.dev0.tar.gz` & `tmp/NxTransit-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NxTransit-0.1.20.dev0.tar", last modified: Thu Mar 21 22:05:56 2024, max compression
+gzip compressed data, was "NxTransit-0.1.21.tar", last modified: Mon Apr  1 15:15:17 2024, max compression
```

## Comparing `NxTransit-0.1.20.dev0.tar` & `NxTransit-0.1.21.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 22:05:56.746844 NxTransit-0.1.20.dev0/
--rw-rw-rw-   0        0        0     1101 2024-02-20 06:07:02.000000 NxTransit-0.1.20.dev0/LICENSE
-drwxrwxrwx   0        0        0        0 2024-03-21 22:05:56.743842 NxTransit-0.1.20.dev0/NxTransit.egg-info/
--rw-rw-rw-   0        0        0     3276 2024-03-21 22:05:56.000000 NxTransit-0.1.20.dev0/NxTransit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2024-03-21 22:05:56.000000 NxTransit-0.1.20.dev0/NxTransit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 22:05:56.000000 NxTransit-0.1.20.dev0/NxTransit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2024-03-21 22:05:56.000000 NxTransit-0.1.20.dev0/NxTransit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-21 22:05:56.000000 NxTransit-0.1.20.dev0/NxTransit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3276 2024-03-21 22:05:56.744841 NxTransit-0.1.20.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     2032 2024-03-11 22:00:04.000000 NxTransit-0.1.20.dev0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 22:05:56.736847 NxTransit-0.1.20.dev0/nxtransit/
--rw-rw-rw-   0        0        0     1947 2024-03-21 22:02:07.000000 NxTransit-0.1.20.dev0/nxtransit/__init__.py
--rw-rw-rw-   0        0        0    14866 2024-03-21 21:51:59.000000 NxTransit-0.1.20.dev0/nxtransit/accessibility.py
--rw-rw-rw-   0        0        0     5807 2024-03-15 20:39:27.000000 NxTransit-0.1.20.dev0/nxtransit/connectors.py
--rw-rw-rw-   0        0        0     1163 2024-03-17 13:00:56.000000 NxTransit-0.1.20.dev0/nxtransit/converters.py
--rw-rw-rw-   0        0        0     7626 2024-03-19 14:18:38.000000 NxTransit-0.1.20.dev0/nxtransit/frequency.py
--rw-rw-rw-   0        0        0    10837 2024-03-19 13:59:18.000000 NxTransit-0.1.20.dev0/nxtransit/functions.py
--rw-rw-rw-   0        0        0    17944 2024-03-19 14:20:27.000000 NxTransit-0.1.20.dev0/nxtransit/loaders.py
--rw-rw-rw-   0        0        0     2700 2024-03-11 20:56:23.000000 NxTransit-0.1.20.dev0/nxtransit/other.py
--rw-rw-rw-   0        0        0     5977 2024-02-25 22:09:23.000000 NxTransit-0.1.20.dev0/nxtransit/prism.py
--rw-rw-rw-   0        0        0    14351 2024-03-20 15:33:58.000000 NxTransit-0.1.20.dev0/nxtransit/routers.py
--rw-rw-rw-   0        0        0     1440 2024-03-21 22:00:02.000000 NxTransit-0.1.20.dev0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-21 22:05:56.746844 NxTransit-0.1.20.dev0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-21 22:05:56.740852 NxTransit-0.1.20.dev0/tests/
--rw-rw-rw-   0        0        0     1316 2024-02-24 22:43:44.000000 NxTransit-0.1.20.dev0/tests/test_functions.py
--rw-rw-rw-   0        0        0     2823 2024-03-20 15:12:08.000000 NxTransit-0.1.20.dev0/tests/test_routers.py
+drwxrwxrwx   0        0        0        0 2024-04-01 15:15:17.652983 NxTransit-0.1.21/
+-rw-rw-rw-   0        0        0     1101 2024-02-20 06:07:02.000000 NxTransit-0.1.21/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-01 15:15:17.643965 NxTransit-0.1.21/NxTransit.egg-info/
+-rw-rw-rw-   0        0        0     3290 2024-04-01 15:15:17.000000 NxTransit-0.1.21/NxTransit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2024-04-01 15:15:17.000000 NxTransit-0.1.21/NxTransit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 15:15:17.000000 NxTransit-0.1.21/NxTransit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      156 2024-04-01 15:15:17.000000 NxTransit-0.1.21/NxTransit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-01 15:15:17.000000 NxTransit-0.1.21/NxTransit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3290 2024-04-01 15:15:17.646972 NxTransit-0.1.21/PKG-INFO
+-rw-rw-rw-   0        0        0     2032 2024-03-26 18:30:04.000000 NxTransit-0.1.21/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 15:15:17.638964 NxTransit-0.1.21/nxtransit/
+-rw-rw-rw-   0        0        0     1991 2024-04-01 15:10:34.000000 NxTransit-0.1.21/nxtransit/__init__.py
+-rw-rw-rw-   0        0        0    15200 2024-04-01 13:47:17.000000 NxTransit-0.1.21/nxtransit/accessibility.py
+-rw-rw-rw-   0        0        0     5868 2024-03-25 19:57:15.000000 NxTransit-0.1.21/nxtransit/connectors.py
+-rw-rw-rw-   0        0        0     1156 2024-03-25 12:26:14.000000 NxTransit-0.1.21/nxtransit/converters.py
+-rw-rw-rw-   0        0        0     7555 2024-03-29 17:16:04.000000 NxTransit-0.1.21/nxtransit/frequency.py
+-rw-rw-rw-   0        0        0    13028 2024-03-29 17:42:08.000000 NxTransit-0.1.21/nxtransit/functions.py
+-rw-rw-rw-   0        0        0    17492 2024-03-29 21:20:45.000000 NxTransit-0.1.21/nxtransit/loaders.py
+-rw-rw-rw-   0        0        0      441 2024-03-29 20:28:51.000000 NxTransit-0.1.21/nxtransit/other.py
+-rw-rw-rw-   0        0        0     5977 2024-02-25 22:09:23.000000 NxTransit-0.1.21/nxtransit/prism.py
+-rw-rw-rw-   0        0        0    14318 2024-03-28 09:51:45.000000 NxTransit-0.1.21/nxtransit/routers.py
+-rw-rw-rw-   0        0        0     1462 2024-03-29 17:11:31.000000 NxTransit-0.1.21/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 15:15:17.652983 NxTransit-0.1.21/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 15:15:17.641969 NxTransit-0.1.21/tests/
+-rw-rw-rw-   0        0        0     2361 2024-03-29 17:46:46.000000 NxTransit-0.1.21/tests/test_functions.py
+-rw-rw-rw-   0        0        0     2823 2024-03-20 15:12:08.000000 NxTransit-0.1.21/tests/test_routers.py
```

### Comparing `NxTransit-0.1.20.dev0/LICENSE` & `NxTransit-0.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `NxTransit-0.1.20.dev0/NxTransit.egg-info/PKG-INFO` & `NxTransit-0.1.21/NxTransit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: NxTransit
-Version: 0.1.20.dev0
+Version: 0.1.21
 Summary: Construct and analyze time-dependent transit networks from GTFS data
 Author: Chingiz Zhanarbaev
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
@@ -22,15 +23,14 @@
 Requires-Dist: networkx>=3.2.0
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: osmnx>=1.9.1
 Requires-Dist: pandas>=2.2.0
 Requires-Dist: pytest>=8.0.1
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: Shapely>=2.0.3
-Requires-Dist: tqdm>=4.66.1
 Requires-Dist: geocube>=0.5.0
 Provides-Extra: tests
 Requires-Dist: pytest>=8.0.1; extra == "tests"
 
 # NxTransit
 
 [![tests](https://github.com/chingiztob/NxTransit/actions/workflows/basic_tests.yml/badge.svg?event=push)](https://github.com/chingiztob/NxTransit/actions/workflows/basic_tests.yml)
@@ -57,11 +57,11 @@
 - More features are planned for future updates.
 
 ### GTFS Data Support
 NxTransit utilizes GTFS data, a common format for public transportation schedules and geographic information.
 
 ### Installation
 ```bash
-pip install NxTransit
+pip install nxtransit
 ```
 ### License
 Package is open source and licensed under the MIT license. OpenStreetMap's open data [license](https://www.openstreetmap.org/copyright/) requires that derivative works provide proper attribution. This package heavily depends on [OSMnx](https://geoffboeing.com/publications/osmnx-complex-street-networks/) by Geoff Boeing, which is also licensed under the MIT license.
```

### Comparing `NxTransit-0.1.20.dev0/PKG-INFO` & `NxTransit-0.1.21/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: NxTransit
-Version: 0.1.20.dev0
+Version: 0.1.21
 Summary: Construct and analyze time-dependent transit networks from GTFS data
 Author: Chingiz Zhanarbaev
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
@@ -22,15 +23,14 @@
 Requires-Dist: networkx>=3.2.0
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: osmnx>=1.9.1
 Requires-Dist: pandas>=2.2.0
 Requires-Dist: pytest>=8.0.1
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: Shapely>=2.0.3
-Requires-Dist: tqdm>=4.66.1
 Requires-Dist: geocube>=0.5.0
 Provides-Extra: tests
 Requires-Dist: pytest>=8.0.1; extra == "tests"
 
 # NxTransit
 
 [![tests](https://github.com/chingiztob/NxTransit/actions/workflows/basic_tests.yml/badge.svg?event=push)](https://github.com/chingiztob/NxTransit/actions/workflows/basic_tests.yml)
@@ -57,11 +57,11 @@
 - More features are planned for future updates.
 
 ### GTFS Data Support
 NxTransit utilizes GTFS data, a common format for public transportation schedules and geographic information.
 
 ### Installation
 ```bash
-pip install NxTransit
+pip install nxtransit
 ```
 ### License
 Package is open source and licensed under the MIT license. OpenStreetMap's open data [license](https://www.openstreetmap.org/copyright/) requires that derivative works provide proper attribution. This package heavily depends on [OSMnx](https://geoffboeing.com/publications/osmnx-complex-street-networks/) by Geoff Boeing, which is also licensed under the MIT license.
```

### Comparing `NxTransit-0.1.20.dev0/README.md` & `NxTransit-0.1.21/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,11 +24,11 @@
 - More features are planned for future updates.
 
 ### GTFS Data Support
 NxTransit utilizes GTFS data, a common format for public transportation schedules and geographic information.
 
 ### Installation
 ```bash
-pip install NxTransit
+pip install nxtransit
 ```
 ### License
 Package is open source and licensed under the MIT license. OpenStreetMap's open data [license](https://www.openstreetmap.org/copyright/) requires that derivative works provide proper attribution. This package heavily depends on [OSMnx](https://geoffboeing.com/publications/osmnx-complex-street-networks/) by Geoff Boeing, which is also licensed under the MIT license.
```

### Comparing `NxTransit-0.1.20.dev0/nxtransit/__init__.py` & `NxTransit-0.1.21/nxtransit/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 It uses General Transit Feed Specification (GTFS) data to construct the graph and perform various time-dependent calculations.
 
 Key Features:
 - Multimodal Graph Creation: NxTransit can generate a graph that integrates different modes of transportation with street network.
 - Time-Dependent Calculations: The package allows for the analysis of transit dynamics by considering the time-dependency of transit schedules. This includes calculating shortest paths with departure times, travel time matrices, and service frequency.
 - GTFS Data Support: NxTransit uses GTFS data, a common format for public transportation schedules and associated geographic information, as the basis for graph construction and analysis.
 """
-__version__ = "0.1.20.dev0"
+__version__ = "0.1.21"
 
 from .loaders import feed_to_graph
 from .loaders import load_stops_gdf
 
 from .routers import time_dependent_dijkstra
 from .routers import single_source_time_dependent_dijkstra
 
@@ -24,15 +24,16 @@
 from .accessibility import last_service
 
 from .frequency import edge_frequency
 from .frequency import node_frequency
 from .frequency import connectivity_frequency
 from .frequency import single_source_connectivity_frequency
 
-from .functions import create_grid
+from .functions import aggregate_to_grid
+from .functions import determine_utm_zone
 from .functions import create_centroids_dataframe
 from .functions import validate_feed
 from .functions import separate_travel_times
 from .functions import process_graph_to_hash_table
 
 from .converters import parse_seconds_to_time
 from .converters import parse_time_to_seconds
```

### Comparing `NxTransit-0.1.20.dev0/nxtransit/accessibility.py` & `NxTransit-0.1.21/nxtransit/accessibility.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """Tools for calculating accessibility metrics"""
+
 import multiprocessing
 import time
 from functools import partial
+from typing import Any, Dict, Optional
 
 import geopandas as gpd
 import pandas as pd
-import tqdm
 import xarray as xr
 from geocube.api.core import make_geocube
 from geocube.vector import vectorize
+from networkx import DiGraph
 from shapely.geometry import Point
 
+from .functions import determine_utm_zone
 from .routers import single_source_time_dependent_dijkstra
 
 
-def calculate_od_matrix(graph, nodes: list, departure_time: int,
-                        hashtable: dict = None, algorithm='sorted'
-                        ):
+def calculate_od_matrix(
+    graph, nodes: list, departure_time: int, hashtable: dict = None, algorithm="sorted"
+):
     """
     Calculates the Origin-Destination (OD) matrix for a given graph, nodes, and departure time.
 
     Parameters
     ----------
     graph : networkx.DiGraph
         The graph representing the transit network.
@@ -41,66 +44,74 @@
             - destination_node: The ID of the destination node.
             - arrival_time: The arrival time at the destination node in seconds since midnight.
             - travel_time: The travel time from the origin node to the destination node in seconds.
     """
 
     results = []
 
-    for source_node in tqdm.tqdm(nodes):
-        # Calculate arrival times and travel times 
+    for source_node in nodes:
+        # Calculate arrival times and travel times
         # for each node using the specified algorithm
         arrival_times, _, travel_times = single_source_time_dependent_dijkstra(
-            graph, source_node, departure_time,
-            hashtable, algorithm=algorithm
-            )
+            graph, source_node, departure_time, hashtable, algorithm=algorithm
+        )
 
-        # Iterate through all nodes to select them 
+        # Iterate through all nodes to select them
         # in the results of Dijkstra's algorithm
         for dest_node in nodes:
             if dest_node in arrival_times:
                 # Add results to the list
                 results.append(
                     {
-                     'source_node': source_node,
-                     'destination_node': dest_node,
-                     'arrival_time': arrival_times[dest_node],
-                     'travel_time': travel_times.get(dest_node, None)  # .get() to avoid KeyError
-                     })
+                        "source_node": source_node,
+                        "destination_node": dest_node,
+                        "arrival_time": arrival_times[dest_node],
+                        "travel_time": travel_times.get(dest_node, None),  # .get() to avoid KeyError
+                    }
+                )
 
     # Convert the list of results to a DataFrame and to a csv file
     results_df = pd.DataFrame(results)
 
     return results_df
 
 
-def _calculate_od_worker(source_node, nodes_list, graph, departure_time, hashtable=None):
+def _calculate_od_worker(
+    source_node, nodes_list, graph, departure_time, hashtable=None
+):
     """
     Internal worker function to calculate the OD matrix for a single source node.
     """
-    
+
     if hashtable:
         arrival_times, _, travel_times = single_source_time_dependent_dijkstra(
-            graph, source_node, departure_time, hashtable, algorithm='hashed'
+            graph, source_node, departure_time, hashtable, algorithm="hashed"
         )
     else:
         arrival_times, _, travel_times = single_source_time_dependent_dijkstra(
-            graph, source_node, departure_time, algorithm='sorted'
+            graph, source_node, departure_time, algorithm="sorted"
         )
-        
-    return [{
-        'source_node': source_node,
-        'destination_node': dest_node,
-        'arrival_time': arrival_times[dest_node],
-        'travel_time': travel_times.get(dest_node, None)
-    } for dest_node in nodes_list if dest_node in arrival_times]
 
+    return [
+        {
+            "source_node": source_node,
+            "destination_node": dest_node,
+            "arrival_time": arrival_times[dest_node],
+            "travel_time": travel_times.get(dest_node, None),
+        }
+        for dest_node in nodes_list
+        if dest_node in arrival_times
+    ]
 
-def calculate_od_matrix_parallel(graph, nodes, departure_time, target_nodes=None, num_processes=2, hashtable=None):
+
+def calculate_od_matrix_parallel(
+    graph, nodes, departure_time, target_nodes=None, num_processes=2, hashtable=None
+):
     """
-    Calculates the Origin-Destination (OD) matrix for a given graph, 
+    Calculates the Origin-Destination (OD) matrix for a given graph,
     nodes, and departure time using parallel processing.
 
     Parameters
     ----------
     graph : networkx.DiGraph
         The graph representing the transit network.
     nodes : list
@@ -115,111 +126,121 @@
         Optional hash table for the graph.
 
     Returns
     -------
     results_df : pandas.DataFrame
         A DataFrame containing the OD matrix.
     """
-    print(f'Calculating the OD using {num_processes} processes')
-
+    print(f"Calculating the OD using {num_processes} processes")
     time_start = time.perf_counter()
-    
+
     if not target_nodes:
         target_nodes = nodes
-    
+
     with multiprocessing.Pool(processes=num_processes) as pool:
         # Fix the arguments of the calculate_OD_worker function for nodes list
         partial_worker = partial(
             _calculate_od_worker,
-            nodes_list=target_nodes, 
-            graph=graph, 
+            nodes_list=target_nodes,
+            graph=graph,
             departure_time=departure_time,
-            hashtable=hashtable
-            )
-   
+            hashtable=hashtable,
+        )
         results = pool.map(partial_worker, nodes)
 
-    # Flatten the list of lists
-    results = [item for sublist in results for item in sublist]
-    results_df = pd.DataFrame(results)
-
     print(f"Time elapsed: {time.perf_counter() - time_start}")
-
-    return results_df
+    # Return flattened list of lists
+    return pd.DataFrame([item for sublist in results for item in sublist])
 
 
-def service_area(graph, source, start_time, cutoff, buffer_radius, algorithm = 'sorted', hashtable=None):
+def service_area(
+    graph: DiGraph,
+    source: Any,
+    start_time: int,
+    cutoff: float,
+    buffer_radius: float = 100,
+    algorithm: str = "sorted",
+    hashtable: Optional[Dict] = None,
+) -> gpd.GeoDataFrame:
     """
-    Creates a service area by buffering around all nodes within a travel time cutoff.
+    Creates a service area by buffering around all street edges within a travel time cutoff.
 
     Parameters
     ----------
     graph : networkx.DiGraph
         The graph to search.
-    source : hashable
+    source : node
         The graph node to start the search from.
     start_time : int
         The time to start the search from.
     cutoff : float
         The travel time cutoff for including nodes in the service area.
     buffer_radius : float
         The radius in meters for buffering around each point.
     algorithm : str, optional
-        Algorithm to use for the service area calculation (default: 'sorted').
+        Algorithm to use for the service area calculation (default: "sorted").
     hashtable : dict, optional
-        Hashtable required for the algorithm.
+        Hashtable required for the "hashed" algorithm.
 
     Returns
     -------
     geopandas.GeoDataFrame
         A GeoDataFrame containing the service area polygon.
+
+    Notes
+    -----
+    Output crs is EPSG:4087 (World Equidistant Cylindrical).
+
+    See Also
+    --------
+    nxtransit.accessibility.percent_access_service_area : Service area reachable with specified chance
+    nxtransit.accessibility.service_area_multiple_sources : Service areas for multiple sources using multiprocessing
+    nxtransit.functions.determine_utm_zone : Determine the UTM zone of a GeoDataFrame.
     """
 
     _, _, travel_times = single_source_time_dependent_dijkstra(
-        graph, 
-        source,
-        start_time,
-        hashtable,
-        algorithm
+        graph, source, start_time, hashtable, algorithm
     )
 
     # Filter nodes that are reachable within the cutoff
-    points_data = [{'node': node,
-                    'geometry': Point(graph.nodes[node]['x'],graph.nodes[node]['y']),
-                    'travel_time': travel_time
-                    }
-                   for node, travel_time in travel_times.items()
-                   if travel_time <= cutoff
-                   and 'x' in graph.nodes[node]
-                   and 'y' in graph.nodes[node]]
-    
-    reached_nodes = set([data['node'] for data in points_data])
+    points_data = [
+        {
+            "node": node,
+            "geometry": Point(graph.nodes[node]["x"], graph.nodes[node]["y"]),
+            "travel_time": travel_time,
+        }
+        for node, travel_time in travel_times.items()
+        if travel_time <= cutoff
+        and "x" in graph.nodes[node]
+        and "y" in graph.nodes[node]
+    ]
+
+    reached_nodes = set([data["node"] for data in points_data])
 
     # Filter edges so that both nodes are reached
-    reached_edges = [{'edge': (u, v), 'geometry': data['geometry']}
-                     for u, v, data in graph.edges(data=True)
-                     if u in reached_nodes 
-                     and v in reached_nodes 
-                     and 'geometry' in data
-                     and data['type'] == 'street'
-                     ]
-    
-    points_gdf = gpd.GeoDataFrame(points_data, geometry='geometry', crs="EPSG:4326")
-    edges_gdf = gpd.GeoDataFrame(reached_edges, geometry='geometry', crs="EPSG:4326")
-    
-    # Combine the GeoDataFrames
+    reached_edges = [
+        {"edge": (u, v), "geometry": data["geometry"]}
+        for u, v, data in graph.edges(data=True)
+        if u in reached_nodes
+        and v in reached_nodes
+        and "geometry" in data
+        and data["type"] == "street"
+    ]
+
+    edges_gdf = gpd.GeoDataFrame(reached_edges, geometry="geometry", crs="EPSG:4326")
+    utm_crs = determine_utm_zone(edges_gdf)
     # Re-projection to World Equidistant Cylindrical (EPSG:4087) for buffering in meters
-    merged_gdf = pd.concat([points_gdf, edges_gdf], ignore_index=True).to_crs("EPSG:4087")
-    # Nodes and edges buffered and merged into a single polygon
-    buffer_gdf = merged_gdf.buffer(buffer_radius)
-    
+    buffer_gdf = edges_gdf.to_crs(crs=utm_crs).buffer(buffer_radius)
+
     service_area_polygon = buffer_gdf.unary_union
     # overlap_count is needed for percent_access calculation
-    service_area_gdf = gpd.GeoDataFrame({'geometry': [service_area_polygon], 'id': source, 'overlap_count': 1}, 
-                                        crs="EPSG:4087")
+    service_area_gdf = gpd.GeoDataFrame(
+        {"geometry": [service_area_polygon], "id": source, "overlap_count": 1},
+        crs=utm_crs,
+    ).to_crs("EPSG:4087")
     return service_area_gdf
 
 
 def _rasterize_service_areas(service_areas, threshold, resolution=(100, 100)):
     """
     Rasterize given service area GeoDataFrames and summarize intersections.
 
@@ -240,53 +261,53 @@
     rasters = []
     # Rasterize each service area and append to the list
     for sa in service_areas:
         # Rasterize each service area
         cube = make_geocube(
             vector_data=sa,
             resolution=resolution,
-            measurements=['overlap_count'],
+            measurements=["overlap_count"],
         )
-
         rasters.append(cube)
-    
+
     # Combine the rasters into 3-dimensional xarray DataSet
     # Then sum the values along the 'summary' dimension
-    summarized_raster = xr.concat(rasters, dim='summary').sum(dim='summary')
-
+    summarized_raster = xr.concat(rasters, dim="summary").sum(dim="summary")
     # Vectorize the summarized raster back into a GeoDataFrame
-    vectorized_result = vectorize(
-        summarized_raster.overlap_count.astype("float32"))
-    
+    vectorized_result = vectorize(summarized_raster.overlap_count.astype("float32"))
+
     # Filter the vectorized result to include only polygons that cover at least the threshold of the service areas
     polygons_needed = int(len(service_areas) * threshold)
-    vectorized_result = vectorized_result[vectorized_result['overlap_count'] >= polygons_needed].unary_union
-    result_gdf = gpd.GeoDataFrame({'geometry': [vectorized_result]}, crs="EPSG:4087")
-    
+    vectorized_result = vectorized_result[
+        vectorized_result["overlap_count"] >= polygons_needed
+    ].unary_union
+    result_gdf = gpd.GeoDataFrame({"geometry": [vectorized_result]}, crs="EPSG:4087")
+
     return result_gdf
- 
- 
+
+
 def percent_access_service_area(
-        graph,
-        source,
-        start_time,
-        end_time,
-        sample_interval,
-        cutoff,
-        buffer_radius,
-        threshold,
-        **kwargs
-):
+    graph,
+    source,
+    start_time,
+    end_time,
+    sample_interval,
+    cutoff,
+    buffer_radius,
+    threshold,
+    algorithm="sorted",
+    hashtable=None,
+) -> gpd.GeoDataFrame:
     """
     Calculate service area reachable with specified chance within the given time period.
-    
+
     This tool rasterize service areas for each time step and overlays them.
-    Part of the raster that is covered by at least the threshold of 
+    Part of the raster that is covered by at least the threshold of
     the service areas is returned as a vectorized GeoDataFrame.
-    
+
     Parameters
     ----------
     graph : networkx.DiGraph
         The graph representing the transit network.
     source : Any
         The source node from which to service areas.
     start_time : int
@@ -297,43 +318,50 @@
         The interval between samples.
     cutoff : int
         The maximum travel time allowed to reach the service area.
     buffer_radius : float
         The radius of the buffer around the service area.
     threshold : float
         The threshold value for rasterizing the service areas.
-    **kwargs : dict
-        Additional keyword arguments for the service_area function.
-        - algorithm : str, optional. Algorithm to use for the service area calculation (default: 'sorted').
-        - hashtable : dict, optional. Hashtable required for the algorithm (default: None).
+    algorithm : str
+        optional. Algorithm to use for the service area calculation (default: 'sorted').
+    hashtable : dict, optional
+        Hashtable required for the algorithm (default: None).
 
     Returns
     -------
     gpd.GeoDataFrame
         GeoDataFrame containing the vectorized result.
     """
 
-    service_areas = [service_area(
-        graph, source, timestamp, cutoff, buffer_radius, **kwargs
-        ) for timestamp in range(start_time, end_time, sample_interval)]
-    
-    mean_area = _rasterize_service_areas(service_areas, threshold)
-    
-    return mean_area
-    
- 
+    service_areas = [
+        service_area(
+            graph=graph,
+            source=source,
+            start_time=timestamp,
+            cutoff=cutoff,
+            buffer_radius=buffer_radius,
+            algorithm=algorithm,
+            hashtable=hashtable,
+        )
+        for timestamp in range(start_time, end_time, sample_interval)
+    ]
+
+    return _rasterize_service_areas(service_areas=service_areas, threshold=threshold)
+
+
 def service_area_multiple_sources(
-        graph,
-        sources,
-        start_time,
-        cutoff,
-        buffer_radius,
-        algorithm='sorted',
-        hashtable=None,
-        num_processes=6
+    graph,
+    sources,
+    start_time,
+    cutoff,
+    buffer_radius,
+    algorithm="sorted",
+    hashtable=None,
+    num_processes=6,
 ):
     """
     Calculates service areas for multiple sources using multiprocessing, returning a combined service area polygon.
 
     Parameters
     ----------
     graph : networkx.DiGraph
@@ -355,24 +383,28 @@
 
     Returns
     -------
     combined_service_area : GeoDataFrame
         A GeoDataFrame containing the combined service area polygon for all sources.
     """
     # Prepare arguments for each task
-    tasks = [(graph, source, start_time, cutoff, buffer_radius, algorithm, hashtable) 
-             for source in sources]
-    
+    tasks = [
+        (graph, source, start_time, cutoff, buffer_radius, algorithm, hashtable)
+        for source in sources
+    ]
+
     with multiprocessing.Pool(processes=num_processes) as pool:
         results = pool.starmap(service_area, tasks)
-    
+
     # At this point, 'results' is a list of GeoDataFrames, each containing the service area polygon for a source
     # Combine all service area polygons into a single GeoDataFrame
-    combined_service_area = gpd.GeoDataFrame(pd.concat(results, ignore_index=True), crs="EPSG:4087")
- 
+    combined_service_area = gpd.GeoDataFrame(
+        pd.concat(results, ignore_index=True), crs="EPSG:4087"
+    )
+
     return combined_service_area
 
 
 def last_service(graph):
     """
     Calculate the last service time for each stop in the graph.
     Populates the 'last_service' attribute of each transit stop.
@@ -383,25 +415,27 @@
         The graph representing the transit network.
 
     Returns
     -------
     None
     """
     for node, data in graph.nodes(data=True):
-        if data['type'] == 'transit':
-            last_service_time = float('-inf')
+        if data["type"] == "transit":
+            last_service_time = float("-inf")
 
             for _, _, edge_data in graph.edges(node, data=True):
-                if 'sorted_schedules' in edge_data:
+                if "sorted_schedules" in edge_data:
                     # Get the last arrival and departure times
                     # from the sorted schedules
-                    last_arrival = edge_data['sorted_schedules'][-1][0]
-                    last_departure = edge_data['sorted_schedules'][-1][1]
+                    last_arrival = edge_data["sorted_schedules"][-1][0]
+                    last_departure = edge_data["sorted_schedules"][-1][1]
                     # Update the last service time if the current edge
                     # has a later service time
-                    last_service_time = max(last_service_time, last_arrival, last_departure)
+                    last_service_time = max(
+                        last_service_time, last_arrival, last_departure
+                    )
 
             # if the stop is not serviced, set last_service_time to None
-            if last_service_time == float('-inf'):
+            if last_service_time == float("-inf"):
                 last_service_time = None
 
-            data['last_service'] = last_service_time
+            data["last_service"] = last_service_time
```

### Comparing `NxTransit-0.1.20.dev0/nxtransit/connectors.py` & `NxTransit-0.1.21/nxtransit/connectors.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,30 +25,28 @@
             coords = transformer.transform(graph.nodes[node]['y'], graph.nodes[node]['x'])
 
             graph.nodes[node]['metric_X'] = coords[0]
             graph.nodes[node]['metric_Y'] = coords[1]
         except Exception as e:
             raise Exception(f'{e} occurred for node {node}')
 
-    return graph
-
 
 def connect_stops_to_streets(graph, stops: pd.DataFrame):
     """
     Connects GTFS stops to the nearest street node in the graph
     using projected coordinates in EPSG:4087.
     """
     # Create a list of street node tuples (x, y, node_id)
-    node_data = [(data['metric_X'], data['metric_Y'], n)
-                 for n, data in graph.nodes(data=True)
+    node_data = [(data['metric_X'], data['metric_Y'], idx)
+                 for idx, data in graph.nodes(data=True)
                  if 'metric_X' in data and 'metric_Y' in data
                  and data['type'] == 'street']
 
-    node_data_wgs = [(data['x'], data['y'], n)
-                     for n, data in graph.nodes(data=True)
+    node_data_wgs = [(data['x'], data['y'], idx)
+                     for idx, data in graph.nodes(data=True)
                      if 'y' in data and 'x' in data
                      and data['type'] == 'street']
 
     # Create a KD-tree for nearest neighbor search
     # The tree is created from a list of street node tuples (x, y, node_id)
     tree = KDTree([(x, y) for x, y, _ in node_data])
 
@@ -77,16 +75,14 @@
                         )
         graph.add_edge(nearest_street_node, stop['stop_id'],
                         weight=walk_time,
                         type='connector',
                         geometry=linestring
                         )
 
-    return graph
-
 
 def snap_points_to_network(graph, points):
     """
     Snaps point features from GeoDataFrame to the nearest street node in the graph.
 
     Parameters
     ----------
@@ -121,14 +117,17 @@
     # Create a KD-tree for nearest neighbor search
     # The tree is created from a list of street node tuples (x, y, node_id)
     tree = KDTree([(x, y) for x, y, _ in node_data_metric])
     
     crs_4326 = CRS.from_epsg(4326)
     crs_4087 = CRS.from_epsg(4087)
     transformer = Transformer.from_crs(crs_4326, crs_4087)
+    
+    if 'origin_id' not in points.columns:
+        points['origin_id'] = points.index
 
     for index, row in points.iterrows():
 
         geometry = row['geometry']
         point_id = row['origin_id']
         pnt_x, pnt_y = transformer.transform(geometry.y, geometry.x)
```

### Comparing `NxTransit-0.1.20.dev0/nxtransit/converters.py` & `NxTransit-0.1.21/nxtransit/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Utility functions for converting between different data types."""
 import time
 
 
 def parse_time_to_seconds(time_str: str) -> int:
-    """Converts a time string to the number of seconds since midnight.
-    """
+    """Converts a time string to the number of seconds since midnight"""
     try:
         if not isinstance(time_str, str):
             raise ValueError("Input must be a string.")
 
         parts = time_str.split(':')
         if len(parts) != 3:
             raise ValueError("Time string must be in 'HH:MM:SS' format.")
```

### Comparing `NxTransit-0.1.20.dev0/nxtransit/frequency.py` & `NxTransit-0.1.21/nxtransit/frequency.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Tools for calculating various frequency of transit service metrics in a network."""
 from functools import partial
 from statistics import mean
 
 import numpy as np
 import scipy.signal
-import tqdm
 
 from .routers import single_source_time_dependent_dijkstra, time_dependent_dijkstra
 
 
 def edge_frequency(graph, start_time, end_time):
     """
     Calculates the frequency of edges in a graph 
@@ -24,29 +23,29 @@
         The end time in seconds from midnight.
 
     Returns
     -------
     None
     """
 
-    for edge in graph.edges(data = True):
-        if 'schedules' in edge[2]:
-
-            trips = edge[2]['sorted_schedules']
-            seq = [(trips[i+1][0] - trips[i][0])
-                   for i in range(len(trips)-1)
-                   if start_time <= trips[i][0] <= end_time
-                   ]  # list containing the headways between consecutive trips along the edge
+    for edge in graph.edges(data=True):
+        if "schedules" in edge[2]:
+            trips = edge[2]["sorted_schedules"]
+            seq = [
+                (trips[i + 1][0] - trips[i][0])
+                for i in range(len(trips) - 1)
+                if start_time <= trips[i][0] <= end_time
+            ]  # list containing the headways between consecutive trips along the edge
 
             if len(seq) > 0:
                 frequency = mean(seq)
             else:
                 frequency = None
 
-            edge[2]['frequency'] = frequency  # mean vehicle headway in seconds along the edge
+            edge[2]["frequency"] = frequency
 
 
 def node_frequency(graph, start_time, end_time):
     """
     Calculates the frequency of departures at nodes in a graph 
     based on the schedules of adjacent edges between start_time and end_time.
 
@@ -60,42 +59,41 @@
         The end time in seconds from midnight.
 
     Returns
     -------
     None
     """
 
-    for node_view in tqdm.tqdm(graph.nodes(data=True)):
+    for node_view in graph.nodes(data=True):
         node = node_view[0]
         all_times = []
 
-        if node_view[1]['type'] == 'transit':
-
+        if node_view[1]["type"] == "transit":
             # Iterate through all edges adjacent to the current node
             for edge in graph.edges(node, data=True):
-                if 'schedules' in edge[2]:
-
-                    for schedule in edge[2]['schedules']:
+                if "schedules" in edge[2]:
+                    for schedule in edge[2]["schedules"]:
                         departure_time = schedule[0]
                         if start_time <= departure_time <= end_time:
                             all_times.append(departure_time)
 
             all_times.sort()
             # Calculate the headways between consecutive departures (arrivals?)
-            headways = [(all_times[i+1] - all_times[i])
-                        for i in range(len(all_times)-1)]
+            headways = [
+                (all_times[i + 1] - all_times[i]) for i in range(len(all_times) - 1)
+            ]
 
             if len(headways) > 0:
                 frequency = mean(headways)
             else:
                 frequency = None
 
-            graph.nodes[node]['frequency'] = frequency
-       
-     
+            graph.nodes[node]["frequency"] = frequency
+
+
 def connectivity_frequency(graph, source, target, start_time, end_time, sampling_interval=60):
     """
     Calculates the connectivity frequency between a source and target node in a graph
     over a specified time period.
 
     Parameters
     ----------
@@ -115,17 +113,18 @@
     Returns
     -------
     float
         The mean interval between peaks in the connectivity.
     """
     travel_parameters = [graph, source, target]
     func = partial(time_dependent_dijkstra, *travel_parameters)
-    data = [(start_time, func(start_time)[1]) for start_time
-            in range(start_time, end_time, sampling_interval)
-            ]
+    data = [
+        (start_time, func(start_time)[1])
+        for start_time in range(start_time, end_time, sampling_interval)
+    ]
 
     # Convert the travel times to a numpy array
     time_values = np.array([float(item[1]) for item in data])
     # Convert the time values to seconds
     time_seconds = np.array([float(item[0]) for item in data])
 
     # Compute the first and second derivatives of the travel times
@@ -141,16 +140,21 @@
     # Calculate the mean interval between the peaks
     mean_interval_between_peaks = np.mean(intervals)
 
     return mean_interval_between_peaks
 
 
 def single_source_connectivity_frequency(
-        graph, source, start_time, end_time,
-        sampling_interval=60, hashtable=None, algorithm='sorted'
+    graph,
+    source,
+    start_time,
+    end_time,
+    sampling_interval=60,
+    hashtable=None,
+    algorithm="sorted",
 ):
     """
     Calculates the mean interval between peaks in travel times from a source node to all other nodes
     in a graph over a specified time period.
 
     Parameters
     ----------
@@ -175,16 +179,15 @@
         A dictionary mapping each node to the mean interval between peaks in travel times.
     """
     node_to_intervals = {}  # Dictionary to hold intervals for each node
 
     # Iterate over each sampling interval
     for current_time in range(start_time, end_time, sampling_interval):
         _, _, travel_times = single_source_time_dependent_dijkstra(
-            graph, source, current_time,
-            hashtable=hashtable, algorithm=algorithm
+            graph, source, current_time, hashtable=hashtable, algorithm=algorithm
         )
 
         # Update travel times for each node
         for node, travel_time in travel_times.items():
             # Add the current time to the list of travel times for the node
             if node not in node_to_intervals:
                 node_to_intervals[node] = []
```

### Comparing `NxTransit-0.1.20.dev0/nxtransit/functions.py` & `NxTransit-0.1.21/nxtransit/functions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,124 @@
+import math
 import os
 
 import geopandas as gpd
 import pandas as pd
-import tqdm
 from shapely.geometry import Polygon
 
 
-def create_grid(gdf, cell_size):
+def determine_utm_zone(gdf) -> str:
     """
-    Creates a rectangular grid within the bounding box of a GeoDataFrame.
+    Determines the UTM zone for a GeoDataFrame based on its centroid.
+    
+    Parameters
+    ----------
+    gdf : GeoDataFrame
+        The input geospatial data.
+    
+    Returns
+    -------
+    epsg_code: str
+        UTM EPSG code as string.
+    """
+    # Ensure the GeoDataFrame is in geographic coordinates (EPSG:4326)
+    gdf_proj = gdf.to_crs("EPSG:4326")
 
+    minx, miny, maxx, maxy = gdf_proj.total_bounds
+    centroid_longitude = (minx + maxx) / 2
+
+    # Determine UTM zone number
+    utm_zone = math.floor((centroid_longitude + 180) / 6) + 1
+    # Determine hemisphere (north or south)
+    hemisphere = "north" if (miny + maxy) / 2 >= 0 else "south"
+    # Construct EPSG code for UTM
+    epsg_code = (
+        f"EPSG:326{utm_zone}" if hemisphere == "north" else f"EPSG:327{utm_zone}"
+    )
+
+    return epsg_code
+
+
+def aggregate_to_grid(gdf: gpd.GeoDataFrame, cell_size: float) -> gpd.GeoDataFrame:
+    """
+    Creates a grid of square cells covering the extent of the input GeoDataFrame, 
+    and keeps cells that contain at least one feature from the source GeoDataFrame.
+    
     Parameters
     ----------
     gdf : gpd.GeoDataFrame
-        GeoDataFrame containing the geometry to be gridded.
+        The input GeoDataFrame representing the spatial extent and features.
     cell_size : float
-        Size of the grid cells in the meters.
-
+        The size of each square cell in the grid in meters.
+    
     Returns
     -------
     gpd.GeoDataFrame
-        Polygon grid.
+        The resulting grid GeoDataFrame, with cells containing at least
+        one feature from the source GeoDataFrame, and a 'id' for each cell.
     """
-
-    gdf = gdf.to_crs("EPSG:4087")  # Project to metric CRS for accurate cell size
-    xmin, ymin, xmax, ymax = gdf.total_bounds
-    rows = int((ymax - ymin) / cell_size)
-    cols = int((xmax - xmin) / cell_size)
-    grid = []
-    ids = []  # List to hold the unique IDs
-
-    for i in range(cols):
-        for j in range(rows):
-            x1 = xmin + i * cell_size
-            y1 = ymin + j * cell_size
+    utm_crs = determine_utm_zone(gdf)
+    gdf_utm = gdf.to_crs(utm_crs)
+    minx, miny, maxx, maxy = gdf_utm.total_bounds
+
+    nx = math.ceil((maxx - minx) / cell_size)
+    ny = math.ceil((maxy - miny) / cell_size)
+    grid_cells = []
+    grid_indices = []
+    index = 0  # Initialize a counter for the grid index
+    for i in range(nx):
+        for j in range(ny):
+            x1 = minx + i * cell_size
+            y1 = miny + j * cell_size
             x2 = x1 + cell_size
             y2 = y1 + cell_size
-            grid.append(Polygon([(x1, y1), (x2, y1), (x2, y2), (x1, y2)]))
-            ids.append(f"grid_{i*rows + j + 1}")  # Generate unique ID
+            cell = Polygon([(x1, y1), (x2, y1), (x2, y2), (x1, y2)])
+            grid_cells.append(cell)
+            grid_indices.append(f"grid_{index}")  # Add the current index to the list
+            index += 1  # Increment the index for the next cell
 
-    grid_geodataframe = gpd.GeoDataFrame({'id': ids, 'geometry': grid}, crs="EPSG:4087")
-    
-    return grid_geodataframe
+    # Create the initial grid GeoDataFrame
+    grid = gpd.GeoDataFrame({'id': grid_indices, 'geometry': grid_cells}, crs=utm_crs)
+
+    # Perform a spatial join between the grid and the original GeoDataFrame
+    filtered_grid = gpd.sjoin(grid, gdf_utm, how='inner')
 
+    # Drop duplicates to ensure each cell is unique, keeping only 'geometry' and 'grid_index'
+    filtered_grid = filtered_grid[['geometry', 'id']].drop_duplicates(subset=['id'])
+    filtered_grid.reset_index(drop=True, inplace=True)
 
-def create_centroids_dataframe(polygon_gdf):
+    return filtered_grid
+
+
+def create_centroids_dataframe(polygon_gdf) -> gpd.GeoDataFrame:
     """
     Creates a GeoDataFrame with the centroids of polygons from the given GeoDataFrame.
 
     Parameters
     ----------
     polygon_gdf : gpd.GeoDataFrame
         GeoDataFrame containing polygons.
 
     Returns
     -------
     gpd.GeoDataFrame
         GeoDataFrame with Point geometries of the centroids.
     """
-
+    # Create id column if it doesn't exist
+    # ID is required for the explicit origin_id column in the final output
+    if "id" not in polygon_gdf.columns:
+        polygon_gdf["id"] = polygon_gdf.index
     # Create a GeoDataFrame with these centroids
     # and include the 'origin_id' from the parent polygon
-    centroids_gdf = gpd.GeoDataFrame(polygon_gdf[['id']].copy(),
-                                     geometry=polygon_gdf.geometry.centroid, 
-                                     crs=polygon_gdf.crs
-                                     )
-    centroids_gdf.rename(columns={'id': 'origin_id'}, inplace=True)
+    centroids_gdf = gpd.GeoDataFrame(
+        polygon_gdf[["id"]].copy(),
+        geometry=polygon_gdf.to_crs("EPSG:4087").geometry.centroid,
+        crs="EPSG:4087",
+    )
+    centroids_gdf.rename(columns={"id": "origin_id"}, inplace=True)
 
     return centroids_gdf
 
 
 def validate_feed(gtfs_path: str) -> bool:
     """
     Validates the GTFS feed located at the specified path.
@@ -161,14 +210,16 @@
         # Validate time format (HH:MM:SS)
         time_format_regex = r'^(\d{2}):([0-5]\d):([0-5]\d)$'  # check for HH:MM:SS format
         invalid_departure_times = stop_times_df[~stop_times_df['departure_time'].str.match(time_format_regex)]
         invalid_arrival_times = stop_times_df[~stop_times_df['arrival_time'].str.match(time_format_regex)]
 
         if not invalid_departure_times.empty or not invalid_arrival_times.empty:
             print("Invalid time format found in departure or arrival times in stop_times.txt.")
+            print(f"Invalid departure times: {invalid_departure_times['departure_time'].values}")
+            print(f"Invalid arrival times: {invalid_arrival_times['arrival_time'].values}")
         
         # Additional format and consistency checks= will be added
      
     except Exception as e:
         print(f"Error during validation: {e}")
         return False
 
@@ -257,34 +308,35 @@
         The source node from which to calculate the travel times.
 
     Returns
     -------
     pandas.DataFrame
         A DataFrame containing the transit time and pedestrian time for each node.
     """
-    
     results = []
-    
-    for node in tqdm.tqdm(graph.nodes(data=True)):
-        
+    for node in graph.nodes(data=True):
         if node[0] != source:
-
             path = _reconstruct_path(node[0], predecessors)
             pedestrian_path = _unpack_path_vertices(path)
             pedestrian_time = _calculate_pedestrian_time(pedestrian_path, graph)
-            
+
             transit_time = travel_times[node[0]] - pedestrian_time
+            results.append(
+                {
+                    "node": node[0],
+                    "transit_time": transit_time,
+                    "pedestrian_time": pedestrian_time,
+                }
+            )
 
-            results.append({'node': node[0], 'transit_time': transit_time, 'pedestrian_time': pedestrian_time})
-        
     results = pd.DataFrame(results)
     return results
 
 
-def process_graph_to_hash_table(graph):
+def process_graph_to_hash_table(graph) -> dict:
     """
     Process a graph and convert it into a hash table
     mapping edges to their sorted schedules or static weights.
 
     Parameters
     ----------
     graph : networkx.DiGraph
@@ -293,17 +345,17 @@
     Returns
     -------
     dict
         A dict mapping edges to their sorted schedules or static weights.
     """
     schedules_hash = {}
     for from_node, to_node, data in graph.edges(data=True):
-        if 'sorted_schedules' in data:
-            schedules_hash[(from_node, to_node)] = data['sorted_schedules']
+        if "sorted_schedules" in data:
+            schedules_hash[(from_node, to_node)] = data["sorted_schedules"]
         else:
             # Static weight wrapped in a list of tuples to make it iterable
-            static_weight = data['weight']
+            static_weight = data["weight"]
             schedules_hash[(from_node, to_node)] = [
                 (static_weight,)
             ]  # comma is to make it a tuple
 
     return schedules_hash
```

### Comparing `NxTransit-0.1.20.dev0/nxtransit/loaders.py` & `NxTransit-0.1.21/nxtransit/loaders.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,115 +11,127 @@
 
 from .connectors import _fill_coordinates, connect_stops_to_streets
 from .converters import parse_time_to_seconds
 from .other import logger
 
 
 def _preprocess_schedules(graph: nx.DiGraph):
-    # Sorting schedules for faster lookup using binary search
-    for edge in graph.edges(data=True):
-        if 'schedules' in edge[2]:
-            edge[2]['sorted_schedules'] = sorted(
-                edge[2]['schedules'],
-                key=lambda x: x[0])
-
-            edge[2]['departure_times'] = sorted([elem[0] for elem
-                                                 in edge[2]['sorted_schedules']],
-                                                key=lambda x: x)
-
-
-def _add_edges_to_graph(graph: nx.DiGraph,
-                        sorted_stop_times: pd.DataFrame,
-                        trips_df: pd.DataFrame,
-                        shapes: dict,
-                        trip_to_shape_map: dict,
-                        read_shapes: bool = False
-                        ):
     """
-    Adds edges with schedule information and optionally shape geometry between stops to the graph.
+    Sorts the schedules on each edge for faster lookup.
+    """
+    for _, _, data in graph.edges(data=True):
+        if "schedules" in data:
+            sorted_schedules = sorted(data["schedules"], key=lambda x: x[0])
+            data["sorted_schedules"] = sorted_schedules
+            data["departure_times"] = [schedule[0] for schedule in sorted_schedules]
+
+
+def _add_edge_with_geometry(graph, start_stop, end_stop, schedule_info, geometry):
+    """
+    Adds or updates an edge in the graph with schedule information and geometry.
+    """
+    edge = (start_stop["stop_id"], end_stop["stop_id"])
+    if graph.has_edge(*edge):
+        graph[edge[0]][edge[1]]["schedules"].append(schedule_info)
+        if "geometry" not in graph[edge[0]][edge[1]]:
+            graph[edge[0]][edge[1]]["geometry"] = geometry
+    else:
+        graph.add_edge(*edge, schedules=[schedule_info], type="transit", geometry=geometry)
+
+
+def _process_trip_group(
+    group, graph, trips_df, shapes, trip_to_shape_map, stops_df, read_shapes
+):
+    """
+    Processes a group of sorted stops for a single trip, adding edges between them to the graph.
 
     Parameters
     ----------
-    graph : nx.DiGraph
-        The networkx graph to which the edges will be added.
-    sorted_stop_times : pd.DataFrame
-        A DataFrame containing sorted stop times information.
+    group : pd.DataFrame
+        A group of sorted stops for a single trip.
+    graph : networkx.DiGraph
+        The graph to which the edges will be added.
     trips_df : pd.DataFrame
-        A DataFrame containing trip information, including shape_id.
+        DataFrame containing trip information.
     shapes : dict
-        A dictionary mapping shape_ids to their respective linestring geometries.
+        Dictionary mapping shape IDs to shape geometries.
     trip_to_shape_map : dict
-        A dictionary mapping trip_ids to shape_ids.
-    read_shapes : bool, optional
-        If True, shape geometries will be added to the edges. Defaults to True.
+        Dictionary mapping trip IDs to shape IDs.
+    stops_df : pd.DataFrame
+        DataFrame containing stop information.
+    read_shapes : bool
+        Flag indicating whether to read shape geometries from shapes.txt.
+
+    Returns
+    -------
+    None
     """
-    # For each pair of consecutive stops in the group (trip),
-    # create an edge with schedule information
-    # If the edge already exists, add the schedule to the list of schedules
-
-    # Uses trip_id -> shape_id mapping to add shape geometry to the edge
-    # In order to avoid searching the shapes DataFrame for each trip_id
-
-    for i in range(len(sorted_stop_times) - 1):
-        start_stop = sorted_stop_times.iloc[i]
-        end_stop = sorted_stop_times.iloc[i + 1]
-        edge = (start_stop['stop_id'], end_stop['stop_id'])
-
-        departure = parse_time_to_seconds(start_stop['departure_time'])
-        arrival = parse_time_to_seconds(end_stop['arrival_time'])
-        trip_id = start_stop['trip_id']
-
-        # Getting route_id from trips_df
-        # (searching by trip_id in trips_df and selecting route_id column)
-        route_id = trips_df.loc[trips_df['trip_id'] == trip_id, 'route_id'].values[0]
-
-        if 'wheelchair_accessible' in trips_df.columns:
-            wheelchair_accessible = trips_df.loc[
-                trips_df['trip_id'] == trip_id, 
-                'wheelchair_accessible'].values[0]
-        else:
-            wheelchair_accessible = None
+    # Mapping stop_id to coordinates for faster lookup
+    stop_coords_mapping = stops_df.set_index("stop_id")[["stop_lat", "stop_lon"]].to_dict("index")
+    trip_route_mapping = trips_df.set_index("trip_id")["route_id"].to_dict()
+
+    # Some GTFS feeds do not have wheelchair_accessible information
+    if "wheelchair_accessible" in trips_df.columns:
+        trip_wheelchair_mapping = trips_df.set_index("trip_id")["wheelchair_accessible"].to_dict()
+    else:
+        trip_wheelchair_mapping = {}
 
-        schedule_info = (departure, arrival, route_id, wheelchair_accessible)
+    # For each pair of consecutive stops in the group, add an edge to the graph
+    for i in range(len(group) - 1):
+        start_stop, end_stop = group.iloc[i], group.iloc[i + 1]
+        departure, arrival = (
+            parse_time_to_seconds(start_stop["departure_time"]),
+            parse_time_to_seconds(end_stop["arrival_time"]),
+        )
+        trip_id = start_stop["trip_id"]
+        route_id = trip_route_mapping.get(trip_id)
+        wheelchair_accessible = trip_wheelchair_mapping.get(trip_id, None)
 
+        schedule_info = (departure, arrival, route_id, wheelchair_accessible)
+    
+        # If read_shapes is True, use the shape geometry from shapes.txt
         geometry = None
         if read_shapes:
             shape_id = trip_to_shape_map.get(trip_id)
-            if shape_id in shapes:
-                geometry = shapes[shape_id]
-
-        # if edge already exists, add schedule to the list of schedules
-        # Currently the geometry is added to the first edge found
-
-        if graph.has_edge(*edge):
-            graph[edge[0]][edge[1]]['schedules'].append(schedule_info)
-        # Create a new edge otherwise
+            geometry = shapes.get(shape_id)
+        # Otherwise, use the stop coordinates to create a simple LineString geometry
         else:
-            if read_shapes:
-                graph.add_edge(
-                    *edge, schedules=[schedule_info],
-                    type='transit', geometry=geometry
+            start_coords, end_coords = (
+                stop_coords_mapping.get(start_stop["stop_id"]),
+                stop_coords_mapping.get(end_stop["stop_id"])
+            )
+            if start_coords and end_coords:
+                geometry = LineString(
+                    [
+                        (start_coords["stop_lon"], start_coords["stop_lat"]),
+                        (end_coords["stop_lon"], end_coords["stop_lat"]),
+                    ]
                 )
-            else:
-                graph.add_edge(*edge, schedules=[schedule_info], type='transit')
 
+        _add_edge_with_geometry(graph, start_stop, end_stop, schedule_info, geometry)
 
-def _add_edges_parallel(graph, trips_chunk, trips_df, shapes, read_shapes, trip_to_shape_map):
-    """
-    Adds edges to the graph for a chunk of trips.
-    """
-    local_graph = graph.copy()  # Make a copy for local modifications
-    for trip_id, group in trips_chunk.groupby(['trip_id']):
-        sorted_group = group.sort_values('stop_sequence')
-        _add_edges_to_graph(local_graph,
-                            sorted_group,
-                            trips_df=trips_df,
-                            shapes=shapes,
-                            read_shapes=read_shapes,
-                            trip_to_shape_map=trip_to_shape_map)
+
+def _add_edges_parallel(
+    graph, trips_chunks, trips_df, shapes, read_shapes, trip_to_shape_map, stops_df
+):
+    """
+    Adds edges to the graph for chunks of trips in parallel.
+    """
+    local_graph = graph.copy()
+    for _, group in trips_chunks.groupby(["trip_id"]):
+        sorted_group = group.sort_values("stop_sequence")
+        _process_trip_group(
+            sorted_group,
+            local_graph,
+            trips_df,
+            shapes,
+            trip_to_shape_map,
+            stops_df,
+            read_shapes,
+        )
     return local_graph
 
 
 def _filter_stop_times_by_time(stop_times: pd.DataFrame, departure_time: int, duration_seconds: int):
     """Filters stop_times to only include trips that occur within a specified time window."""
 
     stop_times['departure_time_seconds'] = stop_times['departure_time'].apply(parse_time_to_seconds)
@@ -177,46 +189,45 @@
     trips_df = pd.read_csv(os.path.join(GTFSpath, "trips.txt"))
 
     routes = pd.read_csv(os.path.join(GTFSpath, "routes.txt"), 
                          usecols=['route_id', 'route_short_name'])
 
     # Load shapes.txt if read_shapes is True
     if read_shapes:
-        if 'shapes.txt' not in os.listdir(GTFSpath):
-            raise FileNotFoundError('shapes.txt not found')
+        if "shapes.txt" not in os.listdir(GTFSpath):
+            raise FileNotFoundError("shapes.txt not found")
 
         shapes_df = pd.read_csv(os.path.join(GTFSpath, "shapes.txt"))
         # Group geometry by shape_id, resulting in a Pandas Series
         # with trip_id (shape_id ?) as keys and LineString geometries as values
         # This is definitely not working as intended
-        shapes = shapes_df.groupby('shape_id')[['shape_pt_lon', 'shape_pt_lat']].apply(
-        lambda group: LineString(group.values)
+        shapes = shapes_df.groupby("shape_id")[["shape_pt_lon", "shape_pt_lat"]].apply(
+            lambda group: LineString(group.values)
         )
         # Mapping trip_id to shape_id for faster lookup
-        trip_to_shape_map = trips_df.set_index('trip_id')['shape_id'].to_dict()
+        trip_to_shape_map = trips_df.set_index("trip_id")["shape_id"].to_dict()
 
     else:
         shapes = None
         trip_to_shape_map = None
 
     # Join route information to trips``
-    trips_df = trips_df.merge(routes, on='route_id')
+    trips_df = trips_df.merge(routes, on="route_id")
 
     # Check if calendar.txt exists in GTFS directory
     # If it does, filter by day of the week, otherwise raise an error
-    if 'calendar.txt' in os.listdir(GTFSpath):
+    if "calendar.txt" in os.listdir(GTFSpath):
         calendar_df = pd.read_csv(os.path.join(GTFSpath, "calendar.txt"))
         # Filter for the day of the week
-        service_ids = calendar_df[calendar_df[day_of_week] == 1]['service_id']
-        trips_df = trips_df[trips_df['service_id'].isin(service_ids)]
+        service_ids = calendar_df[calendar_df[day_of_week] == 1]["service_id"]
+        trips_df = trips_df[trips_df["service_id"].isin(service_ids)]
     else:
-        raise FileNotFoundError('Required file calendar.txt not found')
+        raise FileNotFoundError("Required file calendar.txt not found")
 
-    # Filter stop_times to only include trips that occur 
-    # within a specified time window
+    # Filter stop_times to only include trips that occur within a specified time window
     valid_trips = stop_times_df['trip_id'].isin(trips_df['trip_id'])
     stop_times_df = stop_times_df[valid_trips].dropna()
 
     # Convert departure_time from HH:MM:SS o seconds
     departure_time_seconds = parse_time_to_seconds(departure_time_input)
     # Filtering stop_times by time window
     filtered_stops = _filter_stop_times_by_time(stop_times_df,
@@ -224,85 +235,85 @@
                                                 duration_seconds
                                                 )
 
     print(f'GTFS data loaded\n{len(filtered_stops)} of {len(stop_times_df)} trips retained')
 
     # Adding stops as nodes to the graph
     for _, stop in stops_df.iterrows():
-        G.add_node(stop['stop_id'],
-                   type='transit',
-                   pos=(stop['stop_lon'], stop['stop_lat']),
-                   x=stop['stop_lon'],
-                   y=stop['stop_lat']
-                   )
+        G.add_node(
+            stop["stop_id"],
+            type="transit",
+            pos=(stop["stop_lon"], stop["stop_lat"]),
+            x=stop["stop_lon"],
+            y=stop["stop_lat"],
+        )
 
     if multiprocessing:
-
-        print('Building graph in parallel')
+        print("Building graph in parallel")
         # Divide filtered_stops into chunks for parallel processing
         # Use half of the available CPU logical cores
         # (likely equal to the number of physical cores)
         num_cores = int(mp.cpu_count() / 2)
         chunks = np.array_split(filtered_stops, num_cores)
 
         # Create a pool of processes
         with mp.Pool(processes=num_cores) as pool:
             # Create a subgraph in each process
             # Each will return a graph with edges for a subset of trips
             # The results will be combined into a single graph
-            results = pool.starmap(_add_edges_parallel,
-                                   [(G, chunk, trips_df, shapes,
-                                     read_shapes, trip_to_shape_map) for chunk in chunks
-                                    ])
+            results = pool.starmap(
+                _add_edges_parallel,
+                [
+                    (G, chunk, trips_df, shapes, read_shapes, trip_to_shape_map, stops_df)
+                    for chunk in chunks
+                ],
+            )
 
         # Merge results from all processes
         merged_graph = nx.DiGraph()
 
         for graph in results:
             merged_graph.add_nodes_from(graph.nodes(data=True))
-        # Add edges from subgraphs to the merged graph 
+        # Add edges from subgraphs to the merged graph
         for graph in results:
             for u, v, data in graph.edges(data=True):
                 # If edge already exists, merge schedules
                 if merged_graph.has_edge(u, v):
                     # Merge sorted_schedules attribute
-                    existing_schedules = merged_graph[u][v]['schedules']
-                    new_schedules = data['schedules']
-                    merged_graph[u][v]['schedules'] = existing_schedules + new_schedules
+                    existing_schedules = merged_graph[u][v]["schedules"]
+                    new_schedules = data["schedules"]
+                    merged_graph[u][v]["schedules"] = existing_schedules + new_schedules
                 # If edge does not exist, add it
                 else:
                     # Add new edge with data
                     merged_graph.add_edge(u, v, **data)
 
         # Sorting schedules for faster lookup using binary search
         _preprocess_schedules(merged_graph)
-        logger.info('Transit graph created')
+        logger.info("Transit graph created")
 
         return merged_graph, stops_df
 
     else:
-
-        print('Building graph in a single process')
-        # Splitting trips into groups by trip_id, then iteratively processing each group
-        # For each group, sort by stop_sequence, then add edges to the graph
-        for trip_id, group in filtered_stops.groupby('trip_id'):
-            sorted_group = group.sort_values('stop_sequence')
-            _add_edges_to_graph(
-                G,
+        for trip_id, group in filtered_stops.groupby("trip_id"):
+            sorted_group = group.sort_values("stop_sequence")
+            _process_trip_group(
                 sorted_group,
-                trips_df = trips_df,
-                shapes = shapes,
-                read_shapes = read_shapes,
-                trip_to_shape_map = trip_to_shape_map
+                G,
+                trips_df,
+                shapes,
+                trip_to_shape_map,
+                stops_df,
+                read_shapes,
             )
 
         # Sorting schedules for faster lookup using binary search
         _preprocess_schedules(G)
 
-        logger.info('Transit graph created')
+        logger.info("Transit graph created")
 
         return G, stops_df
 
 
 def _load_osm(stops, save_graphml, path) -> nx.DiGraph:
     """
     Loads OpenStreetMap data within a convex hull of stops in GTFS feed, 
@@ -319,127 +330,126 @@
 
     Returns
     -------
     G_city : networkx.DiGraph
         A street network graph with walking times as edge weights.
     """
     # Building a convex hull from stop coordinates for OSM loading
-    boundary = gpd.GeoSeries(
-        [Point(lon, lat) for lon, lat
-         in zip(stops['stop_lon'], stops['stop_lat'])
-         ]).unary_union.convex_hull
+    stops_gdf = gpd.GeoDataFrame(stops, geometry=gpd.points_from_xy(stops.stop_lon, stops.stop_lat))
+    boundary = stops_gdf.unary_union.convex_hull
 
-    logger.info('Loading OSM graph via OSMNX')
+    logger.info("Loading OSM graph via OSMNX")
     # Loading OSM data within the convex hull
-    G_city = ox.graph_from_polygon(boundary,
-                                   network_type='walk',
-                                   simplify=True)
-
+    G_city = ox.graph_from_polygon(boundary, network_type="walk", simplify=True)
+    
+    attributes_to_keep = {"length", "highway", "name"}
     for u, v, key, data in G_city.edges(keys=True, data=True):
         # Clean extra attributes
-        attributes_to_keep = {'length', 'highway', 'name'}
+        
         for attribute in list(data):
             if attribute not in attributes_to_keep:
                 del data[attribute]
-        
+
         # Calculate walking time in seconds
-        data['weight'] = data['length'] / 1.39
-        data['type'] = 'street'
-        
+        data["weight"] = data["length"] / 1.39
+        data["type"] = "street"
+
         # Add geometry to the edge
-        u_geom = Point(G_city.nodes[u]['x'], G_city.nodes[u]['y'])
-        v_geom = Point(G_city.nodes[v]['x'], G_city.nodes[v]['y'])
-        data['geometry'] = LineString([u_geom, v_geom])
+        u_geom = Point(G_city.nodes[u]["x"], G_city.nodes[u]["y"])
+        v_geom = Point(G_city.nodes[v]["x"], G_city.nodes[v]["y"])
+        data["geometry"] = LineString([u_geom, v_geom])
 
-    for _, data in G_city.nodes(data=True):
-        data['type'] = 'street'
+    nx.set_node_attributes(G_city, "street", "type")
 
     if save_graphml:
         ox.save_graphml(G_city, path)
 
-    # Convert MultiDiGraph from OSMNX to DiGraph
-    G_city = nx.DiGraph(G_city)
-    logger.info('Street network graph created')
+    logger.info("Street network graph created")
 
-    return G_city
+    return nx.DiGraph(G_city)
 
 
 def feed_to_graph(
     GTFSpath: str, 
     departure_time_input: str,
     day_of_week: str,
     duration_seconds: int,
     read_shapes: bool = False,
-    multiprocessing: bool = False,
+    multiprocessing: bool = True,
     input_graph_path: str = None,
     output_graph_path: str = None,
     save_graphml: bool = False,
     load_graphml: bool = False,
-) -> tuple[nx.DiGraph, pd.DataFrame]:
+) -> nx.DiGraph:
     """
     Creates a directed graph (DiGraph) based on General Transit Feed Specification (GTFS) and OpenStreetMap (OSM) data.
 
     Parameters
     ----------
     GTFSpath : str
         Path to the GTFS files.
     departure_time_input : str
         Departure time in 'HH:MM:SS' format.
     day_of_week : str
         Day of the week in lowercase (e.g., 'monday').
     duration_seconds : int
         Time period from departure for which the graph will be loaded.
     read_shapes : bool, optional
-        Flag for reading geometry from shapes.txt file. Default is False.
+        Flag for reading geometry from shapes.txt file. Default is False. This parameter is currently not working as intended.
     multiprocessing : bool, optional
         Flag for using multiprocessing. Default is False.
     input_graph_path : str, optional
         Path to the OSM graph file in GraphML format. Default is None.
     output_graph_path : str, optional
         Path for saving the OSM graph in GraphML format. Default is None.
     save_graphml : bool, optional
         Flag for saving the OSM graph in GraphML format. Default is False.
     load_graphml : bool, optional
         Flag for loading the OSM graph from a GraphML file. Default is False.
 
     Returns
     -------
     G_combined : nx.DiGraph
-        Combined directed graph.
+        Combined multimodal graph representing transit network.
     """
-    G_transit, stops = _load_GTFS(GTFSpath, departure_time_input,
-                                  day_of_week, duration_seconds,
-                                  read_shapes=read_shapes,
-                                  multiprocessing=multiprocessing)
+    G_transit, stops = _load_GTFS(
+        GTFSpath,
+        departure_time_input,
+        day_of_week,
+        duration_seconds,
+        read_shapes=read_shapes,
+        multiprocessing=multiprocessing,
+    )
 
     if load_graphml:
-        print('Loading OSM graph from GraphML file')
+        print("Loading OSM graph from GraphML file")
         # Dictionary with data types for edges
-        edge_dtypes = {'weight': float, 'length': float}
+        edge_dtypes = {"weight": float, "length": float}
         G_city = ox.load_graphml(input_graph_path, edge_dtypes=edge_dtypes)
         G_city = nx.DiGraph(G_city)
     else:
         # Import OSM data
         G_city = _load_osm(stops, save_graphml, output_graph_path)
 
     # Combining OSM and GTFS data
     G_combined = nx.compose(G_transit, G_city)
     # Filling projected coordinates for graph nodes
     _fill_coordinates(G_combined)
 
     # Connecting stops to OSM streets
-    G_combined = connect_stops_to_streets(G_combined, stops)
+    connect_stops_to_streets(G_combined, stops)
 
     logger.info(
-        f'Nodes: {G_combined.number_of_nodes()}, Edges: {G_combined.number_of_edges()}'
+        f"Nodes: {G_combined.number_of_nodes()}, Edges: {G_combined.number_of_edges()}"
     )
 
     return G_combined
 
-def load_stops_gdf(path):
+
+def load_stops_gdf(path) -> gpd.GeoDataFrame:
     """
     Load stops data from a specified path and return a GeoDataFrame.
 
     Parameters
     ----------
     path: str
         The path to the directory containing the stops data.
@@ -447,14 +457,13 @@
     Returns
     -------
     stops_gdf: gpd.GeoDataFrame
         GeoDataFrame containing the stops data with geometry information.
 
     """
     stops_df = pd.read_csv(os.path.join(path, "stops.txt"))
-    stops_gdf = gpd.GeoDataFrame(stops_df, 
-                                 geometry=gpd.points_from_xy(
-                                     stops_df.stop_lon, 
-                                     stops_df.stop_lat),
-                                 crs = 'epsg:4326'
-                                 )
+    stops_gdf = gpd.GeoDataFrame(
+        stops_df,
+        geometry=gpd.points_from_xy(stops_df.stop_lon, stops_df.stop_lat),
+        crs="epsg:4326",
+    )
     return stops_gdf
```

### Comparing `NxTransit-0.1.20.dev0/nxtransit/prism.py` & `NxTransit-0.1.21/nxtransit/prism.py`

 * *Files identical despite different names*

### Comparing `NxTransit-0.1.20.dev0/nxtransit/routers.py` & `NxTransit-0.1.21/nxtransit/routers.py`

 * *Files 8% similar despite different names*

```diff
@@ -127,19 +127,17 @@
         # Add the node to the visited set to avoid visiting it again
         visited.add(u)
 
         # Iterate over all neighbors of the node
         for v in graph.neighbors(u):
             # If the neighbor has not been visited yet
             if v not in visited:
-                delay, route = _calculate_delay_sorted(graph,
-                                                       u, v,
-                                                       current_time,
-                                                       wheelchair=wheelchair
-                                                       )
+                delay, route = _calculate_delay_sorted(
+                    graph, u, v, current_time, wheelchair=wheelchair
+                )
                 # Skip the neighbor if the arrival time is infinite
                 if delay == float('inf'):
                     continue
                 # Calculate the new arrival time for the neighbor
                 new_arrival_time = current_time + delay
                 # If the new arrival time is better, update the arrival time and predecessor
                 if new_arrival_time < arrival_times[v]:
@@ -206,38 +204,41 @@
         A tuple containing three dictionaries:
             - arrival_times: A dictionary mapping each node to the earliest arrival time from the source node.
             - predecessors: A dictionary mapping each node to its predecessor on the shortest path from the source node.
             - travel_times: A dictionary mapping each node to the travel time from the source node.
     """
     if source not in graph:
         raise ValueError(f"The source node {source} does not exist in the graph.")
+    
+    if not isinstance(start_time, (int, float)):
+        raise ValueError("The start time must be a number.")
 
-    arrival_times = {node: float('inf') for node in graph.nodes}
+    arrival_times = {node: float("inf") for node in graph.nodes}
     predecessors = {node: None for node in graph.nodes}
     arrival_times[source] = start_time
     travel_times = {}
     queue = [(start_time, source)]
 
     while queue:
         current_time, current_node = heappop(queue)
 
         for neighbor in graph.neighbors(current_node):
             delay = _calculate_delay_sorted_nr(
                 graph, current_node, neighbor, current_time
-                )
+            )
             new_arrival_time = current_time + delay
 
             if new_arrival_time < arrival_times[neighbor]:
                 arrival_times[neighbor] = new_arrival_time
                 predecessors[neighbor] = current_node
                 heappush(queue, (new_arrival_time, neighbor))
 
                 travel_times[neighbor] = new_arrival_time - start_time
-    # Реконструкция пути не производится
-    # Однако на основе 'predecessors' можно восстановить путь к любому узлу
+    # Path reconstruction is not performed
+    # However, based on 'predecessors', you can reconstruct the path to any node
 
     return arrival_times, predecessors, travel_times
 
 
 def single_source_time_dependent_dijkstra_hashed(graph, source, start_time, hashtable):
     """
     Finds the shortest path from a source node to all other nodes in a time-dependent graph using Dijkstra's algorithm.
@@ -269,26 +270,30 @@
     """
     if hashtable is None:
         raise ValueError("The hash table is required for this algorithm.")
 
     if source not in graph:
         raise ValueError(f"The source node {source} does not exist in the graph.")
 
-    arrival_times = {node: float('inf') for node in graph.nodes}
+    if not isinstance(start_time, (int, float)):
+        raise ValueError("The start time must be a number.")
+
+    arrival_times = {node: float("inf") for node in graph.nodes}
     predecessors = {node: None for node in graph.nodes}
     arrival_times[source] = start_time
     travel_times = {}
     queue = [(start_time, source)]
 
     while queue:
         current_time, current_node = heappop(queue)
 
         for neighbor in graph.neighbors(current_node):
-
-            delay = _calculate_delay_hashed(current_node, neighbor, current_time, hashtable)
+            delay = _calculate_delay_hashed(
+                current_node, neighbor, current_time, hashtable
+            )
             new_arrival_time = current_time + delay
 
             if new_arrival_time < arrival_times[neighbor]:
                 arrival_times[neighbor] = new_arrival_time
                 predecessors[neighbor] = current_node
                 heappush(queue, (new_arrival_time, neighbor))
 
@@ -325,18 +330,15 @@
             - predecessors: A dictionary mapping each node to its predecessor on the shortest path from the source node.
             - travel_times: A dictionary mapping each node to the travel time from the source node.
             
     See Also
     --------
     nxtransit.functions.process_graph_to_hash_table : Create a hash table for quick access to sorted schedules.
     """
-
-    if algorithm == 'sorted':
-        return(single_source_time_dependent_dijkstra_sorted(
-            graph, source, start_time
-            ))
-    elif algorithm == 'hashed':
-        return(single_source_time_dependent_dijkstra_hashed(
+    if algorithm == "sorted":
+        return single_source_time_dependent_dijkstra_sorted(graph, source, start_time)
+    elif algorithm == "hashed":
+        return single_source_time_dependent_dijkstra_hashed(
             graph, source, start_time, hashtable
-            ))
+        )
     else:
         raise (ValueError, "Invalid algorithm. Use 'sorted' or 'hashed'")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `NxTransit-0.1.20.dev0/pyproject.toml` & `NxTransit-0.1.21/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 authors = [{ name = "Chingiz Zhanarbaev" }]
 readme = "README.md" 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows",
+    "Operating System :: POSIX :: Linux",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: GIS",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Visualization",
@@ -26,15 +27,14 @@
     "networkx>=3.2.0",
     "numpy>=1.26.4",
     "osmnx>=1.9.1",
     "pandas>=2.2.0",
     "pytest>=8.0.1",
     "scipy>=1.12.0",
     "Shapely>=2.0.3",
-    "tqdm>=4.66.1",
     "geocube>=0.5.0",
 ]
 license = {text = "MIT License"}
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 tests = [
```

### Comparing `NxTransit-0.1.20.dev0/tests/test_routers.py` & `NxTransit-0.1.21/tests/test_routers.py`

 * *Files identical despite different names*

