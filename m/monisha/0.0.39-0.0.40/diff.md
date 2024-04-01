# Comparing `tmp/monisha-0.0.39.tar.gz` & `tmp/monisha-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.39.tar", last modified: Fri Mar 29 06:56:08 2024, max compression
+gzip compressed data, was "monisha-0.0.40.tar", last modified: Mon Apr  1 16:36:53 2024, max compression
```

## Comparing `monisha-0.0.39.tar` & `monisha-0.0.40.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:56:08.578969 monisha-0.0.39/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-29 06:56:02.000000 monisha-0.0.39/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:56:08.574969 monisha-0.0.39/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 06:56:02.000000 monisha-0.0.39/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:56:08.574969 monisha-0.0.39/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-29 06:56:02.000000 monisha-0.0.39/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-03-29 06:56:02.000000 monisha-0.0.39/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-29 06:56:02.000000 monisha-0.0.39/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-29 06:56:02.000000 monisha-0.0.39/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-29 06:56:02.000000 monisha-0.0.39/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-29 06:56:02.000000 monisha-0.0.39/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-03-29 06:56:02.000000 monisha-0.0.39/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-29 06:56:02.000000 monisha-0.0.39/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-29 06:56:02.000000 monisha-0.0.39/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-29 06:56:02.000000 monisha-0.0.39/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-03-29 06:56:02.000000 monisha-0.0.39/Monisha/functions/function10.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:56:08.574969 monisha-0.0.39/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-29 06:56:02.000000 monisha-0.0.39/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-29 06:56:02.000000 monisha-0.0.39/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-29 06:56:02.000000 monisha-0.0.39/Monisha/scripts/se.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-29 06:56:02.000000 monisha-0.0.39/Monisha/scripts/uo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-03-29 06:56:08.578969 monisha-0.0.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-29 06:56:02.000000 monisha-0.0.39/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:56:08.578969 monisha-0.0.39/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-03-29 06:56:08.000000 monisha-0.0.39/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-29 06:56:08.000000 monisha-0.0.39/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 06:56:08.000000 monisha-0.0.39/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 06:56:08.000000 monisha-0.0.39/monisha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-29 06:56:08.000000 monisha-0.0.39/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 06:56:08.578969 monisha-0.0.39/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-29 06:56:02.000000 monisha-0.0.39/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:36:53.214939 monisha-0.0.40/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-01 16:36:48.000000 monisha-0.0.40/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:36:53.210939 monisha-0.0.40/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:36:53.214939 monisha-0.0.40/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:36:53.214939 monisha-0.0.40/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/scripts/se.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/scripts/uo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-01 16:36:53.214939 monisha-0.0.40/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-01 16:36:48.000000 monisha-0.0.40/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:36:53.214939 monisha-0.0.40/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-01 16:36:53.000000 monisha-0.0.40/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-01 16:36:53.000000 monisha-0.0.40/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:36:53.000000 monisha-0.0.40/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:36:53.000000 monisha-0.0.40/monisha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 16:36:53.000000 monisha-0.0.40/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 16:36:53.214939 monisha-0.0.40/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-01 16:36:48.000000 monisha-0.0.40/setup.py
```

### Comparing `monisha-0.0.39/LICENSE` & `monisha-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.39/Monisha/functions/function01.py` & `monisha-0.0.40/Monisha/functions/function01.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,73 +12,36 @@
     minutes, seconds = divmod(hourz, 60)
     return round(hours), round(minutes), round(seconds)
 
 #=========================================================================
 
 def Timemod(moonos: int) -> str:
     mosems = 1 if moonos == Scripted.DATA02 else moonos
-    moonse = mosems if mosems > 1 else 1
+    moonse = mosems if 1 < mosems else 1
     minute, seconds = divmod(moonse, 60)
     hours, minute = divmod(minute, 60)
     days, hours = divmod(hours, 24)
     year, days = divmod(days, 365)
     mos  = ((str(year) + "𝚢𝚎𝚊𝚛, ") if year else Scripted.DATA01)
     mos += ((str(days) + "𝚍𝚊𝚢𝚜, ") if days else Scripted.DATA01)
     mos += ((str(hours) + "𝚑𝚛𝚜, ") if hours else Scripted.DATA01)
     mos += ((str(minute) + "𝚖𝚒𝚗, ") if minute else Scripted.DATA01)
     mos += ((str(seconds) + "𝚜𝚎𝚌") if seconds else Scripted.DATA06)
     return mos
 
 #=========================================================================
 
