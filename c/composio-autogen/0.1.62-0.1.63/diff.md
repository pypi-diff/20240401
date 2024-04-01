# Comparing `tmp/composio_autogen-0.1.62.tar.gz` & `tmp/composio_autogen-0.1.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.1.62.tar", last modified: Sun Mar 31 17:29:47 2024, max compression
+gzip compressed data, was "composio_autogen-0.1.63.tar", last modified: Mon Apr  1 14:15:12 2024, max compression
```

## Comparing `composio_autogen-0.1.62.tar` & `composio_autogen-0.1.63.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-03-31 17:29:47.297396 composio_autogen-0.1.62/
--rw-r--r--   0 utkarsh    (501) staff       (20)      661 2024-03-31 17:29:47.297212 composio_autogen-0.1.62/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      128 2024-03-20 12:04:29.000000 composio_autogen-0.1.62/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-03-31 17:29:47.296113 composio_autogen-0.1.62/composio_autogen/
--rw-r--r--   0 utkarsh    (501) staff       (20)       79 2024-03-21 07:30:14.000000 composio_autogen-0.1.62/composio_autogen/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     6977 2024-03-27 14:52:24.000000 composio_autogen-0.1.62/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-03-31 17:29:47.297014 composio_autogen-0.1.62/composio_autogen.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      661 2024-03-31 17:29:47.000000 composio_autogen-0.1.62/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-03-31 17:29:47.000000 composio_autogen-0.1.62/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-03-31 17:29:47.000000 composio_autogen-0.1.62/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       42 2024-03-31 17:29:47.000000 composio_autogen-0.1.62/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-03-31 17:29:47.000000 composio_autogen-0.1.62/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-03-31 17:27:52.000000 composio_autogen-0.1.62/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-03-31 17:29:47.297442 composio_autogen-0.1.62/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      841 2024-03-31 17:27:52.000000 composio_autogen-0.1.62/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-01 14:15:12.477454 composio_autogen-0.1.63/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      661 2024-04-01 14:15:12.477198 composio_autogen-0.1.63/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      128 2024-03-20 12:04:29.000000 composio_autogen-0.1.63/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-01 14:15:12.475854 composio_autogen-0.1.63/composio_autogen/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       79 2024-03-21 07:30:14.000000 composio_autogen-0.1.63/composio_autogen/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     6977 2024-03-27 14:52:24.000000 composio_autogen-0.1.63/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-01 14:15:12.476917 composio_autogen-0.1.63/composio_autogen.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      661 2024-04-01 14:15:12.000000 composio_autogen-0.1.63/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-01 14:15:12.000000 composio_autogen-0.1.63/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-01 14:15:12.000000 composio_autogen-0.1.63/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       42 2024-04-01 14:15:12.000000 composio_autogen-0.1.63/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-01 14:15:12.000000 composio_autogen-0.1.63/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-04-01 14:14:25.000000 composio_autogen-0.1.63/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-01 14:15:12.477503 composio_autogen-0.1.63/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      841 2024-04-01 14:14:25.000000 composio_autogen-0.1.63/setup.py
```

### Comparing `composio_autogen-0.1.62/PKG-INFO` & `composio_autogen-0.1.63/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.62
+Version: 0.1.63
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.62
+Requires-Dist: composio_core===0.1.63
 Requires-Dist: pyautogen===0.2.19
 
 Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 # Usage
 Within your Autogen project:
```

### Comparing `composio_autogen-0.1.62/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.1.63/composio_autogen/autogen_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.62/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.1.63/composio_autogen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.62
+Version: 0.1.63
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.62
+Requires-Dist: composio_core===0.1.63
 Requires-Dist: pyautogen===0.2.19
 
 Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 # Usage
 Within your Autogen project:
```

### Comparing `composio_autogen-0.1.62/setup.py` & `composio_autogen-0.1.63/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.1.62",
+    version="0.1.63",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

