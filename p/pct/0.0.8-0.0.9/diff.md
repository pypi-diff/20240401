# Comparing `tmp/pct-0.0.8.tar.gz` & `tmp/pct-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pct-0.0.8.tar", last modified: Sat Sep  5 12:10:30 2020, max compression
+gzip compressed data, was "dist\pct-0.0.9.tar", last modified: Tue Nov  3 20:02:47 2020, max compression
```

## Comparing `pct-0.0.8.tar` & `pct-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,24 @@
-drwxrwxrwx   0        0        0        0 2020-09-05 12:10:30.000000 pct-0.0.8/
--rw-rw-rw-   0        0        0     2381 2020-07-07 20:02:14.000000 pct-0.0.8/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11558 2020-07-07 20:02:14.000000 pct-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      116 2020-07-07 20:02:14.000000 pct-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5873 2020-09-05 12:10:30.000000 pct-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4109 2020-09-05 12:08:31.000000 pct-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2020-09-05 12:10:30.000000 pct-0.0.8/nbdev_template/
--rw-rw-rw-   0        0        0       23 2020-07-08 18:42:29.000000 pct-0.0.8/nbdev_template/__init__.py
--rw-rw-rw-   0        0        0      360 2020-07-08 18:42:30.000000 pct-0.0.8/nbdev_template/_nbdev.py
--rw-rw-rw-   0        0        0      200 2020-07-08 18:42:30.000000 pct-0.0.8/nbdev_template/core.py
-drwxrwxrwx   0        0        0        0 2020-09-05 12:10:30.000000 pct-0.0.8/pct/
--rw-rw-rw-   0        0        0       23 2020-09-05 12:09:42.000000 pct-0.0.8/pct/__init__.py
--rw-rw-rw-   0        0        0     1171 2020-09-05 12:09:42.000000 pct-0.0.8/pct/_nbdev.py
--rw-rw-rw-   0        0        0      111 2020-09-05 12:09:42.000000 pct-0.0.8/pct/examples.py
--rw-rw-rw-   0        0        0    13117 2020-09-05 12:09:42.000000 pct-0.0.8/pct/functions.py
--rw-rw-rw-   0        0        0     8736 2020-09-05 12:09:42.000000 pct-0.0.8/pct/hierarchy.py
--rw-rw-rw-   0        0        0      932 2020-09-05 12:09:42.000000 pct-0.0.8/pct/mymod.py
--rw-rw-rw-   0        0        0     9904 2020-09-05 12:09:42.000000 pct-0.0.8/pct/nodes.py
--rw-rw-rw-   0        0        0     1902 2020-09-05 12:09:42.000000 pct-0.0.8/pct/putils.py
-drwxrwxrwx   0        0        0        0 2020-09-05 12:10:30.000000 pct-0.0.8/pct.egg-info/
--rw-rw-rw-   0        0        0     5873 2020-09-05 12:10:30.000000 pct-0.0.8/pct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2020-09-05 12:10:30.000000 pct-0.0.8/pct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-09-05 12:10:30.000000 pct-0.0.8/pct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2020-09-05 12:10:30.000000 pct-0.0.8/pct.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2020-07-30 19:43:58.000000 pct-0.0.8/pct.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2020-09-05 12:10:30.000000 pct-0.0.8/pct.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2020-09-05 12:10:30.000000 pct-0.0.8/pct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      647 2020-09-05 11:08:14.000000 pct-0.0.8/settings.ini
--rw-rw-rw-   0        0        0       42 2020-09-05 12:10:30.000000 pct-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1968 2020-07-07 20:02:14.000000 pct-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2020-11-03 20:02:47.000000 pct-0.0.9/
+-rw-rw-rw-   0        0        0     2381 2020-10-20 19:06:56.000000 pct-0.0.9/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11558 2020-10-20 19:06:56.000000 pct-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      116 2020-10-20 19:06:56.000000 pct-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4480 2020-11-03 20:02:47.000000 pct-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3012 2020-11-03 19:53:46.000000 pct-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2020-11-03 20:02:47.000000 pct-0.0.9/pct/
+-rw-rw-rw-   0        0        0       23 2020-11-03 19:53:34.000000 pct-0.0.9/pct/__init__.py
+-rw-rw-rw-   0        0        0     1330 2020-11-03 19:53:34.000000 pct-0.0.9/pct/_nbdev.py
+-rw-rw-rw-   0        0        0    20165 2020-11-03 19:53:34.000000 pct-0.0.9/pct/functions.py
+-rw-rw-rw-   0        0        0    12440 2020-11-03 19:53:34.000000 pct-0.0.9/pct/hierarchy.py
+-rw-rw-rw-   0        0        0    13391 2020-11-03 19:53:34.000000 pct-0.0.9/pct/nodes.py
+-rw-rw-rw-   0        0        0     2702 2020-11-03 19:53:34.000000 pct-0.0.9/pct/putils.py
+drwxrwxrwx   0        0        0        0 2020-11-03 20:02:47.000000 pct-0.0.9/pct.egg-info/
+-rw-rw-rw-   0        0        0     4480 2020-11-03 20:02:47.000000 pct-0.0.9/pct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2020-11-03 20:02:47.000000 pct-0.0.9/pct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-11-03 20:02:47.000000 pct-0.0.9/pct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2020-11-03 20:02:47.000000 pct-0.0.9/pct.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2020-10-31 13:04:39.000000 pct-0.0.9/pct.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2020-11-03 20:02:47.000000 pct-0.0.9/pct.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2020-11-03 20:02:47.000000 pct-0.0.9/pct.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      672 2020-10-20 19:06:56.000000 pct-0.0.9/settings.ini
+-rw-rw-rw-   0        0        0       42 2020-11-03 20:02:47.000000 pct-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1968 2020-10-20 19:06:56.000000 pct-0.0.9/setup.py
```

### Comparing `pct-0.0.8/CONTRIBUTING.md` & `pct-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pct-0.0.8/LICENSE` & `pct-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pct-0.0.8/pct/_nbdev.py` & `pct-0.0.9/pct/_nbdev.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # AUTOGENERATED BY NBDEV! DO NOT EDIT!
 
 __all__ = ["index", "modules", "custom_doc_links", "git_url"]
 
 index = {"UniqueNamer": "01_putils.ipynb",
          "FunctionsList": "01_putils.ipynb",
+         "sigmoid": "01_putils.ipynb",
+         "is_in_notebooks": "01_putils.ipynb",
          "BaseFunction": "02_functions.ipynb",
+         "Subtract": "02_functions.ipynb",
          "Proportional": "02_functions.ipynb",
          "Variable": "02_functions.ipynb",
          "PassOn": "02_functions.ipynb",
          "GreaterThan": "02_functions.ipynb",
-         "Subtract": "02_functions.ipynb",
          "Constant": "02_functions.ipynb",
+         "Step": "02_functions.ipynb",
          "Integration": "02_functions.ipynb",
+         "IntegrationDual": "02_functions.ipynb",
+         "Sigmoid": "02_functions.ipynb",
          "WeightedSum": "02_functions.ipynb",
          "IndexedParameter": "02_functions.ipynb",
          "OpenAIGym": "02_functions.ipynb",
          "PCTNode": "03_nodes.ipynb",
          "PCTNodeData": "03_nodes.ipynb",
-         "PCTHierarchy": "04_hierarchy.ipynb",
-         "MyNamer": "06_mymod.ipynb"}
+         "PCTHierarchy": "04_hierarchy.ipynb"}
 
 modules = ["putils.py",
            "functions.py",
            "nodes.py",
-           "hierarchy.py",
-           "mymod.py"]
+           "hierarchy.py"]
 
 doc_url = "https://perceptualrobots.github.io/pct/"
 
 git_url = "https://github.com/perceptualrobots/pct/tree/master/"
 
 def custom_doc_links(name): return None
