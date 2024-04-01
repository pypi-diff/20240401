# Comparing `tmp/configureout-1.1.tar.gz` & `tmp/configureout-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configureout-1.1.tar", last modified: Mon Apr  1 14:57:08 2024, max compression
+gzip compressed data, was "configureout-1.2.tar", last modified: Mon Apr  1 15:03:52 2024, max compression
```

## Comparing `configureout-1.1.tar` & `configureout-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 14:57:08.516528 configureout-1.1/
--rw-rw-rw-   0        0        0     2193 2024-04-01 14:57:08.515529 configureout-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1792 2024-04-01 13:08:22.000000 configureout-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 14:57:08.507027 configureout-1.1/configureout/
--rw-rw-rw-   0        0        0      923 2024-04-01 14:56:05.000000 configureout-1.1/configureout/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 14:57:08.514529 configureout-1.1/configureout.egg-info/
--rw-rw-rw-   0        0        0     2193 2024-04-01 14:57:08.000000 configureout-1.1/configureout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2024-04-01 14:57:08.000000 configureout-1.1/configureout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 14:57:08.000000 configureout-1.1/configureout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-01 14:57:08.000000 configureout-1.1/configureout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-01 14:57:08.000000 configureout-1.1/configureout.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 14:57:08.516528 configureout-1.1/setup.cfg
--rw-rw-rw-   0        0        0      671 2024-04-01 14:55:59.000000 configureout-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 15:03:52.166612 configureout-1.2/
+-rw-rw-rw-   0        0        0     2193 2024-04-01 15:03:52.165605 configureout-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1792 2024-04-01 13:08:22.000000 configureout-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 15:03:52.150596 configureout-1.2/configureout/
+-rw-rw-rw-   0        0        0      993 2024-04-01 15:03:27.000000 configureout-1.2/configureout/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 15:03:52.164101 configureout-1.2/configureout.egg-info/
+-rw-rw-rw-   0        0        0     2193 2024-04-01 15:03:52.000000 configureout-1.2/configureout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-04-01 15:03:52.000000 configureout-1.2/configureout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 15:03:52.000000 configureout-1.2/configureout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-01 15:03:52.000000 configureout-1.2/configureout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-01 15:03:52.000000 configureout-1.2/configureout.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 15:03:52.166612 configureout-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      671 2024-04-01 15:03:45.000000 configureout-1.2/setup.py
```

### Comparing `configureout-1.1/PKG-INFO` & `configureout-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configureout
-Version: 1.1
+Version: 1.2
 Summary: A simple configuration module
 Home-page: https://github.com/EightShift/configureout
 Author: EightShift
 Author-email: the8shift@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `configureout-1.1/README.md` & `configureout-1.2/README.md`

 * *Files identical despite different names*

### Comparing `configureout-1.1/configureout/__init__.py` & `configureout-1.2/configureout/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 class BaseConfig():
     def __init__(self, config):
         self.__config = config
         
         for key, value in self.__config.items():
             setattr(self, key, BaseConfig(value) if type(value) == dict else value)
 
+    def __getitem__(self, key):
+        return getattr(self, key)
+
     def keys(self):
         for key in self.__config.keys():
             yield key
 
     def values(self):
         for key in self.__config.keys():
             yield getattr(self, key)
```

### Comparing `configureout-1.1/configureout.egg-info/PKG-INFO` & `configureout-1.2/configureout.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configureout
-Version: 1.1
+Version: 1.2
 Summary: A simple configuration module
 Home-page: https://github.com/EightShift/configureout
 Author: EightShift
 Author-email: the8shift@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `configureout-1.1/setup.py` & `configureout-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='configureout',
-    version='1.1',
+    version='1.2',
     description='A simple configuration module',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='EightShift',
     author_email='the8shift@gmail.com',
     url='https://github.com/EightShift/configureout',
     packages=find_packages(),
```

