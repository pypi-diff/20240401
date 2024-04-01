# Comparing `tmp/dateroll-0.1.8-py3-none-any.whl.zip` & `tmp/dateroll-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 467556 bytes, number of entries: 40
+Zip file size: 467653 bytes, number of entries: 40
 -rw-r--r--  2.0 unx      662 b- defN 24-Mar-28 21:03 dateroll/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 23:50 dateroll/__main__.py
 -rw-r--r--  2.0 unx     3246 b- defN 24-Mar-26 16:39 dateroll/pretty.py
 -rw-r--r--  2.0 unx     3892 b- defN 24-Mar-26 16:39 dateroll/settings.py
 -rw-r--r--  2.0 unx     1390 b- defN 24-Mar-27 20:06 dateroll/tblfmt.py
 -rw-r--r--  2.0 unx     6115 b- defN 24-Mar-27 13:14 dateroll/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 23:50 dateroll/calendars/__init__.py
@@ -11,15 +11,15 @@
 -rw-r--r--  2.0 unx     9108 b- defN 24-Mar-28 20:56 dateroll/calendars/calendars.py
 -rw-r--r--  2.0 unx     2197 b- defN 24-Mar-26 16:39 dateroll/calendars/sampledata.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 23:50 dateroll/date/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 23:50 dateroll/date/__main__.py
 -rw-r--r--  2.0 unx     8479 b- defN 24-Mar-27 13:26 dateroll/date/date.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 23:50 dateroll/ddh/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 23:50 dateroll/ddh/__main__.py
--rw-r--r--  2.0 unx     2116 b- defN 24-Mar-28 21:02 dateroll/ddh/ddh.py
+-rw-r--r--  2.0 unx     2919 b- defN 24-Mar-28 22:04 dateroll/ddh/ddh.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 23:50 dateroll/duration/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 23:50 dateroll/duration/__main__.py
 -rw-r--r--  2.0 unx    24491 b- defN 24-Mar-27 14:24 dateroll/duration/duration.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 23:50 dateroll/parser/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 23:50 dateroll/parser/__main__.py
 -rw-r--r--  2.0 unx     5968 b- defN 24-Mar-26 16:39 dateroll/parser/parser.py
 -rw-r--r--  2.0 unx    11777 b- defN 24-Mar-27 13:14 dateroll/parser/parsers.py
@@ -30,13 +30,13 @@
 -rw-r--r--  2.0 unx    50116 b- defN 24-Feb-29 23:50 dateroll/sampledata/FED.csv
 -rw-r--r--  2.0 unx    43461 b- defN 24-Feb-29 23:50 dateroll/sampledata/LN.csv
 -rw-r--r--  2.0 unx    50116 b- defN 24-Feb-29 23:50 dateroll/sampledata/NY.csv
 -rw-r--r--  2.0 unx   459162 b- defN 24-Feb-29 23:50 dateroll/sampledata/WE.csv
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 23:50 dateroll/schedule/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 23:50 dateroll/schedule/__main__.py
 -rw-r--r--  2.0 unx     5306 b- defN 24-Mar-27 13:14 dateroll/schedule/schedule.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Mar-28 21:03 dateroll-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1141 b- defN 24-Mar-28 21:03 dateroll-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-28 21:03 dateroll-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Mar-28 21:03 dateroll-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3258 b- defN 24-Mar-28 21:03 dateroll-0.1.8.dist-info/RECORD
-40 files, 2388548 bytes uncompressed, 462368 bytes compressed:  80.7%
+-rw-r--r--  2.0 unx    11357 b- defN 24-Mar-28 22:05 dateroll-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1141 b- defN 24-Mar-28 22:05 dateroll-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-28 22:05 dateroll-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Mar-28 22:05 dateroll-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3258 b- defN 24-Mar-28 22:05 dateroll-0.1.9.dist-info/RECORD
+40 files, 2389351 bytes uncompressed, 462465 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -99,23 +99,23 @@
 
 Filename: dateroll/schedule/__main__.py
 Comment: 
 
 Filename: dateroll/schedule/schedule.py
 Comment: 
 
-Filename: dateroll-0.1.8.dist-info/LICENSE
+Filename: dateroll-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: dateroll-0.1.8.dist-info/METADATA
+Filename: dateroll-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: dateroll-0.1.8.dist-info/WHEEL
+Filename: dateroll-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: dateroll-0.1.8.dist-info/top_level.txt
+Filename: dateroll-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: dateroll-0.1.8.dist-info/RECORD
+Filename: dateroll-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dateroll/ddh/ddh.py