```

### Comparing `pct-0.0.8/pct/hierarchy.py` & `pct-0.0.9/pct/hierarchy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: nbs/04_hierarchy.ipynb (unless otherwise specified).
 
 __all__ = ['PCTHierarchy']
 
 # Cell
+import networkx as nx
+import json
+from networkx.drawing.nx_agraph import graphviz_layout
+import matplotlib.pyplot as plt
 import numpy as np
 from .nodes import PCTNode
 from .functions import *
 from .putils import UniqueNamer
 from .putils import FunctionsList
 
 # Cell
 class PCTHierarchy():
     "A hierarchical perceptual control system, of PCTNodes."
-    def __init__(self, levels=0, cols=0, pre=[], post=[], name="pcthierarchy", clear_names=True, links="single", history=False, build=True, **pargs):
+    def __init__(self, levels=0, cols=0, pre=None, post=None, name="pcthierarchy", clear_names=True, links="single", history=False, build=True, **pargs):
         self.links_built = False
         self.order=None
         if clear_names:
             UniqueNamer.getInstance().clear()
         self.name=UniqueNamer.getInstance().get_name(name)
-        self.preCollection=pre
-        self.postCollection=post
+        if pre==None:
+            self.preCollection=[]
+        else:
+            self.preCollection=pre
+        if post==None:
+            self.postCollection=[]
+        else:
+            self.postCollection=post
         self.hierarchy = []
         for r in range(levels):
             col_list=[]
             for c in range(cols):
                 if links == "dense":
                     if r > 0:
                         perc = WeightedSum(weights=np.ones(cols))
