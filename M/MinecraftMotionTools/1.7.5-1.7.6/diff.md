# Comparing `tmp/MinecraftMotionTools-1.7.5.tar.gz` & `tmp/MinecraftMotionTools-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MinecraftMotionTools-1.7.5.tar", last modified: Sun Mar 31 22:43:57 2024, max compression
+gzip compressed data, was "MinecraftMotionTools-1.7.6.tar", last modified: Mon Apr  1 14:55:01 2024, max compression
```

## Comparing `MinecraftMotionTools-1.7.5.tar` & `MinecraftMotionTools-1.7.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-03-31 22:43:57.217622 MinecraftMotionTools-1.7.5/
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     1083 2024-03-31 22:34:50.000000 MinecraftMotionTools-1.7.5/LICENSE
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     5458 2024-03-31 22:43:57.208278 MinecraftMotionTools-1.7.5/PKG-INFO
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     5135 2024-03-31 22:34:50.000000 MinecraftMotionTools-1.7.5/README.md
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      481 2024-03-31 22:36:58.000000 MinecraftMotionTools-1.7.5/pyproject.toml
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       38 2024-03-31 22:43:57.219066 MinecraftMotionTools-1.7.5/setup.cfg
-drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-03-31 22:43:57.045714 MinecraftMotionTools-1.7.5/src/
-drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-03-31 22:43:57.193638 MinecraftMotionTools-1.7.5/src/MinecraftMotionTools.egg-info/
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     5458 2024-03-31 22:43:56.000000 MinecraftMotionTools-1.7.5/src/MinecraftMotionTools.egg-info/PKG-INFO
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      301 2024-03-31 22:43:56.000000 MinecraftMotionTools-1.7.5/src/MinecraftMotionTools.egg-info/SOURCES.txt
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        1 2024-03-31 22:43:56.000000 MinecraftMotionTools-1.7.5/src/MinecraftMotionTools.egg-info/dependency_links.txt
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       14 2024-03-31 22:43:56.000000 MinecraftMotionTools-1.7.5/src/MinecraftMotionTools.egg-info/requires.txt
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       23 2024-03-31 22:43:56.000000 MinecraftMotionTools-1.7.5/src/MinecraftMotionTools.egg-info/top_level.txt
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)    10267 2024-03-31 22:42:38.000000 MinecraftMotionTools-1.7.5/src/minecraft_motion_tools.py
+drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-01 14:55:01.740114 MinecraftMotionTools-1.7.6/
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     1083 2024-04-01 14:50:13.000000 MinecraftMotionTools-1.7.6/LICENSE
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     5406 2024-04-01 14:55:01.732113 MinecraftMotionTools-1.7.6/PKG-INFO
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     5083 2024-04-01 14:53:59.000000 MinecraftMotionTools-1.7.6/README.md
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      481 2024-04-01 14:51:52.000000 MinecraftMotionTools-1.7.6/pyproject.toml
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       38 2024-04-01 14:55:01.740694 MinecraftMotionTools-1.7.6/setup.cfg
+drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-01 14:55:01.592615 MinecraftMotionTools-1.7.6/src/
+drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-01 14:55:01.721433 MinecraftMotionTools-1.7.6/src/MinecraftMotionTools.egg-info/
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     5406 2024-04-01 14:55:01.000000 MinecraftMotionTools-1.7.6/src/MinecraftMotionTools.egg-info/PKG-INFO
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      301 2024-04-01 14:55:01.000000 MinecraftMotionTools-1.7.6/src/MinecraftMotionTools.egg-info/SOURCES.txt
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        1 2024-04-01 14:55:01.000000 MinecraftMotionTools-1.7.6/src/MinecraftMotionTools.egg-info/dependency_links.txt
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       14 2024-04-01 14:55:01.000000 MinecraftMotionTools-1.7.6/src/MinecraftMotionTools.egg-info/requires.txt
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       23 2024-04-01 14:55:01.000000 MinecraftMotionTools-1.7.6/src/MinecraftMotionTools.egg-info/top_level.txt
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)    10267 2024-04-01 14:50:13.000000 MinecraftMotionTools-1.7.6/src/minecraft_motion_tools.py
```

### Comparing `MinecraftMotionTools-1.7.5/LICENSE` & `MinecraftMotionTools-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `MinecraftMotionTools-1.7.5/PKG-INFO` & `MinecraftMotionTools-1.7.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MinecraftMotionTools
-Version: 1.7.5
+Version: 1.7.6
 Summary: A library to compute entities' motion in Minecraft.
 Author: OrHy3
 Project-URL: Homepage, https://github.com/OrHy3/MinecraftMotionTools
 Project-URL: Issues, https://github.com/OrHy3/MinecraftMotionTools/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -40,15 +40,15 @@
 |Llama spit|0.05999999865889549|0.009999990463256836|0.009999990463256836|Before|0|
 |Fired arrows and thrown tridents|0.05000000074505806|0.009999990463256836|0.009999990463256836|Before|0|
 |Fireballs, wither skulls and dragon fireballs|0.1|0.050000011920928955|0.050000011920928955|After|0|
 |Dangerous wither skulls|0.1|0.26999998092651367|0.26999998092651367|After|0|
 |Wind charges|0.1|0|0|-|0|
 
 NOTES:
-- For fireballs and alike, use negative velocity and position, since "opposite acceleration" [would be negative for them](https://minecraft.wiki/w/Entity#cite_ref-boom_5-0).
+- For fireballs and alike, use negative acceleration (see [here](https://minecraft.wiki/w/Entity#cite_ref-boom_5-0) why).
 - Players, mobs and armor stands whose OnGround property is set to 1 have an horizontal drag force of 0.45399993658065796.
 - The maximum general velocity value is 10. Any greater value is reset to 0.
 - Minecarts have a maximum horizontal velocity of 0.4. Any greater value is reset to that number.
 - Boats' horizontal position gets updated using next tick's velocity instead of the current one.
 # Function list
 v0: initial velocity<br>
 t: ticks passed<br>
```