-def Timecod(moonos: int) -> str:
-    mosems = 1 if moonos == Scripted.DATA02 else moonos
-    moonse = mosems if mosems > 1 else 1
-    seconds, millesec = divmod(moonse, 1000)
-    minute, seconds = divmod(seconds, 60)
-    hours, minute = divmod(minute, 60)
-    days, hours = divmod(hours, 24)
-    year, days = divmod(days, 365)
-    mos  = ((str(year) + "𝚢𝚎𝚊𝚛, ") if year else Scripted.DATA01)
-    mos += ((str(days) + "𝚍𝚊𝚢𝚜, ") if days else Scripted.DATA01)
-    mos += ((str(hours) + "𝚑𝚛𝚜, ") if hours else Scripted.DATA01)
-    mos += ((str(minute) + "𝚖𝚒𝚗, ") if minute else Scripted.DATA01)
-    mos += ((str(seconds) + "𝚜𝚎𝚌, ") if seconds else Scripted.DATA01)
-    mos += ((str(millesec) + "𝚖𝚜𝚌") if millesec else Scripted.DATA10)
-    return mos
-
-#=========================================================================
-# N FONT
-
-def Timenod(moonos: int) -> str:
-    mosems = 1 if moonos == Scripted.DATA02 else moonos
-    moonse = mosems if mosems > 1 else 1
-    minute, seconds = divmod(moonse, 60)
-    hours, minute = divmod(minute, 60)
-    days, hours = divmod(hours, 24)
-    year, days = divmod(days, 365)
-    mos  = ((str(year) + "year, ") if year else Scripted.DATA01)
-    mos += ((str(days) + "days, ") if days else Scripted.DATA01)
-    mos += ((str(hours) + "hrs, ") if hours else Scripted.DATA01)
-    mos += ((str(minute) + "min, ") if minute else Scripted.DATA01)
-    mos += ((str(seconds) + "sec") if seconds else Scripted.DATA07)
-    return mos
-
-#=========================================================================
-
 def Timesod(moonos: int) -> str:
     mosems = 1 if moonos == Scripted.DATA02 else moonos
-    moonse = mosems if mosems > 1 else 1
-    seconds, millesec = divmod(moonse, 1000)
-    minute, seconds = divmod(seconds, 60)
+    moonse = mosems if 1 < mosems else 1
+    minute, seconds = divmod(moonse, 60)
     hours, minute = divmod(minute, 60)
     days, hours = divmod(hours, 24)
     year, days = divmod(days, 365)
     mos  = ((str(year) + "year, ") if year else Scripted.DATA01)
     mos += ((str(days) + "days, ") if days else Scripted.DATA01)
     mos += ((str(hours) + "hrs, ") if hours else Scripted.DATA01)
     mos += ((str(minute) + "min, ") if minute else Scripted.DATA01)
-    mos += ((str(seconds) + "sec, ") if seconds else Scripted.DATA01)
-    mos += ((str(millesec) + "mse") if millesec else Scripted.DATA11)
+    mos += ((str(seconds) + "sec, ") if seconds else Scripted.DATA07)
     return mos
 
 #=========================================================================
```

### Comparing `monisha-0.0.39/Monisha/functions/function02.py` & `monisha-0.0.40/Monisha/functions/function02.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.39/Monisha/functions/function03.py` & `monisha-0.0.40/Monisha/functions/function03.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.39/Monisha/functions/function04.py` & `monisha-0.0.40/Monisha/functions/function04.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.39/Monisha/functions/function06.py` & `monisha-0.0.40/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.39/Monisha/functions/function07.py` & `monisha-0.0.40/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.39/Monisha/functions/function10.py` & `monisha-0.0.40/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.39/PKG-INFO` & `monisha-0.0.40/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.39
+Version: 0.0.40
 Summary: python helper modules
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.39 Summary: python helper
+Metadata-Version: 2.1 Name: monisha Version: 0.0.40 Summary: python helper
 modules Home-page: https://github.com/Clinton-Abraham Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,clinton,abraham Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Natural Language ::
 English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `monisha-0.0.39/README.md` & `monisha-0.0.40/README.md`

 * *Files identical despite different names*

### Comparing `monisha-0.0.39/monisha.egg-info/PKG-INFO` & `monisha-0.0.40/monisha.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.39
+Version: 0.0.40
 Summary: python helper modules
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.39 Summary: python helper
+Metadata-Version: 2.1 Name: monisha Version: 0.0.40 Summary: python helper
 modules Home-page: https://github.com/Clinton-Abraham Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,clinton,abraham Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Natural Language ::
 English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `monisha-0.0.39/monisha.egg-info/SOURCES.txt` & `monisha-0.0.40/monisha.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 Monisha/functions/function04.py
 Monisha/functions/function05.py
 Monisha/functions/function06.py
 Monisha/functions/function07.py
 Monisha/functions/function08.py
 Monisha/functions/function09.py
 Monisha/functions/function10.py
+Monisha/functions/function11.py
 Monisha/scripts/__init__.py
 Monisha/scripts/en.py
 Monisha/scripts/se.py
 Monisha/scripts/uo.py
 monisha.egg-info/PKG-INFO
 monisha.egg-info/SOURCES.txt
 monisha.egg-info/dependency_links.txt
```

### Comparing `monisha-0.0.39/setup.py` & `monisha-0.0.40/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules']
 
 setup(
     name='monisha',
     license='MIT',
     zip_safe=False,
-    version='0.0.39',
+    version='0.0.40',
     classifiers=DATA02,
     author_email=DATA01,
     python_requires='~=3.8',
     packages=find_packages(),
     author='Clinton-Abraham',
     long_description=long_description,
     description='python helper modules',
```