@@ -138,40 +148,127 @@
             thatnode.add_link("reference", thisnode.get_function("output"))
 
         if links_type == "dense":
             for column in range(len(self.hierarchy[level-1])):
                 thatnode = self.hierarchy[level-1][column]
                 thatnode.add_link("reference", thisnode.get_function("output"))
 
+
+    def get_node_positions(self, align='horizontal'):
+        graph = self.graph()
+        pos = nx.multipartite_layout(graph, subset_key="layer", align=align)
+        return pos
+
+
+    def draw(self, with_labels=True,  font_size=12, font_weight='bold', node_color='red',
+             node_size=500, arrowsize=25, align='horizontal', file=None, figsize=(8,8), move={}):
+        graph = self.graph()
+        pos = nx.multipartite_layout(graph, subset_key="layer", align=align)
+
+        for key in move.keys():
+            pos[key][0]+=move[key][0]
+            pos[key][1]+=move[key][1]
+
+        plt.figure(figsize=figsize)
+        nx.draw(graph, pos=pos, with_labels=with_labels, font_size=font_size, font_weight=font_weight,
+                node_color=node_color,  node_size=node_size, arrowsize=arrowsize)
+        #plt.show()
+
+        if file != None:
+            plt.title(self.name)
+            plt.savefig(file)
+
+    def graph(self):
+        graph = nx.DiGraph()
+
+        self.set_graph_data(graph)
+
+        return graph
+
+    def set_graph_data(self, graph):
+        layer=0
+        if len(self.preCollection)>0 or len(self.postCollection)>0:
+            layer=1
+
+        for func in self.postCollection:
+            func.set_graph_data(graph, layer=0)
+
+        for func in self.preCollection:
+            func.set_graph_data(graph, layer=0)
+
+        for level in range(len(self.hierarchy)):
+            for col in range(len(self.hierarchy[level])-1, -1, -1):
+            #for col in range(len(self.hierarchy[level])):
+                  self.hierarchy[level][col].set_graph_data(graph, layer=layer)
+            layer+=3
+
+
+    def build_links(self):
+        for level in range(len(self.hierarchy)):
+            for col in range(len(self.hierarchy[level])):
+                  self.hierarchy[level][col].build_links()
+
+
+    def clear_values(self):
+        for func in self.postCollection:
+            func.value = 0
+
+        for func in self.preCollection:
+            func.value = 0
+
+        for level in range(len(self.hierarchy)):
+            for col in range(len(self.hierarchy[level])):
+                  self.hierarchy[level][col].clear_values()
+
+
     def summary(self, build=True):
         print(self.name, type(self).__name__)
 
         print("**************************")
         print("PRE:", end=" ")
         if len(self.preCollection) == 0:
             print("None")
         for func in self.preCollection:
             func.summary()
 
 
