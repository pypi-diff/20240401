# Comparing `tmp/talklib-1.0.8.tar.gz` & `tmp/talklib-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talklib-1.0.8.tar", last modified: Wed Feb  7 23:01:15 2024, max compression
+gzip compressed data, was "talklib-1.0.9.tar", last modified: Thu Feb  8 22:37:42 2024, max compression
```

## Comparing `talklib-1.0.8.tar` & `talklib-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 23:01:15.084327 talklib-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-02-07 22:58:48.000000 talklib-1.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14149 2024-02-07 23:01:15.084327 talklib-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-02-07 22:58:48.000000 talklib-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-07 22:58:48.000000 talklib-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-07 22:58:48.000000 talklib-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 23:01:15.084327 talklib-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 23:01:15.080327 talklib-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 23:01:15.084327 talklib-1.0.8/src/talklib/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-07 22:58:48.000000 talklib-1.0.8/src/talklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-02-07 22:58:48.000000 talklib-1.0.8/src/talklib/ev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-02-07 22:58:48.000000 talklib-1.0.8/src/talklib/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-02-07 22:58:48.000000 talklib-1.0.8/src/talklib/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)    21499 2024-02-07 22:58:48.000000 talklib-1.0.8/src/talklib/show.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-02-07 22:58:48.000000 talklib-1.0.8/src/talklib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 23:01:15.084327 talklib-1.0.8/src/talklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14149 2024-02-07 23:01:15.000000 talklib-1.0.8/src/talklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-07 23:01:15.000000 talklib-1.0.8/src/talklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 23:01:15.000000 talklib-1.0.8/src/talklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-07 23:01:15.000000 talklib-1.0.8/src/talklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-07 23:01:15.000000 talklib-1.0.8/src/talklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:37:42.233012 talklib-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-02-08 22:37:31.000000 talklib-1.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14149 2024-02-08 22:37:42.233012 talklib-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-02-08 22:37:31.000000 talklib-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-08 22:37:31.000000 talklib-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-08 22:37:31.000000 talklib-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 22:37:42.233012 talklib-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:37:42.233012 talklib-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:37:42.233012 talklib-1.0.9/src/talklib/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-08 22:37:31.000000 talklib-1.0.9/src/talklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-02-08 22:37:31.000000 talklib-1.0.9/src/talklib/ev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-08 22:37:31.000000 talklib-1.0.9/src/talklib/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-02-08 22:37:31.000000 talklib-1.0.9/src/talklib/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21482 2024-02-08 22:37:31.000000 talklib-1.0.9/src/talklib/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-02-08 22:37:31.000000 talklib-1.0.9/src/talklib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:37:42.233012 talklib-1.0.9/src/talklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14149 2024-02-08 22:37:42.000000 talklib-1.0.9/src/talklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-08 22:37:42.000000 talklib-1.0.9/src/talklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 22:37:42.000000 talklib-1.0.9/src/talklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-08 22:37:42.000000 talklib-1.0.9/src/talklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-08 22:37:42.000000 talklib-1.0.9/src/talklib.egg-info/top_level.txt
```

### Comparing `talklib-1.0.8/LICENSE.txt` & `talklib-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `talklib-1.0.8/PKG-INFO` & `talklib-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talklib
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package to automate processing of shows/segments airing on the TL
 Author-email: Ben Weddle <ben.weddle@gmail.com>
 Maintainer-email: Ben Weddle <ben.weddle@gmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `talklib-1.0.8/README.md` & `talklib-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `talklib-1.0.8/pyproject.toml` & `talklib-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "talklib"
-version = "1.0.8"
+version = "1.0.9"
 description = "A package to automate processing of shows/segments airing on the TL"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 authors = [{name = "Ben Weddle", email = "ben.weddle@gmail.com"}]
 maintainers = [{name = "Ben Weddle", email = "ben.weddle@gmail.com"}]
 requires-python = ">=3.10"
 dynamic = ["dependencies"]
```

