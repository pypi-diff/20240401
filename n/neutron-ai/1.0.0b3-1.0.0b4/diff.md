# Comparing `tmp/neutron-ai-1.0.0b3.tar.gz` & `tmp/neutron-ai-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neutron-ai-1.0.0b3.tar", last modified: Wed Mar 20 14:58:07 2024, max compression
+gzip compressed data, was "neutron-ai-1.0.0b4.tar", last modified: Mon Apr  1 20:39:54 2024, max compression
```

## Comparing `neutron-ai-1.0.0b3.tar` & `neutron-ai-1.0.0b4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:58:07.677354 neutron-ai-1.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-20 14:57:44.000000 neutron-ai-1.0.0b3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-03-20 14:58:07.677354 neutron-ai-1.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-03-20 14:57:44.000000 neutron-ai-1.0.0b3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-20 14:57:44.000000 neutron-ai-1.0.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 14:58:07.677354 neutron-ai-1.0.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-20 14:58:01.000000 neutron-ai-1.0.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:58:07.673354 neutron-ai-1.0.0b3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:58:07.677354 neutron-ai-1.0.0b3/src/neutron/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 14:57:44.000000 neutron-ai-1.0.0b3/src/neutron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-20 14:57:44.000000 neutron-ai-1.0.0b3/src/neutron/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-03-20 14:57:44.000000 neutron-ai-1.0.0b3/src/neutron/interactive_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-03-20 14:57:44.000000 neutron-ai-1.0.0b3/src/neutron/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-03-20 14:57:44.000000 neutron-ai-1.0.0b3/src/neutron/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:58:07.677354 neutron-ai-1.0.0b3/src/neutron_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-03-20 14:58:07.000000 neutron-ai-1.0.0b3/src/neutron_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-20 14:58:07.000000 neutron-ai-1.0.0b3/src/neutron_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 14:58:07.000000 neutron-ai-1.0.0b3/src/neutron_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-20 14:58:07.000000 neutron-ai-1.0.0b3/src/neutron_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-20 14:58:07.000000 neutron-ai-1.0.0b3/src/neutron_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-20 14:58:07.000000 neutron-ai-1.0.0b3/src/neutron_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:39:54.489673 neutron-ai-1.0.0b4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-01 20:39:36.000000 neutron-ai-1.0.0b4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-01 20:39:54.489673 neutron-ai-1.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-01 20:39:36.000000 neutron-ai-1.0.0b4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-01 20:39:36.000000 neutron-ai-1.0.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:39:54.489673 neutron-ai-1.0.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-01 20:39:47.000000 neutron-ai-1.0.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:39:54.485673 neutron-ai-1.0.0b4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:39:54.485673 neutron-ai-1.0.0b4/src/neutron/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:39:36.000000 neutron-ai-1.0.0b4/src/neutron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-01 20:39:36.000000 neutron-ai-1.0.0b4/src/neutron/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-01 20:39:36.000000 neutron-ai-1.0.0b4/src/neutron/interactive_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-01 20:39:36.000000 neutron-ai-1.0.0b4/src/neutron/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-01 20:39:36.000000 neutron-ai-1.0.0b4/src/neutron/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:39:54.489673 neutron-ai-1.0.0b4/src/neutron_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-01 20:39:54.000000 neutron-ai-1.0.0b4/src/neutron_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-01 20:39:54.000000 neutron-ai-1.0.0b4/src/neutron_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:39:54.000000 neutron-ai-1.0.0b4/src/neutron_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 20:39:54.000000 neutron-ai-1.0.0b4/src/neutron_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 20:39:54.000000 neutron-ai-1.0.0b4/src/neutron_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 20:39:54.000000 neutron-ai-1.0.0b4/src/neutron_ai.egg-info/top_level.txt
```

### Comparing `neutron-ai-1.0.0b3/LICENSE.md` & `neutron-ai-1.0.0b4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neutron-ai-1.0.0b3/PKG-INFO` & `neutron-ai-1.0.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neutron-ai
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: AI Powered Ethical Hacking Assistant
 Home-page: https://github.com/berylliumsec/neutron
 Author: David I
 Author-email: david@berylliumsec.com
 License: BSD
 Keywords: AI,Ethical Hacking
 Classifier: Development Status :: 4 - Beta
@@ -54,35 +54,36 @@
 
 🚀 We're thrilled to unveil a sneak peek of Nebula Pro, our latest innovation designed to empower ethical hackers with advanced, AI-driven capabilities. After months of dedicated development, we have launched the preview version. Some of the exciting features are:
 
 - AI Powered Autonomous Mode
 - AI Powered Suggestions
 - AI Powered Note Taking
 
