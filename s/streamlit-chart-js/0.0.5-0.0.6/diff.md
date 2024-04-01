# Comparing `tmp/streamlit_chart_js-0.0.5.tar.gz` & `tmp/streamlit_chart_js-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_chart_js-0.0.5.tar", last modified: Mon Apr  1 13:27:53 2024, max compression
+gzip compressed data, was "streamlit_chart_js-0.0.6.tar", last modified: Mon Apr  1 13:49:52 2024, max compression
```

## Comparing `streamlit_chart_js-0.0.5.tar` & `streamlit_chart_js-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cwargnier   (501) staff       (20)        0 2024-04-01 13:27:53.302623 streamlit_chart_js-0.0.5/
--rw-r--r--   0 cwargnier   (501) staff       (20)        0 2024-03-28 18:07:16.000000 streamlit_chart_js-0.0.5/MANIFEST.in
--rw-r--r--   0 cwargnier   (501) staff       (20)     8351 2024-04-01 13:27:53.301629 streamlit_chart_js-0.0.5/PKG-INFO
--rw-r--r--   0 cwargnier   (501) staff       (20)     7940 2024-03-30 21:44:31.000000 streamlit_chart_js-0.0.5/README.md
--rw-r--r--   0 cwargnier   (501) staff       (20)       38 2024-04-01 13:27:53.302836 streamlit_chart_js-0.0.5/setup.cfg
--rw-r--r--   0 cwargnier   (501) staff       (20)      666 2024-04-01 13:27:22.000000 streamlit_chart_js-0.0.5/setup.py
-drwxr-xr-x   0 cwargnier   (501) staff       (20)        0 2024-04-01 13:27:53.297728 streamlit_chart_js-0.0.5/streamlit_chart_js.egg-info/
--rw-r--r--   0 cwargnier   (501) staff       (20)     8351 2024-04-01 13:27:53.000000 streamlit_chart_js-0.0.5/streamlit_chart_js.egg-info/PKG-INFO
--rw-r--r--   0 cwargnier   (501) staff       (20)      309 2024-04-01 13:27:53.000000 streamlit_chart_js-0.0.5/streamlit_chart_js.egg-info/SOURCES.txt
--rw-r--r--   0 cwargnier   (501) staff       (20)        1 2024-04-01 13:27:53.000000 streamlit_chart_js-0.0.5/streamlit_chart_js.egg-info/dependency_links.txt
--rw-r--r--   0 cwargnier   (501) staff       (20)       10 2024-04-01 13:27:53.000000 streamlit_chart_js-0.0.5/streamlit_chart_js.egg-info/requires.txt
--rw-r--r--   0 cwargnier   (501) staff       (20)       18 2024-04-01 13:27:53.000000 streamlit_chart_js-0.0.5/streamlit_chart_js.egg-info/top_level.txt
-drwxr-xr-x   0 cwargnier   (501) staff       (20)        0 2024-04-01 13:27:53.300508 streamlit_chart_js-0.0.5/streamlit_chartjs/
--rw-r--r--   0 cwargnier   (501) staff       (20)        0 2024-03-28 18:07:16.000000 streamlit_chart_js-0.0.5/streamlit_chartjs/__init__.py
--rw-r--r--   0 cwargnier   (501) staff       (20)     2673 2024-04-01 10:11:37.000000 streamlit_chart_js-0.0.5/streamlit_chartjs/st_chart_component.py
+drwxr-xr-x   0 cwargnier   (501) staff       (20)        0 2024-04-01 13:49:52.406656 streamlit_chart_js-0.0.6/
+-rw-r--r--   0 cwargnier   (501) staff       (20)        0 2024-03-28 18:07:16.000000 streamlit_chart_js-0.0.6/MANIFEST.in
+-rw-r--r--   0 cwargnier   (501) staff       (20)    12747 2024-04-01 13:49:52.406146 streamlit_chart_js-0.0.6/PKG-INFO
+-rw-r--r--   0 cwargnier   (501) staff       (20)    12320 2024-04-01 13:47:22.000000 streamlit_chart_js-0.0.6/README.md
+-rw-r--r--   0 cwargnier   (501) staff       (20)       38 2024-04-01 13:49:52.406820 streamlit_chart_js-0.0.6/setup.cfg
+-rw-r--r--   0 cwargnier   (501) staff       (20)      682 2024-04-01 13:48:50.000000 streamlit_chart_js-0.0.6/setup.py
+drwxr-xr-x   0 cwargnier   (501) staff       (20)        0 2024-04-01 13:49:52.401547 streamlit_chart_js-0.0.6/streamlit_chart_js.egg-info/
+-rw-r--r--   0 cwargnier   (501) staff       (20)    12747 2024-04-01 13:49:52.000000 streamlit_chart_js-0.0.6/streamlit_chart_js.egg-info/PKG-INFO
+-rw-r--r--   0 cwargnier   (501) staff       (20)      309 2024-04-01 13:49:52.000000 streamlit_chart_js-0.0.6/streamlit_chart_js.egg-info/SOURCES.txt
+-rw-r--r--   0 cwargnier   (501) staff       (20)        1 2024-04-01 13:49:52.000000 streamlit_chart_js-0.0.6/streamlit_chart_js.egg-info/dependency_links.txt
+-rw-r--r--   0 cwargnier   (501) staff       (20)       10 2024-04-01 13:49:52.000000 streamlit_chart_js-0.0.6/streamlit_chart_js.egg-info/requires.txt
+-rw-r--r--   0 cwargnier   (501) staff       (20)       18 2024-04-01 13:49:52.000000 streamlit_chart_js-0.0.6/streamlit_chart_js.egg-info/top_level.txt
+drwxr-xr-x   0 cwargnier   (501) staff       (20)        0 2024-04-01 13:49:52.404445 streamlit_chart_js-0.0.6/streamlit_chartjs/
+-rw-r--r--   0 cwargnier   (501) staff       (20)        0 2024-03-28 18:07:16.000000 streamlit_chart_js-0.0.6/streamlit_chartjs/__init__.py
+-rw-r--r--   0 cwargnier   (501) staff       (20)     2673 2024-04-01 10:11:37.000000 streamlit_chart_js-0.0.6/streamlit_chartjs/st_chart_component.py
```

### Comparing `streamlit_chart_js-0.0.5/setup.py` & `streamlit_chart_js-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="streamlit_chart_js",
-    version="0.0.5",
+    version="0.0.6",
     author="Charly Wargnier",
     author_email="cwar05@gnail.com",
-    description="A custom Streamlit component for Chart.js",
+    description="A custom component to render Chart.js charts in Streamlit",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "streamlit",
         # Any other dependencies your component needs
```

### Comparing `streamlit_chart_js-0.0.5/streamlit_chartjs/st_chart_component.py` & `streamlit_chart_js-0.0.6/streamlit_chartjs/st_chart_component.py`

 * *Files identical despite different names*

