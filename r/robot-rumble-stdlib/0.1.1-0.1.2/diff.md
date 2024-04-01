# Comparing `tmp/robot-rumble-stdlib-0.1.1.tar.gz` & `tmp/robot-rumble-stdlib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robot-rumble-stdlib-0.1.1.tar", last modified: Sun Mar 24 05:47:43 2024, max compression
+gzip compressed data, was "robot-rumble-stdlib-0.1.2.tar", last modified: Mon Apr  1 14:51:19 2024, max compression
```

## Comparing `robot-rumble-stdlib-0.1.1.tar` & `robot-rumble-stdlib-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-03-24 05:47:43.303350 robot-rumble-stdlib-0.1.1/
--rw-r--r--   0 anton     (1000) anton     (1000)    35149 2020-10-26 13:05:47.000000 robot-rumble-stdlib-0.1.1/LICENSE
--rw-r--r--   0 anton     (1000) anton     (1000)      721 2024-03-24 05:47:43.303350 robot-rumble-stdlib-0.1.1/PKG-INFO
--rw-r--r--   0 anton     (1000) anton     (1000)      271 2020-10-26 13:05:47.000000 robot-rumble-stdlib-0.1.1/README.md
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-03-24 05:47:43.303350 robot-rumble-stdlib-0.1.1/robot_rumble_stdlib.egg-info/
--rw-r--r--   0 anton     (1000) anton     (1000)      721 2024-03-24 05:47:43.000000 robot-rumble-stdlib-0.1.1/robot_rumble_stdlib.egg-info/PKG-INFO
--rw-r--r--   0 anton     (1000) anton     (1000)      211 2024-03-24 05:47:43.000000 robot-rumble-stdlib-0.1.1/robot_rumble_stdlib.egg-info/SOURCES.txt
--rw-r--r--   0 anton     (1000) anton     (1000)        1 2024-03-24 05:47:43.000000 robot-rumble-stdlib-0.1.1/robot_rumble_stdlib.egg-info/dependency_links.txt
--rw-r--r--   0 anton     (1000) anton     (1000)       10 2024-03-24 05:47:43.000000 robot-rumble-stdlib-0.1.1/robot_rumble_stdlib.egg-info/top_level.txt
--rwxr-xr-x   0 anton     (1000) anton     (1000)    12429 2024-03-24 05:44:08.000000 robot-rumble-stdlib-0.1.1/rumblelib.py
--rw-r--r--   0 anton     (1000) anton     (1000)       38 2024-03-24 05:47:43.303350 robot-rumble-stdlib-0.1.1/setup.cfg
--rw-r--r--   0 anton     (1000) anton     (1000)      612 2024-01-05 03:35:19.000000 robot-rumble-stdlib-0.1.1/setup.py
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-04-01 14:51:19.113320 robot-rumble-stdlib-0.1.2/
+-rw-r--r--   0 anton     (1000) anton     (1000)    35149 2024-03-31 16:26:18.000000 robot-rumble-stdlib-0.1.2/LICENSE
+-rw-r--r--   0 anton     (1000) anton     (1000)      721 2024-04-01 14:51:19.113320 robot-rumble-stdlib-0.1.2/PKG-INFO
+-rw-r--r--   0 anton     (1000) anton     (1000)      271 2020-10-26 13:05:47.000000 robot-rumble-stdlib-0.1.2/README.md
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-04-01 14:51:19.113320 robot-rumble-stdlib-0.1.2/robot_rumble_stdlib.egg-info/
+-rw-r--r--   0 anton     (1000) anton     (1000)      721 2024-04-01 14:51:19.000000 robot-rumble-stdlib-0.1.2/robot_rumble_stdlib.egg-info/PKG-INFO
+-rw-r--r--   0 anton     (1000) anton     (1000)      211 2024-04-01 14:51:19.000000 robot-rumble-stdlib-0.1.2/robot_rumble_stdlib.egg-info/SOURCES.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)        1 2024-04-01 14:51:19.000000 robot-rumble-stdlib-0.1.2/robot_rumble_stdlib.egg-info/dependency_links.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)       10 2024-04-01 14:51:19.000000 robot-rumble-stdlib-0.1.2/robot_rumble_stdlib.egg-info/top_level.txt
+-rwxr-xr-x   0 anton     (1000) anton     (1000)    12701 2024-03-31 14:04:41.000000 robot-rumble-stdlib-0.1.2/rumblelib.py
+-rw-r--r--   0 anton     (1000) anton     (1000)       38 2024-04-01 14:51:19.113320 robot-rumble-stdlib-0.1.2/setup.cfg
+-rw-r--r--   0 anton     (1000) anton     (1000)      612 2024-04-01 14:50:35.000000 robot-rumble-stdlib-0.1.2/setup.py
```

### Comparing `robot-rumble-stdlib-0.1.1/LICENSE` & `robot-rumble-stdlib-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robot-rumble-stdlib-0.1.1/PKG-INFO` & `robot-rumble-stdlib-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robot-rumble-stdlib
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/robot-rumble/logic/tree/master/lang-runners/python/stdlib
 Author: Robot Rumble Team
 Author-email: antonoutkine@gmail.com
 License: GNU GPL3
 Project-URL: Documentation, https://rr-docs.readthedocs.io/en/latest/api.html
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### Comparing `robot-rumble-stdlib-0.1.1/robot_rumble_stdlib.egg-info/PKG-INFO` & `robot-rumble-stdlib-0.1.2/robot_rumble_stdlib.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robot-rumble-stdlib
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/robot-rumble/logic/tree/master/lang-runners/python/stdlib
 Author: Robot Rumble Team
 Author-email: antonoutkine@gmail.com
 License: GNU GPL3
 Project-URL: Documentation, https://rr-docs.readthedocs.io/en/latest/api.html
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### Comparing `robot-rumble-stdlib-0.1.1/rumblelib.py` & `robot-rumble-stdlib-0.1.2/rumblelib.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 import enum
 import typing
