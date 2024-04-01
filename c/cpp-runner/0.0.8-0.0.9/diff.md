# Comparing `tmp/cpp-runner-0.0.8.tar.gz` & `tmp/cpp-runner-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpp-runner-0.0.8.tar", last modified: Mon Dec 25 14:10:28 2023, max compression
+gzip compressed data, was "cpp-runner-0.0.9.tar", last modified: Mon Dec 25 14:13:51 2023, max compression
```

## Comparing `cpp-runner-0.0.8.tar` & `cpp-runner-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-12-25 14:10:28.783647 cpp-runner-0.0.8/
--rw-rw-rw-   0        0        0      725 2023-12-25 14:10:28.783647 cpp-runner-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-12-25 11:11:37.000000 cpp-runner-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-12-25 14:10:28.783647 cpp-runner-0.0.8/cpp_runner.egg-info/
--rw-rw-rw-   0        0        0      725 2023-12-25 14:10:28.000000 cpp-runner-0.0.8/cpp_runner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-12-25 14:10:28.000000 cpp-runner-0.0.8/cpp_runner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-25 14:10:28.000000 cpp-runner-0.0.8/cpp_runner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-12-25 14:10:28.000000 cpp-runner-0.0.8/cpp_runner.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-12-25 14:10:28.000000 cpp-runner-0.0.8/cpp_runner.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-12-25 14:10:28.000000 cpp-runner-0.0.8/cpp_runner.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-12-25 14:10:28.783647 cpp-runner-0.0.8/crun/
--rw-rw-rw-   0        0        0       21 2023-12-19 17:37:29.000000 cpp-runner-0.0.8/crun/__init__.py
--rw-rw-rw-   0        0        0     8923 2023-12-25 14:02:54.000000 cpp-runner-0.0.8/crun/crun.py
--rw-rw-rw-   0        0        0       42 2023-12-25 14:10:28.783647 cpp-runner-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-12-25 14:02:58.000000 cpp-runner-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-25 14:13:51.156317 cpp-runner-0.0.9/
+-rw-rw-rw-   0        0        0      725 2023-12-25 14:13:51.156317 cpp-runner-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-12-25 11:11:37.000000 cpp-runner-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-12-25 14:13:51.140783 cpp-runner-0.0.9/cpp_runner.egg-info/
+-rw-rw-rw-   0        0        0      725 2023-12-25 14:13:51.000000 cpp-runner-0.0.9/cpp_runner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-12-25 14:13:51.000000 cpp-runner-0.0.9/cpp_runner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-25 14:13:51.000000 cpp-runner-0.0.9/cpp_runner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-12-25 14:13:51.000000 cpp-runner-0.0.9/cpp_runner.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-12-25 14:13:51.000000 cpp-runner-0.0.9/cpp_runner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-12-25 14:13:51.000000 cpp-runner-0.0.9/cpp_runner.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-12-25 14:13:51.140783 cpp-runner-0.0.9/crun/
+-rw-rw-rw-   0        0        0       21 2023-12-19 17:37:29.000000 cpp-runner-0.0.9/crun/__init__.py
+-rw-rw-rw-   0        0        0     8919 2023-12-25 14:13:46.000000 cpp-runner-0.0.9/crun/crun.py
+-rw-rw-rw-   0        0        0       42 2023-12-25 14:13:51.156317 cpp-runner-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      611 2023-12-25 14:13:46.000000 cpp-runner-0.0.9/setup.py
```

### Comparing `cpp-runner-0.0.8/PKG-INFO` & `cpp-runner-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpp-runner
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple, small command line utility to run cpp files.
 Home-page: https://github.com/macaquedev/cpp-runner
 Author: Alex Pylypenko
 Author-email: macaquedev@gmail.com
 License: MIT
 Requires-Python: >=3.3
 Description-Content-Type: text/x-rst
```

### Comparing `cpp-runner-0.0.8/cpp_runner.egg-info/PKG-INFO` & `cpp-runner-0.0.9/cpp_runner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpp-runner
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple, small command line utility to run cpp files.
 Home-page: https://github.com/macaquedev/cpp-runner
 Author: Alex Pylypenko
 Author-email: macaquedev@gmail.com
 License: MIT
 Requires-Python: >=3.3
 Description-Content-Type: text/x-rst
```

### Comparing `cpp-runner-0.0.8/crun/crun.py` & `cpp-runner-0.0.9/crun/crun.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         os << '"' << v[0] << '"';
     }
     else {
         os << v[0];
     }
     for (int i=1; i<v.size(); i++) {
         if (typeid(T) == typeid(string)) {
-            os << ", \"" << v[i] << '"';        
+            os << ", " << v[i] << '"';        
         }
         else {
             os << ", " << v[i];
         }
     }
     os << "]";
     return os;
@@ -224,15 +224,15 @@
         os << '"' << v[0] << '"';
     }
     else {
         os << v[0];
     }
     for (int i=1; i<v.size(); i++) {
         if (typeid(T) == typeid(string)) {
-            os << ", \"" << v[i] << '"';        
+            os << ", " << v[i] << '"';        
         }
         else {
             os << ", " << v[i];
         }
     }
     os << "]";
     return os;
```

### Comparing `cpp-runner-0.0.8/setup.py` & `cpp-runner-0.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name='cpp-runner',
-    version='0.0.8',
+    version='0.0.9',
     license="MIT",
     entry_points={
         'console_scripts': ['crun=crun.crun:cli'],
     },
     packages=["crun"],
     url="https://github.com/macaquedev/cpp-runner",
     author='Alex Pylypenko',
```

