# Comparing `tmp/froggius-0.1.3.tar.gz` & `tmp/froggius-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "froggius-0.1.3.tar", last modified: Mon Apr  1 09:12:55 2024, max compression
+gzip compressed data, was "froggius-0.1.4.tar", last modified: Mon Apr  1 09:29:27 2024, max compression
```

## Comparing `froggius-0.1.3.tar` & `froggius-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:12:55.408937 froggius-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 09:12:51.000000 froggius-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-01 09:12:55.408937 froggius-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-01 09:12:51.000000 froggius-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:12:55.408937 froggius-0.1.3/froggius/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:12:51.000000 froggius-0.1.3/froggius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-01 09:12:51.000000 froggius-0.1.3/froggius/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:12:55.408937 froggius-0.1.3/froggius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-01 09:12:55.000000 froggius-0.1.3/froggius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 09:12:55.000000 froggius-0.1.3/froggius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 09:12:55.000000 froggius-0.1.3/froggius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 09:12:55.000000 froggius-0.1.3/froggius.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 09:12:55.408937 froggius-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-01 09:12:51.000000 froggius-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:29:27.973330 froggius-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 09:29:17.000000 froggius-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-01 09:29:27.973330 froggius-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-01 09:29:17.000000 froggius-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:29:27.973330 froggius-0.1.4/froggius/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:29:17.000000 froggius-0.1.4/froggius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-01 09:29:25.000000 froggius-0.1.4/froggius/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:29:27.973330 froggius-0.1.4/froggius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-01 09:29:27.000000 froggius-0.1.4/froggius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 09:29:27.000000 froggius-0.1.4/froggius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 09:29:27.000000 froggius-0.1.4/froggius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 09:29:27.000000 froggius-0.1.4/froggius.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 09:29:27.973330 froggius-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-01 09:29:25.000000 froggius-0.1.4/setup.py
```

### Comparing `froggius-0.1.3/LICENSE` & `froggius-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `froggius-0.1.3/README.md` & `froggius-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `froggius-0.1.3/froggius/logger.py` & `froggius-0.1.4/froggius/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 Froggius
-Version: v0.1.2
+Version: v0.1.4
 License: GPLv3
 
 Author of this file: zlElo
 """
 
 import datetime
 import sys
 import traceback
 
-class Froggius():
+
+class Froggius:
     """
     Main class of Froggius
     Includes logging methods
     """
+
     def debug(log_msg, file_path=None, highliting=True, print_out=True):
         """
         Writes logs, optionally to a file.
 
         Parameters
         ----------
         log_msg : str
@@ -35,20 +37,24 @@
         str
             The log string if print_out is set to False
         """
         current_date = datetime.datetime.now()
         if highliting:
             log_string = f'\033[92m[DBG]\033[0m [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
         else:
-            log_string = f'[DBG] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
+            log_string = (
+                f'[DBG] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
+            )
 
         # check for filepath
         if file_path is not None:
-            with open(file_path, 'a') as log:
-                log.write(f'\n[DBG] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}')
+            with open(file_path, "a") as log:
+                log.write(
+                    f'\n[DBG] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
+                )
 
         if print_out:
             print(log_string, file=sys.stdout)
         else:
             return log_string
 
     def error(log_msg, file_path=None, highlighting=True, print_out=True, line=None):
@@ -82,43 +88,53 @@
         if highlighting == True:
             log_string = f'[\033[91mERR\033[0m] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg} {f"| Occured on line: {line[0]} in {line[1]}, {line[2]}()" if line is not None else ""}'
         else:
             log_string = f'[ERR] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg} {f"| Occured on line: {line[0]} in {line[1]}, {line[2]}()" if line is not None else ""}'
 
         # check for filepath
         if file_path is not None:
-            with open(file_path, 'a') as log:
-                log.write(f'\n[ERR] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg} {f"| Occured on line: {line[0]} in {line[1]}, {line[2]}()" if line is not None else ""}')
+            with open(file_path, "a") as log:
+                log.write(
+                    f'\n[ERR] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg} {f"| Occured on line: {line[0]} in {line[1]}, {line[2]}()" if line is not None else ""}'
+                )
 
         if print_out == True:
             print(log_string, file=sys.stdout)
         else:
             return log_string
-    
+
     @staticmethod
     def catch(file_path=None):
         """
         A decorator that catches exceptions and logs them with LogMx.error
 
         Parameters
         ----------
         file_path : str, optional
 
         Returns
         -------
         decorator
         """
+
         def decorator(func):
             def wrapper(*args, **kwargs):
                 try:
                     return func(*args, **kwargs)
                 except Exception as e:
                     _, _, tb = sys.exc_info()
                     traceback_info = traceback.extract_tb(tb)
                     line = traceback_info[-1][1]
                     file = traceback_info[-1][0]
                     function_name = traceback_info[-1][2]
 
-                    Froggius.error(log_msg=str(e), highlighting=True, print_out=True, line=[line, file, function_name], file_path=file_path)
+                    Froggius.error(
+                        log_msg=str(e),
+                        highlighting=True,
+                        print_out=True,
+                        line=[line, file, function_name],
+                        file_path=file_path,
+                    )
+
             return wrapper
+
         return decorator
-
```

### Comparing `froggius-0.1.3/setup.py` & `froggius-0.1.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import find_packages, setup
 
-with open("pypi.md", "r") as fh:
+with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
-    name='froggius',
-    packages=find_packages(include=['froggius']),
-    description='Froggius is a dumb easy logging tool for python',
+    name="froggius",
+    packages=find_packages(include=["froggius"]),
+    description="Froggius is a dumb easy logging tool for python",
     long_description=long_description,
-    version='0.1.3',
-    author='zlElo',
+    long_description_content_type="text/markdown",
+    version="0.1.4",
+    author="zlElo",
     author_email="mail@zlelo.de",
-    url = "https://github.com/zlElo/Froggius",
-    keywords=['pypi', 'cicd', 'python'],
+    url="https://github.com/zlElo/Froggius",
+    keywords=["logging", "logger", "easy-to-use", "log"],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows"
-    ]
+        "Operating System :: Microsoft :: Windows",
+    ],
 )
```