+import traceback
 
 
 def check_instance(val: typing.Any, cls: typing.Any, func_name: str):
     if not isinstance(val, cls):
         raise TypeError(f"{func_name} argument must be an instance of {cls.__name__}")
 
 
@@ -69,14 +70,17 @@
     @property
     def y(self) -> int:
         return self[1]
 
     def is_spawn(self) -> int:
         return str(self) in SPAWN_COORDS_STRINGS
 
+    def is_hill(self) -> int:
+        return str(self) in HILL_COORDS_STRINGS
+
     def distance_to(self, other: "Coords") -> float:
         import math
         check_instance(other, Coords, "Coords.distance_to")
         return math.sqrt((other.x - self.x) ** 2 + (other.y - self.y) ** 2)
 
     def walking_distance_to(self, other: "Coords") -> int:
         check_instance(other, Coords, "Coords.walking_distance_to")
@@ -118,14 +122,17 @@
     def __mul__(self, n: int) -> "Coords":
         check_instance(n, int, "Coords.__mul__")
         return Coords(self.x * n, self.y * n)
 
 SPAWN_COORDS = set([Coords(1, 5), Coords(1, 6), Coords(1, 7), Coords(1, 8), Coords(1, 9), Coords(1, 10), Coords(1, 11), Coords(1, 12), Coords(1, 13), Coords(2, 4), Coords(2, 14), Coords(3, 3), Coords(3, 15), Coords(4, 2), Coords(4, 16), Coords(5, 1), Coords(5, 17), Coords(6, 1), Coords(6, 17), Coords(7, 1), Coords(7, 17), Coords(8, 1), Coords(8, 17), Coords(9, 1), Coords(9, 17), Coords(10, 1), Coords(10, 17), Coords(11, 1), Coords(11, 17), Coords(12, 1), Coords(12, 17), Coords(13, 1), Coords(13, 17), Coords(14, 2), Coords(14, 16), Coords(15, 3), Coords(15, 15), Coords(16, 4), Coords(16, 14), Coords(17, 5), Coords(17, 6), Coords(17, 7), Coords(17, 8), Coords(17, 9), Coords(17, 10), Coords(17, 11), Coords(17, 12), Coords(17, 13)])
 SPAWN_COORDS_STRINGS = map(str, SPAWN_COORDS)
 
+HILL_COORDS = set([Coords(9, 9), Coords(8, 9), Coords(8, 8), Coords(9, 8), Coords(10, 8), Coords(10, 9), Coords(10, 10), Coords(9, 10), Coords(8, 10)])
+HILL_COORDS_STRINGS = map(str, SPAWN_COORDS)
+
 class Team(enum.Enum):
     Red = "Red"
     Blue = "Blue"
 
     __repr__ = lambda self: self.__str__()
 
     @property
@@ -261,32 +268,31 @@
     def heal(direction: Direction) -> "Action":
         check_instance(direction, Direction, 'Action.heal')
         return Action(ActionType.Heal, direction)
 
 
 MAP_SIZE = 19
 
-
 def __format_err(exc):
     loc = None
     tb = exc.__traceback__
     while tb:
         if tb.tb_frame.f_code.co_filename == "<robot>":
             loc = {
                 "start": (tb.tb_lineno, None),
                 "end": None,
             }
         tb = tb.tb_next
-    import traceback
+
     tb_lines = list(traceback.TracebackException.from_exception(exc).format())
     # from docs: "The message indicating which exception occurred is always the last string in the output."
     return {
         "summary": tb_lines.pop().strip(),
         "details": "".join(tb_lines),
-        "loc": loc,
+        "loc": loc
     }
 
 
 def __main(state, scope=globals()):
     def __validate_function(name, argcount, mandatory):
         f = scope.get(name)
         if not callable(f):
```

### Comparing `robot-rumble-stdlib-0.1.1/setup.py` & `robot-rumble-stdlib-0.1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="robot-rumble-stdlib",
-    version="0.1.1",
+    version="0.1.2",
     license="GNU GPL3",
     author="Robot Rumble Team",
     author_email="antonoutkine@gmail.com",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
```