-        for level in range(len(self.hierarchy)):
-            print(f'Level {level}')
-            for col in range(len(self.hierarchy[level])):
-                  self.hierarchy[level][col].summary(build=build)
+        if self.order==None:
+            for level in range(len(self.hierarchy)):
+                print(f'Level {level}')
+                for col in range(len(self.hierarchy[level])):
+                      self.hierarchy[level][col].summary(build=build)
+        elif self.order=="Down":
+            for level in range(len(self.hierarchy)-1, -1, -1):
+                print(f'Level {level}')
+                for col in range(len(self.hierarchy[level])-1, -1, -1):
+                      self.hierarchy[level][col].summary(build=build)
 
         print("POST:", end=" ")
         if len(self.postCollection) == 0:
             print("None")
         for func in self.postCollection:
             func.summary()
 
 
         print("**************************")
 
+    def save(self, file=None, indent=4):
+        jsondict = json.dumps(self.get_config(), indent=indent)
+        f = open(file, "w")
+        f.write(jsondict)
+        f.close()
 
+    @classmethod
+    def load(cls, file, clear=True):
+        if clear:
+            FunctionsList.getInstance().clear()
+
+        with open(file) as f:
+            config = json.load(f)
+        return cls.from_config(config)
 
     def get_config(self):
         config = {"type": type(self).__name__,
                     "name": self.name}
 
         pre = {}
         for i in range(len(self.preCollection)):
@@ -239,13 +336,22 @@
             if level == levels:
                 self.hierarchy.append([])
             self.hierarchy[level].insert(col, node)
 
     def insert_function(self, level=None, col=None, collection=None, function=None, position=-1):
         self.hierarchy[level][col].insert_function(collection, function, position)
 
+    def replace_function(self, level=None, col=None, collection=None, function=None, position=-1):
+        self.hierarchy[level][col].replace_function(collection, function, position)
+
     def get_function(self, level=None, col=None, collection=None, position=-1):
         return self.hierarchy[level][col].get_function(collection, position)
 
     def set_links(self, func_name, *link_names):
+        func = FunctionsList.getInstance().get_function(func_name)
+        func.clear_links()
+        for link_name in link_names:
+            func.add_link(FunctionsList.getInstance().get_function(link_name))
+
+    def add_links(self, func_name, *link_names):
         for link_name in link_names:
             FunctionsList.getInstance().get_function(func_name).add_link(FunctionsList.getInstance().get_function(link_name))
```

### Comparing `pct-0.0.8/pct/nodes.py` & `pct-0.0.9/pct/nodes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: nbs/03_nodes.ipynb (unless otherwise specified).
 
 __all__ = ['PCTNode', 'PCTNodeData']
 
 # Cell
+import networkx as nx
+import json
+import matplotlib.pyplot as plt
 from .putils import UniqueNamer
 from .putils import FunctionsList
 from .functions import *
 
 # Cell
 class PCTNode():
     "A single PCT controller."
@@ -152,14 +155,53 @@
         if collection == "comparator":
             self.comparatorCollection[position].set_name(name)
 
         if collection == "output":
             self.outputCollection[position].set_name(name)
 
 
+    def replace_function(self, collection, function, position=-1):
+        if collection == "reference":
+            """
+            func = self.referenceCollection[position]
+            FunctionsList.getInstance().remove_function(func.get_name())
+            if len(self.referenceCollection) == 0:
+                position=-1
+            """
+            self.referenceCollection[position] = function
+
+        if collection == "perception":
+            """
+            func = self.perceptionCollection[position]
+            FunctionsList.getInstance().remove_function(func.get_name())
+            if len(self.perceptionCollection) == 0:
+                position=-1
+            """
+            self.perceptionCollection[position]  = function
+
+        if collection == "comparator":
+            """
+            func = self.comparatorCollection[position]
+            FunctionsList.getInstance().remove_function(func.get_name())
+            if len(self.comparatorCollection) == 0:
+                position=-1
+            """
+            self.comparatorCollection[position] = function
+
+        if collection == "output":
+            """
+            func = self.outputCollection[position]
+            FunctionsList.getInstance().remove_function(func.get_name())
+            if len(self.outputCollection) == 0:
+                position=-1
+            """
+            self.outputCollection[position] = function
+
+
+
     def insert_function(self, collection, function, position=-1):
         if collection == "reference":
             self.referenceCollection[position] = function
 
         if collection == "perception":
             self.perceptionCollection[position]  = function
 