### Comparing `talklib-1.0.8/requirements.txt` & `talklib-1.0.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `talklib-1.0.8/src/talklib/ev.py` & `talklib-1.0.9/src/talklib/ev.py`

 * *Files identical despite different names*

### Comparing `talklib-1.0.8/src/talklib/ffmpeg.py` & `talklib-1.0.9/src/talklib/ffmpeg.py`

 * *Files 17% similar despite different names*

```diff
@@ -48,8 +48,19 @@
     def convert(self):
         '''convert file with ffmpeg and return filename'''
         input_commands = self.build_input_commands()
         output_commands = self.build_output_commands()
         stream = ffmpeg.input(**input_commands)
         stream = ffmpeg.output(stream, **output_commands)
         ffmpeg.run(stream, capture_stdout=True)
-        return self.output_file
+        return self.output_file
+    
+    def get_length_in_minutes(self) -> float:
+        duration = ffmpeg.probe(filename=self.input_file)
+        duration = duration['format']['duration']
+        
+        # convert the number to something more usable/readable
+        duration = float(duration)
+        duration = duration/60
+        duration = round(duration, 2)
+
+        return duration
```

### Comparing `talklib-1.0.8/src/talklib/notify.py` & `talklib-1.0.9/src/talklib/notify.py`

 * *Files identical despite different names*

### Comparing `talklib-1.0.8/src/talklib/show.py` & `talklib-1.0.9/src/talklib/show.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import xml.etree.ElementTree as ET
 
 import ffmpeg
 import requests
 
 from talklib.ev import EV
 from talklib.notify import Notify
-from talklib.utils import get_timestamp, clear_screen, print_to_screen_and_wait, today_is_weekday, get_length_in_minutes
+from talklib.utils import get_timestamp, clear_screen, print_to_screen_and_wait, today_is_weekday
 from talklib.ffmpeg import FFMPEG
 
 
 class TLShow():
     '''TODO write something here'''
     def __init__(self):
 
@@ -227,15 +227,15 @@
         # if these are not declared, don't run this check.
         if not (self.check_if_below and self.check_if_above):
             TLShow.prep_syslog(self, message='The check length function is turned off.')
         else:
             TLShow.prep_syslog(self, message=f'Checking whether length is between \
 {self.check_if_below} and {self.check_if_above}')
 
-            duration = get_length_in_minutes(file_to_check=fileToCheck)
+            duration = FFMPEG(input_file=fileToCheck).get_length_in_minutes()
 
             if duration > self.check_if_above:
                 toSend = (f"Today's {self.show} is {duration} minutes long! \
 Please check manually and make edits to bring it below {self.check_if_above} minutes.\n\n\
 {get_timestamp()}")
                 TLShow.send_notifications(self, message=toSend, subject='Check Length')
```

### Comparing `talklib-1.0.8/src/talklib/utils.py` & `talklib-1.0.9/src/talklib/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -30,19 +30,8 @@
 def today_is_weekday() -> bool:
     '''crude mechanism for determining if today is a weekday.'''
     today = datetime.now().strftime('%a')
     weekend = ['Sat', 'Sun']
     if today not in weekend:
         return True
     else:
-        return False
-
-def get_length_in_minutes(file_to_check) -> float:
-    duration = ffmpeg.probe(filename=file_to_check)
-    duration = duration['format']['duration']
-    
-    # convert the number to something more usable/readable
-    duration = float(duration)
-    duration = duration/60
-    duration = round(duration, 2)
-
-    return duration
+        return False
```

### Comparing `talklib-1.0.8/src/talklib.egg-info/PKG-INFO` & `talklib-1.0.9/src/talklib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talklib
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package to automate processing of shows/segments airing on the TL
 Author-email: Ben Weddle <ben.weddle@gmail.com>
 Maintainer-email: Ben Weddle <ben.weddle@gmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `talklib-1.0.8/src/talklib.egg-info/requires.txt` & `talklib-1.0.9/src/talklib.egg-info/requires.txt`

 * *Files identical despite different names*