```diff
@@ -20,15 +20,15 @@
 import dateroll.calendars.calendarmath as calendarmathModule
 import dateroll.calendars.calendars as calendarModule
 import dateroll.settings as settingsModule
 
 DEBUG = False
 
 class ddh:
-    # Date = dateModule.Date
+    Date = dateModule.Date
     Duration = durationModule.Duration
     Schedule = scheduleModule.Schedule
     settings = settingsModule.settings
     calmath = calendarmathModule.calmath
     hols = calendarmathModule.calmath.cals
 
     def __new__(cls, o):
@@ -55,14 +55,42 @@
             if not file.endswith("lockfile"):
                 if pathlib.Path(file).is_file():
                     os.remove(file)
         self.hols._purge_all()
         self.calmath._purge_all()
 
 
+    class YMD:
+        global settings
+        def __init__(self):
+            self.orig = ddh.settings.convention
+        def __enter__(self):
+            ddh.settings.convention = 'YMD'
+        def __exit__(self,*e):
+            ddh.settings.convention = self.orig
+
+    class MDY:
+        global settings
+        def __init__(self):
+            self.orig = ddh.settings.convention
+        def __enter__(self):
+            ddh.settings.convention = 'MDY'
+        def __exit__(self,*e):
+            ddh.settings.convention = self.orig
+
+    class DMY:
+        global settings
+        def __init__(self):
+            self.orig = ddh.settings.convention
+        def __enter__(self):
+            ddh.settings.convention = 'DMY'
+        def __exit__(self,*e):
+            ddh.settings.convention = self.orig
+
+
 if __name__ == "__main__":  # pragma:no cover
     import time
 
     a = time.time()
     # [calmath.bck['NYuWE'][calmath.fwd['NYuWE'][i]-1] for i in ddh('1/1/1900,1/1/2100,1d').dates]
     [i - "1bd|NYuWE" for i in ddh("1/1/1900,1/1/2100,1d").dates]
     print(time.time() - a)
```

## Comparing `dateroll-0.1.8.dist-info/LICENSE` & `dateroll-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dateroll-0.1.8.dist-info/METADATA` & `dateroll-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dateroll
-Version: 0.1.8
+Version: 0.1.9
 Summary: dateroll makes working with dates less painful.
 Home-page: https://github.com/disentcorp/dateroll
 Author: Anthony Malizzio
 Author-email: anthony.malizzio@disent.com
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

## Comparing `dateroll-0.1.8.dist-info/RECORD` & `dateroll-0.1.9.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 dateroll/calendars/calendars.py,sha256=kDSI5WLCGC38EDcF3M-7nM5bNY1Mj3bx8SdprSCDBpg,9108
 dateroll/calendars/sampledata.py,sha256=ghTTa32jzBhj4woZA5CbyoMa7Ao5o6LhJt6jg2kWDI4,2197
 dateroll/date/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dateroll/date/__main__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dateroll/date/date.py,sha256=aED4wNr204OLCQuoqrE2Oeb-iS9ZdPSZzbY0nJ2qLkg,8479
 dateroll/ddh/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dateroll/ddh/__main__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dateroll/ddh/ddh.py,sha256=ligKncywSOvAT0fPaVP6pC7b_0y48daNu6UoLDGCxKk,2116
+dateroll/ddh/ddh.py,sha256=y54f0dEcq2sUDBX8AfMWXSASIa9YRfeC9zUbs3HUjhM,2919
 dateroll/duration/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dateroll/duration/__main__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dateroll/duration/duration.py,sha256=lI4zLYpj_ASgX29q2kSquY8DovE29WiK2BnXKAeAH-w,24491
 dateroll/parser/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dateroll/parser/__main__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dateroll/parser/parser.py,sha256=3LGqpsu7F6ufjEjflc0AZgbYYyJ8TH5LQAAUTV3QTrI,5968
 dateroll/parser/parsers.py,sha256=alV2NnvKboMO4fG9BcyUrOo27qFwsXZrzDltso5X45Y,11777
@@ -29,12 +29,12 @@
 dateroll/sampledata/FED.csv,sha256=WhzeD5Zbrcg4zQ3EK06Yzh9l6-Od7PJ6xZcTvZy6Hy4,50116
 dateroll/sampledata/LN.csv,sha256=5jwkCP6XhDjrXM6dCeIanYt1Lkt5TES114GL9e5ZZFA,43461
 dateroll/sampledata/NY.csv,sha256=WhzeD5Zbrcg4zQ3EK06Yzh9l6-Od7PJ6xZcTvZy6Hy4,50116
 dateroll/sampledata/WE.csv,sha256=dea9eFyNBwyBGYbXqPjoT84tdIgvRwO34oJ42eT0KJs,459162
 dateroll/schedule/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dateroll/schedule/__main__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dateroll/schedule/schedule.py,sha256=MXcTSrSJwCYp0sZH04QhpQewuOJf0lEveu4WqSGGhO4,5306
-dateroll-0.1.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-dateroll-0.1.8.dist-info/METADATA,sha256=6EresamMerm9lhfhLq_Xl5qtnvI9x-nJmbyg9p49vX0,1141
-dateroll-0.1.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-dateroll-0.1.8.dist-info/top_level.txt,sha256=_nTOdTwmFVeheA44KYWK_l1Z73ynrc4bNPtBClgbmJc,9
-dateroll-0.1.8.dist-info/RECORD,,
+dateroll-0.1.9.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+dateroll-0.1.9.dist-info/METADATA,sha256=qffkp_mbVi1mMlqXIEjnP2aWbRX7jPyV8vzMMRgI8w0,1141
+dateroll-0.1.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+dateroll-0.1.9.dist-info/top_level.txt,sha256=_nTOdTwmFVeheA44KYWK_l1Z73ynrc4bNPtBClgbmJc,9
+dateroll-0.1.9.dist-info/RECORD,,
```