### Comparing `MinecraftMotionTools-1.7.5/README.md` & `MinecraftMotionTools-1.7.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 |Llama spit|0.05999999865889549|0.009999990463256836|0.009999990463256836|Before|0|
 |Fired arrows and thrown tridents|0.05000000074505806|0.009999990463256836|0.009999990463256836|Before|0|
 |Fireballs, wither skulls and dragon fireballs|0.1|0.050000011920928955|0.050000011920928955|After|0|
 |Dangerous wither skulls|0.1|0.26999998092651367|0.26999998092651367|After|0|
 |Wind charges|0.1|0|0|-|0|
 
 NOTES:
-- For fireballs and alike, use negative velocity and position, since "opposite acceleration" [would be negative for them](https://minecraft.wiki/w/Entity#cite_ref-boom_5-0).
+- For fireballs and alike, use negative acceleration (see [here](https://minecraft.wiki/w/Entity#cite_ref-boom_5-0) why).
 - Players, mobs and armor stands whose OnGround property is set to 1 have an horizontal drag force of 0.45399993658065796.
 - The maximum general velocity value is 10. Any greater value is reset to 0.
 - Minecarts have a maximum horizontal velocity of 0.4. Any greater value is reset to that number.
 - Boats' horizontal position gets updated using next tick's velocity instead of the current one.
 # Function list
 v0: initial velocity<br>
 t: ticks passed<br>
```

### Comparing `MinecraftMotionTools-1.7.5/src/MinecraftMotionTools.egg-info/PKG-INFO` & `MinecraftMotionTools-1.7.6/src/MinecraftMotionTools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MinecraftMotionTools
-Version: 1.7.5
+Version: 1.7.6
 Summary: A library to compute entities' motion in Minecraft.
 Author: OrHy3
 Project-URL: Homepage, https://github.com/OrHy3/MinecraftMotionTools
 Project-URL: Issues, https://github.com/OrHy3/MinecraftMotionTools/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -40,15 +40,15 @@
 |Llama spit|0.05999999865889549|0.009999990463256836|0.009999990463256836|Before|0|
 |Fired arrows and thrown tridents|0.05000000074505806|0.009999990463256836|0.009999990463256836|Before|0|
 |Fireballs, wither skulls and dragon fireballs|0.1|0.050000011920928955|0.050000011920928955|After|0|
 |Dangerous wither skulls|0.1|0.26999998092651367|0.26999998092651367|After|0|
 |Wind charges|0.1|0|0|-|0|
 
 NOTES:
-- For fireballs and alike, use negative velocity and position, since "opposite acceleration" [would be negative for them](https://minecraft.wiki/w/Entity#cite_ref-boom_5-0).
+- For fireballs and alike, use negative acceleration (see [here](https://minecraft.wiki/w/Entity#cite_ref-boom_5-0) why).
 - Players, mobs and armor stands whose OnGround property is set to 1 have an horizontal drag force of 0.45399993658065796.
 - The maximum general velocity value is 10. Any greater value is reset to 0.
 - Minecarts have a maximum horizontal velocity of 0.4. Any greater value is reset to that number.
 - Boats' horizontal position gets updated using next tick's velocity instead of the current one.
 # Function list
 v0: initial velocity<br>
 t: ticks passed<br>
```

### Comparing `MinecraftMotionTools-1.7.5/src/minecraft_motion_tools.py` & `MinecraftMotionTools-1.7.6/src/minecraft_motion_tools.py`

 * *Files identical despite different names*

