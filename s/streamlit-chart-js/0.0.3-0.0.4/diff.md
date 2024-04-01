# Comparing `tmp/streamlit_chart_js-0.0.3.tar.gz` & `tmp/streamlit_chart_js-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_chart_js-0.0.3.tar", last modified: Sat Mar 30 12:30:59 2024, max compression
+gzip compressed data, was "streamlit_chart_js-0.0.4.tar", last modified: Mon Apr  1 10:22:36 2024, max compression
```

## Comparing `streamlit_chart_js-0.0.3.tar` & `streamlit_chart_js-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 cwargnier   (501) staff       (20)        0 2024-03-30 12:30:59.944337 streamlit_chart_js-0.0.3/
--rw-r--r--   0 cwargnier   (501) staff       (20)        0 2024-03-28 18:07:16.000000 streamlit_chart_js-0.0.3/MANIFEST.in
--rw-r--r--   0 cwargnier   (501) staff       (20)     2951 2024-03-30 12:30:59.942884 streamlit_chart_js-0.0.3/PKG-INFO
--rw-r--r--   0 cwargnier   (501) staff       (20)     2540 2024-03-29 19:49:40.000000 streamlit_chart_js-0.0.3/README.md
--rw-r--r--   0 cwargnier   (501) staff       (20)       38 2024-03-30 12:30:59.944766 streamlit_chart_js-0.0.3/setup.cfg
--rw-r--r--   0 cwargnier   (501) staff       (20)      666 2024-03-30 12:30:36.000000 streamlit_chart_js-0.0.3/setup.py
-drwxr-xr-x   0 cwargnier   (501) staff       (20)        0 2024-03-30 12:30:59.743476 streamlit_chart_js-0.0.3/streamit_chartjs/
--rw-r--r--   0 cwargnier   (501) staff       (20)        0 2024-03-28 18:07:16.000000 streamlit_chart_js-0.0.3/streamit_chartjs/__init__.py
--rw-r--r--   0 cwargnier   (501) staff       (20)     2681 2024-03-30 12:19:28.000000 streamlit_chart_js-0.0.3/streamit_chartjs/st_chart_component.py
--rw-r--r--   0 cwargnier   (501) staff       (20)     2461 2024-03-30 12:17:55.000000 streamlit_chart_js-0.0.3/streamit_chartjs/st_chart_component_working_back_up.py
-drwxr-xr-x   0 cwargnier   (501) staff       (20)        0 2024-03-30 12:30:59.913795 streamlit_chart_js-0.0.3/streamlit_chart_js.egg-info/
--rw-r--r--   0 cwargnier   (501) staff       (20)     2951 2024-03-30 12:30:59.000000 streamlit_chart_js-0.0.3/streamlit_chart_js.egg-info/PKG-INFO
--rw-r--r--   0 cwargnier   (501) staff       (20)      362 2024-03-30 12:30:59.000000 streamlit_chart_js-0.0.3/streamlit_chart_js.egg-info/SOURCES.txt
--rw-r--r--   0 cwargnier   (501) staff       (20)        1 2024-03-30 12:30:59.000000 streamlit_chart_js-0.0.3/streamlit_chart_js.egg-info/dependency_links.txt
--rw-r--r--   0 cwargnier   (501) staff       (20)       10 2024-03-30 12:30:59.000000 streamlit_chart_js-0.0.3/streamlit_chart_js.egg-info/requires.txt
--rw-r--r--   0 cwargnier   (501) staff       (20)       17 2024-03-30 12:30:59.000000 streamlit_chart_js-0.0.3/streamlit_chart_js.egg-info/top_level.txt
+drwxr-xr-x   0 cwargnier   (501) staff       (20)        0 2024-04-01 10:22:36.874145 streamlit_chart_js-0.0.4/
+-rw-r--r--   0 cwargnier   (501) staff       (20)        0 2024-03-28 18:07:16.000000 streamlit_chart_js-0.0.4/MANIFEST.in
+-rw-r--r--   0 cwargnier   (501) staff       (20)     8351 2024-04-01 10:22:36.873548 streamlit_chart_js-0.0.4/PKG-INFO
+-rw-r--r--   0 cwargnier   (501) staff       (20)     7940 2024-03-30 21:44:31.000000 streamlit_chart_js-0.0.4/README.md
+-rw-r--r--   0 cwargnier   (501) staff       (20)       38 2024-04-01 10:22:36.874348 streamlit_chart_js-0.0.4/setup.cfg
+-rw-r--r--   0 cwargnier   (501) staff       (20)      666 2024-04-01 10:22:33.000000 streamlit_chart_js-0.0.4/setup.py
+drwxr-xr-x   0 cwargnier   (501) staff       (20)        0 2024-04-01 10:22:36.863712 streamlit_chart_js-0.0.4/streamit_chartjs/
+-rw-r--r--   0 cwargnier   (501) staff       (20)        0 2024-03-28 18:07:16.000000 streamlit_chart_js-0.0.4/streamit_chartjs/__init__.py
+-rw-r--r--   0 cwargnier   (501) staff       (20)     2673 2024-04-01 10:11:37.000000 streamlit_chart_js-0.0.4/streamit_chartjs/st_chart_component.py
+-rw-r--r--   0 cwargnier   (501) staff       (20)     2453 2024-04-01 10:11:37.000000 streamlit_chart_js-0.0.4/streamit_chartjs/st_chart_component_working_back_up.py
+drwxr-xr-x   0 cwargnier   (501) staff       (20)        0 2024-04-01 10:22:36.871628 streamlit_chart_js-0.0.4/streamlit_chart_js.egg-info/
+-rw-r--r--   0 cwargnier   (501) staff       (20)     8351 2024-04-01 10:22:36.000000 streamlit_chart_js-0.0.4/streamlit_chart_js.egg-info/PKG-INFO
+-rw-r--r--   0 cwargnier   (501) staff       (20)      362 2024-04-01 10:22:36.000000 streamlit_chart_js-0.0.4/streamlit_chart_js.egg-info/SOURCES.txt
+-rw-r--r--   0 cwargnier   (501) staff       (20)        1 2024-04-01 10:22:36.000000 streamlit_chart_js-0.0.4/streamlit_chart_js.egg-info/dependency_links.txt
+-rw-r--r--   0 cwargnier   (501) staff       (20)       10 2024-04-01 10:22:36.000000 streamlit_chart_js-0.0.4/streamlit_chart_js.egg-info/requires.txt
+-rw-r--r--   0 cwargnier   (501) staff       (20)       17 2024-04-01 10:22:36.000000 streamlit_chart_js-0.0.4/streamlit_chart_js.egg-info/top_level.txt
```

### Comparing `streamlit_chart_js-0.0.3/setup.py` & `streamlit_chart_js-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="streamlit_chart_js",
-    version="0.0.3",
+    version="0.0.4",
     author="Charly Wargnier",
     author_email="cwar05@gnail.com",
     description="A custom Streamlit component for Chart.js",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `streamlit_chart_js-0.0.3/streamit_chartjs/st_chart_component.py` & `streamlit_chart_js-0.0.4/streamit_chartjs/st_chart_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import streamlit.components.v1 as components
 import json
 import uuid
 
 
-def my_chart_component(
+def st_chartjs(
     data,
     chart_type="bar",
     canvas_width=700,  # Set the canvas width for the chart
     canvas_height=700,  # Set the canvas height for the chart
     title="Custom Chart Title",
     legend_position="top",
     x_axis_title="Category",
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 import streamlit.components.v1 as components import json import uuid def
-my_chart_component( data, chart_type="bar", canvas_width=700, # Set the canvas
-width for the chart canvas_height=700, # Set the canvas height for the chart
+st_chartjs( data, chart_type="bar", canvas_width=700, # Set the canvas width
+for the chart canvas_height=700, # Set the canvas height for the chart
 title="Custom Chart Title", legend_position="top", x_axis_title="Category",
 y_axis_title="Value", stacked=False, # Add stacked option with default value
 False ): unique_id = uuid.uuid4().hex canvas_id = f"myChart-{unique_id}"
 data_json = json.dumps(data) options = { "plugins": { "legend": { "display":
 True, "position": legend_position, }, "title": { "display": True, "text":
 title, "font": { "size": 16, }, }, }, "scales": { "y": { "beginAtZero": True,
 "display": chart_type in ["bar", "line"], "title": { "display": True, "text":
```