@@ -191,14 +233,61 @@
 
         print("OUT:", end=" ")
         for outputFunction in self.outputCollection:
             outputFunction.summary()
 
         print("----------------------------")
 
+
+    def graph(self, layer=0):
+        graph = nx.DiGraph()
+
+        self.set_graph_data(graph, layer=layer)
+
+        return graph
+
+
+    def clear_values(self):
+        for referenceFunction in self.referenceCollection:
+            referenceFunction.value = 0
+
+        for comparatorFunction in self.comparatorCollection:
+            comparatorFunction = 0
+
+        for perceptionFunction in self.perceptionCollection:
+            perceptionFunction = 0
+
+        for outputFunction in self.outputCollection:
+            outputFunction  = 0
+
+
+    def set_graph_data(self, graph, layer=0):
+
+        for referenceFunction in self.referenceCollection:
+            referenceFunction.set_graph_data(graph, layer+2)
+
+        for comparatorFunction in self.comparatorCollection:
+            comparatorFunction.set_graph_data(graph, layer+1)
+
+        for perceptionFunction in self.perceptionCollection:
+            perceptionFunction.set_graph_data(graph, layer+2)
+
+        for outputFunction in self.outputCollection:
+            outputFunction.set_graph_data(graph, layer)
+
+
+    def draw(self, with_labels=True,  font_size=12, font_weight='bold', node_color='red',
+             node_size=500, arrowsize=25, align='horizontal', file=None, figsize=(5,5), move={}):
+
+        graph = self.graph()
+        pos = nx.multipartite_layout(graph, subset_key="layer", align=align)
+        plt.figure(figsize=figsize)
+        nx.draw(graph, pos=pos, with_labels=with_labels, font_size=font_size, font_weight=font_weight,
+                node_color=node_color,  node_size=node_size, arrowsize=arrowsize)
+
     def get_config(self):
         config = {"type": type(self).__name__,
                     "name": self.name}
 
         coll_name = 'refcoll'
         collection = self.referenceCollection
         config[coll_name] = self.get_collection_config(coll_name, collection)
@@ -218,14 +307,26 @@
         coll = {}
         ctr=0
         for func in collection:
             coll[str(ctr)] = func.get_config()
             ctr+=1
         return coll
 
+    def save(self, file=None, indent=4):
+        jsondict = json.dumps(self.get_config(), indent=indent)
+        f = open(file, "w")
+        f.write(jsondict)
+        f.close()
+
+    @classmethod
+    def load(cls, file):
+        with open(file) as f:
+            config = json.load(f)
+        return cls.from_config(config)
+
     @classmethod
     def from_config(cls, config):
         node = PCTNode(default=False, name=config['name'])
 
         node.referenceCollection = []
         collection = node.referenceCollection
         coll_dict = config['refcoll']
@@ -242,15 +343,15 @@
         PCTNode.collection_from_config(collection, coll_dict)
 
         node.outputCollection = []
         collection = node.outputCollection
         coll_dict = config['outcoll']
         PCTNode.collection_from_config(collection, coll_dict)
 
-        #node.build_links()
+        node.links_built = True
         return node
 
     @classmethod
     def collection_from_config(node, collection, coll_dict):
         #print("collection_from_config", coll_dict)
         for fndict_label in coll_dict:
             #print("fndict_label",fndict_label)
```

### Comparing `pct-0.0.8/settings.ini` & `pct-0.0.9/settings.ini`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 user = perceptualrobots
 description = Perceptual Control Theory with Python
 keywords = pct, control systems, robotics, psychology
 author = Rupert Young
 author_email = rupert@perceptualrobots.com
 copyright = Rupert Young
 branch = master
-version = 0.0.8
+version = 0.0.9
 min_python = 3.6
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 2
 nbs_path = nbs
 doc_path = docs
 doc_host = https://perceptualrobots.github.io
 doc_baseurl = /pct/
 git_url = https://github.com/perceptualrobots/pct/tree/master/
 lib_path = pct
 title = pct
-requirements = plotly numpy gym
-
+requirements = plotly numpy gym networkx matplotlib graphviz
```

### Comparing `pct-0.0.8/setup.py` & `pct-0.0.9/setup.py`

 * *Files identical despite different names*