-**Neutron will become a part of Nebula Pro's free tier**
+**Neutron is now a part of Nebula Pro's free tier**
 # 📺 [Click Here to Get Access To Nebula Pro Now](https://www.berylliumsec.com/nebula-pro-waitlist) 🚀
 
 
 
 ## Why Neutron?
 
 The purpose of Neutron is straightforward: to provide security professionals  with access to a free AI assistant that can be invoked directly from their command line interface. It was built as part of the free tier of [Nebula Pro](https://www.berylliumsec.com/nebula-pro-waitlist).
 
+
 ## [Click Here to Watch Neutron in Action](https://youtu.be/v5X8TNPsMbM)
 
 
 ## Compatibility
 
 Neutron has been extensively tested and optimized for Linux platforms. As of now, its functionality on Windows or macOS is not guaranteed, and it may not operate as expected.
 
 ## System dependencies
 
 - Storage: A minimum of 50GB is recommended.
 
-- RAM: A minimum of 16GB RAM memory is recommended.
+- RAM: A minimum of 32GB RAM memory is recommended.
 
 - Graphics Processing Unit (GPU) (NOT MANDATORY, Neutron can run on CPU): While not mandatory, having at least 24GB of GPU memory is recommended for optimal performance.
 
 
 **PYPI based distribution requirement(s)**
 
 - Python3: Version 3.10 or later is required for compatibility with all used libraries.
@@ -162,17 +163,18 @@
 ```
 
 
 To use Neutron AI directly from the command line using a shorter alias for example AN, add the following function to your .bashrc or .zshrc:
 
 ```bash
 function AN() {
-    local query=\"$*\"
-    neutron-client \"\$query\"
+    local query="$*"
+    neutron-client "$query"
 }
+
 ```
 After adding, restart your terminal or run 'source ~/.bashrc' (or 'source ~/.zshrc') to apply the changes.
 
 Then after starting the server, you can ask your questions like so:
 
 ```bash
 AN your question
```

### Comparing `neutron-ai-1.0.0b3/README.md` & `neutron-ai-1.0.0b4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,35 +27,36 @@
 
 🚀 We're thrilled to unveil a sneak peek of Nebula Pro, our latest innovation designed to empower ethical hackers with advanced, AI-driven capabilities. After months of dedicated development, we have launched the preview version. Some of the exciting features are:
 
 - AI Powered Autonomous Mode
 - AI Powered Suggestions
 - AI Powered Note Taking
 
-**Neutron will become a part of Nebula Pro's free tier**
+**Neutron is now a part of Nebula Pro's free tier**
 # 📺 [Click Here to Get Access To Nebula Pro Now](https://www.berylliumsec.com/nebula-pro-waitlist) 🚀
 
 
 
 ## Why Neutron?
 
 The purpose of Neutron is straightforward: to provide security professionals  with access to a free AI assistant that can be invoked directly from their command line interface. It was built as part of the free tier of [Nebula Pro](https://www.berylliumsec.com/nebula-pro-waitlist).
 
+
 ## [Click Here to Watch Neutron in Action](https://youtu.be/v5X8TNPsMbM)
 
 
 ## Compatibility
 
 Neutron has been extensively tested and optimized for Linux platforms. As of now, its functionality on Windows or macOS is not guaranteed, and it may not operate as expected.
 
 ## System dependencies
 
 - Storage: A minimum of 50GB is recommended.
 
-- RAM: A minimum of 16GB RAM memory is recommended.
+- RAM: A minimum of 32GB RAM memory is recommended.
 
 - Graphics Processing Unit (GPU) (NOT MANDATORY, Neutron can run on CPU): While not mandatory, having at least 24GB of GPU memory is recommended for optimal performance.
 
 
 **PYPI based distribution requirement(s)**
 
 - Python3: Version 3.10 or later is required for compatibility with all used libraries.
@@ -135,17 +136,18 @@
 ```
 
 
 To use Neutron AI directly from the command line using a shorter alias for example AN, add the following function to your .bashrc or .zshrc:
 
 ```bash
 function AN() {
-    local query=\"$*\"
-    neutron-client \"\$query\"
+    local query="$*"
+    neutron-client "$query"
 }
+
 ```
 After adding, restart your terminal or run 'source ~/.bashrc' (or 'source ~/.zshrc') to apply the changes.
 
 Then after starting the server, you can ask your questions like so:
 
 ```bash
 AN your question
@@ -153,8 +155,8 @@
 
 ### Authentication
 
 To use a password for the server and client simply add it to your ENVs before you run the server and the client like so:
 
 ```bash
 export NEUTRON_TOKEN="YOUR_SECRET"
-```
+```
```

### Comparing `neutron-ai-1.0.0b3/setup.py` & `neutron-ai-1.0.0b4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="neutron-ai",
-    version="1.0.0b3",
+    version="1.0.0b4",
     description="AI Powered Ethical Hacking Assistant",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="David I",
     author_email="david@berylliumsec.com",
     url="https://github.com/berylliumsec/neutron",
     classifiers=[
```

### Comparing `neutron-ai-1.0.0b3/src/neutron/client.py` & `neutron-ai-1.0.0b4/src/neutron/client.py`

 * *Files identical despite different names*

### Comparing `neutron-ai-1.0.0b3/src/neutron/interactive_model.py` & `neutron-ai-1.0.0b4/src/neutron/interactive_model.py`

 * *Files identical despite different names*

### Comparing `neutron-ai-1.0.0b3/src/neutron/server.py` & `neutron-ai-1.0.0b4/src/neutron/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 # Get the process info using psutil
 process = psutil.Process(pid)
 # Get memory usage (in bytes)
 memory_use = process.memory_info().rss
 memory_use_gb = memory_use / 1024 / 1024 / 1024
 print(f"Memory used by Neutron: {memory_use_gb} GB")
 print(
-    "Embrace the future of AI Powered Ethical Hacking with Nebula Pro ->> https://www.berylliumsec.com/nebula-pro-waitlist "
+    "Neutron is now part of Nebula Pro's Free Tier.\nEmbrace the future of AI Powered Ethical Hacking with Nebula Pro ->> https://www.berylliumsec.com/nebula-pro-waitlist "
 )
 
 
 def check_auth(token: str) -> bool:
     """This function is called to check if a given token is valid."""
     # Retrieve the secret token from the NEUTRON_TOKEN environment variable
     secret_token = os.environ.get(
```

### Comparing `neutron-ai-1.0.0b3/src/neutron/utilities.py` & `neutron-ai-1.0.0b4/src/neutron/utilities.py`

 * *Files identical despite different names*

### Comparing `neutron-ai-1.0.0b3/src/neutron_ai.egg-info/PKG-INFO` & `neutron-ai-1.0.0b4/src/neutron_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neutron-ai
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: AI Powered Ethical Hacking Assistant
 Home-page: https://github.com/berylliumsec/neutron
 Author: David I
 Author-email: david@berylliumsec.com
 License: BSD
 Keywords: AI,Ethical Hacking
 Classifier: Development Status :: 4 - Beta
@@ -54,35 +54,36 @@
 
 🚀 We're thrilled to unveil a sneak peek of Nebula Pro, our latest innovation designed to empower ethical hackers with advanced, AI-driven capabilities. After months of dedicated development, we have launched the preview version. Some of the exciting features are:
 
 - AI Powered Autonomous Mode
 - AI Powered Suggestions
 - AI Powered Note Taking
 
-**Neutron will become a part of Nebula Pro's free tier**
+**Neutron is now a part of Nebula Pro's free tier**
 # 📺 [Click Here to Get Access To Nebula Pro Now](https://www.berylliumsec.com/nebula-pro-waitlist) 🚀
 
 
 
 ## Why Neutron?
 
 The purpose of Neutron is straightforward: to provide security professionals  with access to a free AI assistant that can be invoked directly from their command line interface. It was built as part of the free tier of [Nebula Pro](https://www.berylliumsec.com/nebula-pro-waitlist).
 
+
 ## [Click Here to Watch Neutron in Action](https://youtu.be/v5X8TNPsMbM)
 
 
 ## Compatibility
 
 Neutron has been extensively tested and optimized for Linux platforms. As of now, its functionality on Windows or macOS is not guaranteed, and it may not operate as expected.
 
 ## System dependencies
 
 - Storage: A minimum of 50GB is recommended.
 
-- RAM: A minimum of 16GB RAM memory is recommended.
+- RAM: A minimum of 32GB RAM memory is recommended.
 
 - Graphics Processing Unit (GPU) (NOT MANDATORY, Neutron can run on CPU): While not mandatory, having at least 24GB of GPU memory is recommended for optimal performance.
 
 
 **PYPI based distribution requirement(s)**
 
 - Python3: Version 3.10 or later is required for compatibility with all used libraries.
@@ -162,17 +163,18 @@
 ```
 
 
 To use Neutron AI directly from the command line using a shorter alias for example AN, add the following function to your .bashrc or .zshrc:
 
 ```bash
 function AN() {
-    local query=\"$*\"
-    neutron-client \"\$query\"
+    local query="$*"
+    neutron-client "$query"
 }
+
 ```
 After adding, restart your terminal or run 'source ~/.bashrc' (or 'source ~/.zshrc') to apply the changes.
 
 Then after starting the server, you can ask your questions like so:
 
 ```bash
 AN your question
```