### Comparing `streamlit_chart_js-0.0.3/streamit_chartjs/st_chart_component_working_back_up.py` & `streamlit_chart_js-0.0.4/streamit_chartjs/st_chart_component_working_back_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import streamlit.components.v1 as components
 import json
 import uuid
 
 
-def my_chart_component(
+def st_chartjs(
     data,
     chart_type="bar",
     canvas_width=700,  # Set the canvas width for the chart
     canvas_height=700,  # Set the canvas height for the chart
     title="Custom Chart Title",
     legend_position="top",
     x_axis_title="Category",
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 import streamlit.components.v1 as components import json import uuid def
-my_chart_component( data, chart_type="bar", canvas_width=700, # Set the canvas
-width for the chart canvas_height=700, # Set the canvas height for the chart
+st_chartjs( data, chart_type="bar", canvas_width=700, # Set the canvas width
+for the chart canvas_height=700, # Set the canvas height for the chart
 title="Custom Chart Title", legend_position="top", x_axis_title="Category",
 y_axis_title="Value", ): unique_id = uuid.uuid4().hex canvas_id = f"myChart-
 {unique_id}" data_json = json.dumps(data) options = { "plugins": { "legend":
 { "display": True, "position": legend_position, }, "title": { "display": True,
 "text": title, "font": { "size": 16, }, }, }, "scales": { "y": { "beginAtZero":
 True, "display": chart_type in ["bar", "line"], "title": { "display": True,
 "text": y_axis_title, "font": { "size": 14, }, }, }, "x": { "display": True,
```

