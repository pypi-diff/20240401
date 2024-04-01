# Comparing `tmp/eduworld-0.0.8.tar.gz` & `tmp/eduworld-0.0.9.tar.gz`

## Comparing `eduworld-0.0.8.tar` & `eduworld-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 eduworld-0.0.8/test_interactive.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 eduworld-0.0.8/test_oop.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 eduworld-0.0.8/test_simple.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 eduworld-0.0.8/tox.ini
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 eduworld-0.0.8/eduworld/__init__.py
--rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 eduworld-0.0.8/eduworld/algoworldboard.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 eduworld-0.0.8/eduworld/application.py
--rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 eduworld-0.0.8/eduworld/board.py
--rw-r--r--   0        0        0     9430 2020-02-02 00:00:00.000000 eduworld-0.0.8/eduworld/canvas.py
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 eduworld-0.0.8/eduworld/robot.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 eduworld-0.0.8/eduworld/tile.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 eduworld-0.0.8/eduworld/tilemap.py
--rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 eduworld-0.0.8/eduworld/simple/__init__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 eduworld-0.0.8/eduworld/worlds/10x1.aww
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 eduworld-0.0.8/eduworld/worlds/10x10.aww
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 eduworld-0.0.8/eduworld/worlds/5x5.aww
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 eduworld-0.0.8/eduworld/worlds/demo-world.aww
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 eduworld-0.0.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 eduworld-0.0.8/LICENSE
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 eduworld-0.0.8/README.md
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 eduworld-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 eduworld-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 eduworld-0.0.9/test_interactive.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 eduworld-0.0.9/test_oop.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 eduworld-0.0.9/test_simple.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 eduworld-0.0.9/tox.ini
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 eduworld-0.0.9/eduworld/__init__.py
+-rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 eduworld-0.0.9/eduworld/algoworldboard.py
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 eduworld-0.0.9/eduworld/application.py
+-rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 eduworld-0.0.9/eduworld/board.py
+-rw-r--r--   0        0        0     9597 2020-02-02 00:00:00.000000 eduworld-0.0.9/eduworld/canvas.py
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 eduworld-0.0.9/eduworld/robot.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 eduworld-0.0.9/eduworld/tile.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 eduworld-0.0.9/eduworld/tilemap.py
+-rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 eduworld-0.0.9/eduworld/simple/__init__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 eduworld-0.0.9/eduworld/worlds/10x1.aww
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 eduworld-0.0.9/eduworld/worlds/10x10.aww
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 eduworld-0.0.9/eduworld/worlds/5x5.aww
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 eduworld-0.0.9/eduworld/worlds/demo-world.aww
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 eduworld-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 eduworld-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 eduworld-0.0.9/README.md
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 eduworld-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 eduworld-0.0.9/PKG-INFO
```

### Comparing `eduworld-0.0.8/test_oop.py` & `eduworld-0.0.9/test_oop.py`

 * *Files identical despite different names*

### Comparing `eduworld-0.0.8/eduworld/__init__.py` & `eduworld-0.0.9/eduworld/__init__.py`

 * *Files identical despite different names*

### Comparing `eduworld-0.0.8/eduworld/algoworldboard.py` & `eduworld-0.0.9/eduworld/algoworldboard.py`

 * *Files identical despite different names*

### Comparing `eduworld-0.0.8/eduworld/application.py` & `eduworld-0.0.9/eduworld/application.py`

 * *Files identical despite different names*

### Comparing `eduworld-0.0.8/eduworld/board.py` & `eduworld-0.0.9/eduworld/board.py`

 * *Files identical despite different names*

### Comparing `eduworld-0.0.8/eduworld/canvas.py` & `eduworld-0.0.9/eduworld/canvas.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         |    \     /    |  innr_shft = cell_size - od
         |     --=-- +   |
         |           oe  |
         +---------------+
         y (cell_size) + shift
         """
         name = f"b-{tile.x}-{tile.y}"
-        diam = self.cell_size * 0.85
+        diam = self.cell_size * 0.75
         ishift = self.cell_size - diam
         os = [shift_x + ishift, shift_y + ishift]
         oe = [shift_x + diam, shift_y + diam]
         c = os + oe
         tags = ("beeper", name)
         self.create_oval(c, width=2, outline="black", fill="gray95", tags=tags)
 
@@ -234,18 +234,22 @@
         for r in self.board.robots:
             if r.canvas is None:
                 r.canvas = self
             self._draw_robot(r)
 
     def _draw_robot(self, r: Robot):
         """Draw robot on the canvas"""
+        scale = self.cell_size / 1.2
+        inner_shift = self.cell_size * 0.05 
         shift_x = (r.x - 1) * self.cell_size + self.x_left
         shift_y = (r.y - 1) * self.cell_size + self.y_top
         fill = r.color
-        tag = (r.name,)
-        coords = [0.3, 0, 0, 0.3, 0.3, 0.6, 0.6, 0.3]
-        coords = [v * self.cell_size for v in coords]
-
-        self.delete(r.name)
-        self.create_polygon(coords, width=1, outline="gray25", fill=fill, tags=tag)
-        self.moveto(r.name, shift_x, shift_y)
-        self.move(r.name, self.cell_size * 0.18, self.cell_size * 0.18)
+        name = r.name
+        outer = [0.5, 0.0, 1.0, 0.5, 0.5, 1.0, 0.0, 0.5, 0.5, 0.0]
+        inner = [0.5, 0.212, 0.788, 0.5, 0.5, 0.788, 0.212, 0.5, 0.5, 0.212]
+        coords = outer + inner
+        coords = [v * scale for v in coords]
+
+        self.delete(name)
+        self.create_polygon(coords, width=1, outline="gray25", fill=fill, tags=name)
+        self.moveto(name, shift_x, shift_y)
+        self.move(name, inner_shift, inner_shift)
```

### Comparing `eduworld-0.0.8/eduworld/robot.py` & `eduworld-0.0.9/eduworld/robot.py`

 * *Files identical despite different names*

### Comparing `eduworld-0.0.8/eduworld/tile.py` & `eduworld-0.0.9/eduworld/tile.py`

 * *Files identical despite different names*

### Comparing `eduworld-0.0.8/eduworld/tilemap.py` & `eduworld-0.0.9/eduworld/tilemap.py`

 * *Files identical despite different names*

### Comparing `eduworld-0.0.8/eduworld/simple/__init__.py` & `eduworld-0.0.9/eduworld/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `eduworld-0.0.8/.gitignore` & `eduworld-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `eduworld-0.0.8/LICENSE` & `eduworld-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eduworld-0.0.8/README.md` & `eduworld-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `eduworld-0.0.8/pyproject.toml` & `eduworld-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EduWorld"
-version = "0.0.8"
+version = "0.0.9"
 description = "Educational package to learn computational thinking and other basic programming concepts"
 long-description = "``EduWorld`` is an educational ``python`` package designed for students to learn computational thinking, algorithms, and other basic programming concepts. \n Through this process they learn how to divide a problem into smaller steps and refine them; to abstract; to recognize patterns; and to design and implement algorithms;"
 readme = "README.md"
 requires-python = ">=3.8"
 license = "GPL-3.0-or-later"
 keywords = ["education", "gamification", "learning", "beginners", "computational thinking"]
 authors = [
```

### Comparing `eduworld-0.0.8/PKG-INFO` & `eduworld-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EduWorld
-Version: 0.0.8
+Version: 0.0.9
 Summary: Educational package to learn computational thinking and other basic programming concepts
 Project-URL: Documentation, https://codeberg.org/helkaraxe/algoworld-python#readme
 Project-URL: Issues, https://codeberg.org/helkaraxe/algoworld-python/issues
 Project-URL: Source, https://codeberg.org/helkaraxe/algoworld-python
 Author-email: Stanislav Grinkov <StanislavGrinkov@users.noreply.codeberg.org>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
```

