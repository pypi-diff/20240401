# Comparing `tmp/python_arq-6.0.6.tar.gz` & `tmp/python_arq-6.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_arq-6.0.6.tar", last modified: Sat Mar 30 06:29:45 2024, max compression
+gzip compressed data, was "python_arq-6.0.7.tar", last modified: Mon Apr  1 18:34:02 2024, max compression
```

## Comparing `python_arq-6.0.6.tar` & `python_arq-6.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hamker    (1000) hamker    (1000)        0 2024-03-30 06:29:45.007933 python_arq-6.0.6/
--rw-r--r--   0 hamker    (1000) hamker    (1000)     1069 2024-03-30 06:21:29.000000 python_arq-6.0.6/LICENSE
--rw-r--r--   0 hamker    (1000) hamker    (1000)     2348 2024-03-30 06:29:45.007933 python_arq-6.0.6/PKG-INFO
-drwxr-xr-x   0 hamker    (1000) hamker    (1000)        0 2024-03-30 06:29:45.007933 python_arq-6.0.6/Python_ARQ/
--rw-r--r--   0 hamker    (1000) hamker    (1000)      160 2024-03-30 06:21:29.000000 python_arq-6.0.6/Python_ARQ/__init__.py
--rw-r--r--   0 hamker    (1000) hamker    (1000)    19950 2024-03-30 06:23:35.000000 python_arq-6.0.6/Python_ARQ/arq.py
--rw-r--r--   0 hamker    (1000) hamker    (1000)     1667 2024-03-30 06:21:29.000000 python_arq-6.0.6/README.md
-drwxr-xr-x   0 hamker    (1000) hamker    (1000)        0 2024-03-30 06:29:45.007933 python_arq-6.0.6/python_arq.egg-info/
--rw-r--r--   0 hamker    (1000) hamker    (1000)     2348 2024-03-30 06:29:44.000000 python_arq-6.0.6/python_arq.egg-info/PKG-INFO
--rw-r--r--   0 hamker    (1000) hamker    (1000)      236 2024-03-30 06:29:44.000000 python_arq-6.0.6/python_arq.egg-info/SOURCES.txt
--rw-r--r--   0 hamker    (1000) hamker    (1000)        1 2024-03-30 06:29:44.000000 python_arq-6.0.6/python_arq.egg-info/dependency_links.txt
--rw-r--r--   0 hamker    (1000) hamker    (1000)       33 2024-03-30 06:29:44.000000 python_arq-6.0.6/python_arq.egg-info/requires.txt
--rw-r--r--   0 hamker    (1000) hamker    (1000)       11 2024-03-30 06:29:44.000000 python_arq-6.0.6/python_arq.egg-info/top_level.txt
--rw-r--r--   0 hamker    (1000) hamker    (1000)       38 2024-03-30 06:29:45.007933 python_arq-6.0.6/setup.cfg
--rw-r--r--   0 hamker    (1000) hamker    (1000)     1000 2024-03-30 06:28:42.000000 python_arq-6.0.6/setup.py
+drwxr-xr-x   0 hamker    (1000) hamker    (1000)        0 2024-04-01 18:34:02.662148 python_arq-6.0.7/
+-rw-r--r--   0 hamker    (1000) hamker    (1000)     1069 2024-03-30 06:21:29.000000 python_arq-6.0.7/LICENSE
+-rw-r--r--   0 hamker    (1000) hamker    (1000)     2348 2024-04-01 18:34:02.662148 python_arq-6.0.7/PKG-INFO
+drwxr-xr-x   0 hamker    (1000) hamker    (1000)        0 2024-04-01 18:34:02.662148 python_arq-6.0.7/Python_ARQ/
+-rw-r--r--   0 hamker    (1000) hamker    (1000)      160 2024-03-30 06:21:29.000000 python_arq-6.0.7/Python_ARQ/__init__.py
+-rw-r--r--   0 hamker    (1000) hamker    (1000)    19949 2024-04-01 18:33:28.000000 python_arq-6.0.7/Python_ARQ/arq.py
+-rw-r--r--   0 hamker    (1000) hamker    (1000)     1667 2024-03-30 06:21:29.000000 python_arq-6.0.7/README.md
+drwxr-xr-x   0 hamker    (1000) hamker    (1000)        0 2024-04-01 18:34:02.662148 python_arq-6.0.7/python_arq.egg-info/
+-rw-r--r--   0 hamker    (1000) hamker    (1000)     2348 2024-04-01 18:34:02.000000 python_arq-6.0.7/python_arq.egg-info/PKG-INFO
+-rw-r--r--   0 hamker    (1000) hamker    (1000)      236 2024-04-01 18:34:02.000000 python_arq-6.0.7/python_arq.egg-info/SOURCES.txt
+-rw-r--r--   0 hamker    (1000) hamker    (1000)        1 2024-04-01 18:34:02.000000 python_arq-6.0.7/python_arq.egg-info/dependency_links.txt
+-rw-r--r--   0 hamker    (1000) hamker    (1000)       33 2024-04-01 18:34:02.000000 python_arq-6.0.7/python_arq.egg-info/requires.txt
+-rw-r--r--   0 hamker    (1000) hamker    (1000)       11 2024-04-01 18:34:02.000000 python_arq-6.0.7/python_arq.egg-info/top_level.txt
+-rw-r--r--   0 hamker    (1000) hamker    (1000)       38 2024-04-01 18:34:02.662148 python_arq-6.0.7/setup.cfg
+-rw-r--r--   0 hamker    (1000) hamker    (1000)     1000 2024-04-01 18:33:35.000000 python_arq-6.0.7/setup.py
```

### Comparing `python_arq-6.0.6/LICENSE` & `python_arq-6.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_arq-6.0.6/PKG-INFO` & `python_arq-6.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_arq
-Version: 6.0.6
+Version: 6.0.7
 Summary: Asynchronous Python Wrapper For A.R.Q API.
 Home-page: https://github.com/thehamkercat/Python_ARQ
 Author: TheHamkerCat
 Author-email: thehamkercat@gmail.com
 License: MIT
 Keywords: API,ARQ_API,Python-ARQ,ARQ,A.R.Q
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python_arq-6.0.6/Python_ARQ/arq.py` & `python_arq-6.0.7/Python_ARQ/arq.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,16 +340,16 @@
                         Result object (str): Results which you can access with dot notation
 
                         results
         """
         if not isinstance(messages, list):
             messages = [messages]
 
-        def typeToStr(pyrogrma_type):
-            return str(pyrogrma_type).split(".")[-1].loower()
+        def typeToStr(pyrogram_type):
+            return str(pyrogram_type).split(".")[-1].lower()
 
         payload = {
             "type": "quote",
             "format": "png",
             "backgroundColor": "#1b1429",
             "messages": [
                 {
```

### Comparing `python_arq-6.0.6/README.md` & `python_arq-6.0.7/README.md`

 * *Files identical despite different names*

### Comparing `python_arq-6.0.6/python_arq.egg-info/PKG-INFO` & `python_arq-6.0.7/python_arq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_arq
-Version: 6.0.6
+Version: 6.0.7
 Summary: Asynchronous Python Wrapper For A.R.Q API.
 Home-page: https://github.com/thehamkercat/Python_ARQ
 Author: TheHamkerCat
 Author-email: thehamkercat@gmail.com
 License: MIT
 Keywords: API,ARQ_API,Python-ARQ,ARQ,A.R.Q
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python_arq-6.0.6/setup.py` & `python_arq-6.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ) as requirements:
     long_description = readme.read()
     requires = requirements.read().splitlines(keepends=False)
 
 setuptools.setup(
     name="python_arq",
     packages=setuptools.find_packages(),
-    version="6.0.6",
+    version="6.0.7",
     license="MIT",
     description="Asynchronous Python Wrapper For A.R.Q API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="TheHamkerCat",
     author_email="thehamkercat@gmail.com",
     url="https://github.com/thehamkercat/Python_ARQ",
```

