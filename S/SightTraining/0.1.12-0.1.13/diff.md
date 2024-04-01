# Comparing `tmp/SightTraining-0.1.12.tar.gz` & `tmp/SightTraining-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SightTraining-0.1.12.tar", last modified: Mon Apr  1 09:29:37 2024, max compression
+gzip compressed data, was "SightTraining-0.1.13.tar", last modified: Mon Apr  1 09:31:38 2024, max compression
```

## Comparing `SightTraining-0.1.12.tar` & `SightTraining-0.1.13.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-01 09:29:37.490905 SightTraining-0.1.12/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     1067 2024-03-26 11:06:37.000000 SightTraining-0.1.12/LICENSE
--rw-r--r--   0 wangjuntao   (501) staff       (20)      539 2024-04-01 09:29:37.490652 SightTraining-0.1.12/PKG-INFO
--rw-r--r--   0 wangjuntao   (501) staff       (20)      211 2024-03-27 13:26:23.000000 SightTraining-0.1.12/README.md
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-01 09:29:37.490402 SightTraining-0.1.12/SightTraining.egg-info/
--rw-r--r--   0 wangjuntao   (501) staff       (20)      539 2024-04-01 09:29:37.000000 SightTraining-0.1.12/SightTraining.egg-info/PKG-INFO
--rw-r--r--   0 wangjuntao   (501) staff       (20)      365 2024-04-01 09:29:37.000000 SightTraining-0.1.12/SightTraining.egg-info/SOURCES.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)        1 2024-04-01 09:29:37.000000 SightTraining-0.1.12/SightTraining.egg-info/dependency_links.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)       52 2024-04-01 09:29:37.000000 SightTraining-0.1.12/SightTraining.egg-info/entry_points.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)       35 2024-04-01 09:29:37.000000 SightTraining-0.1.12/SightTraining.egg-info/requires.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)       13 2024-04-01 09:29:37.000000 SightTraining-0.1.12/SightTraining.egg-info/top_level.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)       38 2024-04-01 09:29:37.490957 SightTraining-0.1.12/setup.cfg
--rw-r--r--   0 wangjuntao   (501) staff       (20)      885 2024-04-01 09:29:30.000000 SightTraining-0.1.12/setup.py
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-01 09:29:37.490152 SightTraining-0.1.12/spacedefense/
--rw-r--r--   0 wangjuntao   (501) staff       (20)        0 2024-04-01 09:29:33.000000 SightTraining-0.1.12/spacedefense/__init__.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)    31552 2024-04-01 09:20:04.000000 SightTraining-0.1.12/spacedefense/actors.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)     2239 2024-04-01 09:01:37.000000 SightTraining-0.1.12/spacedefense/common.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)     4980 2024-04-01 08:48:15.000000 SightTraining-0.1.12/spacedefense/config.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)    24303 2024-04-01 09:19:50.000000 SightTraining-0.1.12/spacedefense/main.py
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-01 09:31:38.330922 SightTraining-0.1.13/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     1067 2024-03-26 11:06:37.000000 SightTraining-0.1.13/LICENSE
+-rw-r--r--   0 wangjuntao   (501) staff       (20)      539 2024-04-01 09:31:38.330693 SightTraining-0.1.13/PKG-INFO
+-rw-r--r--   0 wangjuntao   (501) staff       (20)      211 2024-03-27 13:26:23.000000 SightTraining-0.1.13/README.md
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-01 09:31:38.330365 SightTraining-0.1.13/SightTraining.egg-info/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)      539 2024-04-01 09:31:38.000000 SightTraining-0.1.13/SightTraining.egg-info/PKG-INFO
+-rw-r--r--   0 wangjuntao   (501) staff       (20)      365 2024-04-01 09:31:38.000000 SightTraining-0.1.13/SightTraining.egg-info/SOURCES.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)        1 2024-04-01 09:31:38.000000 SightTraining-0.1.13/SightTraining.egg-info/dependency_links.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       49 2024-04-01 09:31:38.000000 SightTraining-0.1.13/SightTraining.egg-info/entry_points.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       35 2024-04-01 09:31:38.000000 SightTraining-0.1.13/SightTraining.egg-info/requires.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       13 2024-04-01 09:31:38.000000 SightTraining-0.1.13/SightTraining.egg-info/top_level.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       38 2024-04-01 09:31:38.330958 SightTraining-0.1.13/setup.cfg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)      882 2024-04-01 09:31:29.000000 SightTraining-0.1.13/setup.py
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-01 09:31:38.330103 SightTraining-0.1.13/spacedefense/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       64 2024-04-01 09:31:18.000000 SightTraining-0.1.13/spacedefense/__init__.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    31552 2024-04-01 09:20:04.000000 SightTraining-0.1.13/spacedefense/actors.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     2239 2024-04-01 09:01:37.000000 SightTraining-0.1.13/spacedefense/common.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     4980 2024-04-01 08:48:15.000000 SightTraining-0.1.13/spacedefense/config.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    24303 2024-04-01 09:19:50.000000 SightTraining-0.1.13/spacedefense/main.py
```

### Comparing `SightTraining-0.1.12/LICENSE` & `SightTraining-0.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.12/PKG-INFO` & `SightTraining-0.1.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SightTraining
-Version: 0.1.12
+Version: 0.1.13
 Summary: SightTraining  is a game for children's amblyopia training
 Author: jett.wang
 Author-email: jamiesun.net@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SightTraining-0.1.12/SightTraining.egg-info/PKG-INFO` & `SightTraining-0.1.13/SightTraining.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SightTraining
-Version: 0.1.12
+Version: 0.1.13
 Summary: SightTraining  is a game for children's amblyopia training
 Author: jett.wang
 Author-email: jamiesun.net@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SightTraining-0.1.12/setup.py` & `SightTraining-0.1.13/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 readme = """
 SightTraining  is a game for children's amblyopia training
 """
 
 setup(
     name="SightTraining",
-    version="0.1.12",
+    version="0.1.13",
     author="jett.wang",
     author_email="jamiesun.net@gmail.com",
     description="SightTraining  is a game for children's amblyopia training",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
@@ -24,11 +24,11 @@
     install_requires=[
         "pygame==2.5.1",
         "python-dotenv>=1.0.1"
     ],
     python_requires='>=3.10',
     entry_points={
         "console_scripts": [
-            "spacex01 = spacedefense.main:main"
+            "spacex01 = spacedefense:runapp"
         ]
     },
 )
```

### Comparing `SightTraining-0.1.12/spacedefense/actors.py` & `SightTraining-0.1.13/spacedefense/actors.py`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.12/spacedefense/common.py` & `SightTraining-0.1.13/spacedefense/common.py`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.12/spacedefense/config.py` & `SightTraining-0.1.13/spacedefense/config.py`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.12/spacedefense/main.py` & `SightTraining-0.1.13/spacedefense/main.py`

 * *Files identical despite different names*

