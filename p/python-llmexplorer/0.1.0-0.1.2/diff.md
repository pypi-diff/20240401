# Comparing `tmp/python-llmexplorer-0.1.0.tar.gz` & `tmp/python-llmexplorer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-llmexplorer-0.1.0.tar", last modified: Fri Mar 15 19:59:26 2024, max compression
+gzip compressed data, was "python-llmexplorer-0.1.2.tar", last modified: Mon Apr  1 19:41:15 2024, max compression
```

## Comparing `python-llmexplorer-0.1.0.tar` & `python-llmexplorer-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 19:59:26.098989 python-llmexplorer-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      906 2024-03-15 19:59:26.098989 python-llmexplorer-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      108 2024-02-21 13:37:59.000000 python-llmexplorer-0.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)      646 2024-03-15 18:20:14.000000 python-llmexplorer-0.1.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 19:59:26.098989 python-llmexplorer-0.1.0/python_llmexplorer.egg-info/
--rw-r--r--   0 root         (0) root         (0)      906 2024-03-15 19:59:26.000000 python-llmexplorer-0.1.0/python_llmexplorer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-03-15 19:59:26.000000 python-llmexplorer-0.1.0/python_llmexplorer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-15 19:59:26.000000 python-llmexplorer-0.1.0/python_llmexplorer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-03-15 19:59:26.000000 python-llmexplorer-0.1.0/python_llmexplorer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-15 19:59:26.000000 python-llmexplorer-0.1.0/python_llmexplorer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-15 19:59:26.098989 python-llmexplorer-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1425 2024-03-15 19:58:46.000000 python-llmexplorer-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:15.842109 python-llmexplorer-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)      906 2024-04-01 19:41:15.842109 python-llmexplorer-0.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      108 2024-02-21 13:37:59.000000 python-llmexplorer-0.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      653 2024-03-15 20:04:25.000000 python-llmexplorer-0.1.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:15.842109 python-llmexplorer-0.1.2/python_llmexplorer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      906 2024-04-01 19:41:15.000000 python-llmexplorer-0.1.2/python_llmexplorer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-04-01 19:41:15.000000 python-llmexplorer-0.1.2/python_llmexplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 19:41:15.000000 python-llmexplorer-0.1.2/python_llmexplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-01 19:41:15.000000 python-llmexplorer-0.1.2/python_llmexplorer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 19:41:15.000000 python-llmexplorer-0.1.2/python_llmexplorer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-01 19:41:15.842109 python-llmexplorer-0.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1425 2024-04-01 19:41:01.000000 python-llmexplorer-0.1.2/setup.py
```

### Comparing `python-llmexplorer-0.1.0/PKG-INFO` & `python-llmexplorer-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-llmexplorer
-Version: 0.1.0
+Version: 0.1.2
 Summary: A Tool that can be used to analyse, monitor prompts usage and LLM ops
 Home-page: https://github.com/9throok/LLMExplorer
 Author: The LLM Explorer Team
 Author-email: 
 License: MIT
 Description: # LLMExplorer
         Welcome to LLMExplorer. A Tool that can be used to analyse, monitor prompts usage and LLM ops
```

### Comparing `python-llmexplorer-0.1.0/pyproject.toml` & `python-llmexplorer-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
-name = "llmexplorer"
+name = "python-llmexplorer"
 version = "0.1.0"
 description = "A Tool that can be used to analyse, monitor prompts usage and LLM ops"
 authors = ["The LLM Explorer Team"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.6"
```

### Comparing `python-llmexplorer-0.1.0/python_llmexplorer.egg-info/PKG-INFO` & `python-llmexplorer-0.1.2/python_llmexplorer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-llmexplorer
-Version: 0.1.0
+Version: 0.1.2
 Summary: A Tool that can be used to analyse, monitor prompts usage and LLM ops
 Home-page: https://github.com/9throok/LLMExplorer
 Author: The LLM Explorer Team
 Author-email: 
 License: MIT
 Description: # LLMExplorer
         Welcome to LLMExplorer. A Tool that can be used to analyse, monitor prompts usage and LLM ops
```

### Comparing `python-llmexplorer-0.1.0/setup.py` & `python-llmexplorer-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 # Package metadata
 NAME = 'python-llmexplorer'
-VERSION = '0.1.0'
+VERSION = '0.1.2'
 DESCRIPTION = 'A Tool that can be used to analyse, monitor prompts usage and LLM ops'
 URL = 'https://github.com/9throok/LLMExplorer'
 AUTHOR = 'The LLM Explorer Team'
 EMAIL = ''
 LICENSE = 'MIT'
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
```

