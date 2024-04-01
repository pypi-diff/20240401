# Comparing `tmp/wlr_layout_ui-1.4.4.tar.gz` & `tmp/wlr_layout_ui-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlr_layout_ui-1.4.4.tar", max compression
+gzip compressed data, was "wlr_layout_ui-1.4.5.tar", max compression
```

## Comparing `wlr_layout_ui-1.4.4.tar` & `wlr_layout_ui-1.4.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      558 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.4/README.md
--rw-r--r--   0        0        0      636 2024-03-30 19:09:47.058712 wlr_layout_ui-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     2435 2024-02-19 21:26:30.823859 wlr_layout_ui-1.4.4/src/wlr_layout_ui/__init__.py
--rw-r--r--   0        0        0     4304 2023-12-20 15:42:38.511785 wlr_layout_ui-1.4.4/src/wlr_layout_ui/displaywidget.py
--rw-r--r--   0        0        0      387 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.4/src/wlr_layout_ui/factories.py
--rw-r--r--   0        0        0    20966 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.4/src/wlr_layout_ui/gui.py
--rw-r--r--   0        0        0      469 2023-10-24 21:30:47.569956 wlr_layout_ui-1.4.4/src/wlr_layout_ui/profiles.py
--rw-r--r--   0        0        0     5449 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.4/src/wlr_layout_ui/screens.py
--rw-r--r--   0        0        0      274 2023-10-31 19:56:35.664588 wlr_layout_ui-1.4.4/src/wlr_layout_ui/settings.py
--rw-r--r--   0        0        0     1706 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.4/src/wlr_layout_ui/shapes.py
--rw-r--r--   0        0        0     4496 2024-03-30 19:09:30.198398 wlr_layout_ui-1.4.4/src/wlr_layout_ui/utils.py
--rw-r--r--   0        0        0    12366 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.4/src/wlr_layout_ui/widgets.py
--rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 wlr_layout_ui-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0      558 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.5/README.md
+-rw-r--r--   0        0        0      636 2024-04-01 15:31:36.231423 wlr_layout_ui-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     2435 2024-02-19 21:26:30.823859 wlr_layout_ui-1.4.5/src/wlr_layout_ui/__init__.py
+-rw-r--r--   0        0        0     4304 2023-12-20 15:42:38.511785 wlr_layout_ui-1.4.5/src/wlr_layout_ui/displaywidget.py
+-rw-r--r--   0        0        0      387 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.5/src/wlr_layout_ui/factories.py
+-rw-r--r--   0        0        0    21897 2024-04-01 15:30:20.126238 wlr_layout_ui-1.4.5/src/wlr_layout_ui/gui.py
+-rw-r--r--   0        0        0      469 2023-10-24 21:30:47.569956 wlr_layout_ui-1.4.5/src/wlr_layout_ui/profiles.py
+-rw-r--r--   0        0        0     5449 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.5/src/wlr_layout_ui/screens.py
+-rw-r--r--   0        0        0      274 2023-10-31 19:56:35.664588 wlr_layout_ui-1.4.5/src/wlr_layout_ui/settings.py
+-rw-r--r--   0        0        0     1706 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.5/src/wlr_layout_ui/shapes.py
+-rw-r--r--   0        0        0     4496 2024-03-30 19:09:30.198398 wlr_layout_ui-1.4.5/src/wlr_layout_ui/utils.py
+-rw-r--r--   0        0        0    12366 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.5/src/wlr_layout_ui/widgets.py
+-rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 wlr_layout_ui-1.4.5/PKG-INFO
```

### Comparing `wlr_layout_ui-1.4.4/README.md` & `wlr_layout_ui-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.4/pyproject.toml` & `wlr_layout_ui-1.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wlr-layout-ui"
-version = "1.4.4"
+version = "1.4.5"
 description = "A tiny GUI to configure screen layouts on wayland"
 authors = ["fdev31 <fdev31@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/fdev31/wlr-layout-ui"
 packages = [{include = "wlr_layout_ui", from = "src"}]
 
 [tool.poetry.scripts]
```

### Comparing `wlr_layout_ui-1.4.4/src/wlr_layout_ui/__init__.py` & `wlr_layout_ui-1.4.5/src/wlr_layout_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.4/src/wlr_layout_ui/displaywidget.py` & `wlr_layout_ui-1.4.5/src/wlr_layout_ui/displaywidget.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.4/src/wlr_layout_ui/gui.py` & `wlr_layout_ui-1.4.5/src/wlr_layout_ui/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,37 +360,62 @@
         pyglet.window.Window.on_resize(self, width, height)
 
         for w in self._widgets:
             w.update_alignment(0, 0, width, height)
 
         self.center_layout(immediate=True)
 
+        self._confirm_labels = None
+
     def on_mouse_release(self, x, y, button, modifiers):
         if self.selected_item and self.selected_item.dragging:
             self.snap_active_screen()
             self.selected_item.dragging = False
             self.center_layout()
         if self.selected_item:
             self.on_off_but.toggled = not self.selected_item.screen.active
 
     def draw_countdown(self):
         delay = time.time() - self.confirmation_needed
         if delay >= CONFIRM_DELAY:
             os.system(self.original_cmd)
             self.confirmation_needed = False
-            return
-
-        w, h = self.get_size()
-        pyglet.text.Label(
-            f"Press ENTER to confirm ({CONFIRM_DELAY-delay:.2f}s left) ",
-            font_size=24,
-            x=10,
-            y=h // 2 + 40,
-            align="center",
-        ).draw()
+        else:
+            color = (200, 200, 200, 255)
+            w, h = self.get_size()
+            remaining = CONFIRM_DELAY - delay
+            ratio = remaining / CONFIRM_DELAY
+
+            pyglet.shapes.Rectangle(
+                0,
+                h // 2 - 40,
+                int(w * ratio),
+                10,
+                color=(50 + int(200 * (1.0 - ratio)), int(200 * ratio), 100, 255),
+            ).draw()
+            if getattr(self, "_confirm_labels", None):
+                lbl1, lbl2 = self._confirm_labels
+            else:
+                lbl1 = pyglet.text.HTMLLabel(
+                    "Press <b>ENTER</b>",
+                    x=WINDOW_MARGIN,
+                    y=h // 2 + 40,
+                )
+                lbl1.set_style("color", color)
+                lbl1.font_size = 40
+                lbl2 = pyglet.text.Label(
+                    "to confirm (or ESCAPE to abort)",
+                    font_size=20,
+                    color=color,
+                    x=WINDOW_MARGIN,
+                    y=h // 2,
+                )
+                self._confirm_labels = (lbl1, lbl2)
+            lbl1.draw()
+            lbl2.draw()
 
     def draw_text_input(self):
         w, h = self.get_size()
         pyglet.text.Label(
             "Profile name: ", font_size=24, x=10, y=h // 2 + 40, align="left"
         ).draw()
         text = self.text_input
@@ -421,22 +446,23 @@
 
     def on_draw(self):
         self.clear()
         # Draw a grey background
         pyglet.shapes.Rectangle(
             0, 0, self.width, self.height, color=(50, 50, 50, 255)
         ).draw()
+
         # Higher priority modes
         if self.text_input is not None:
             self.draw_text_input()
         elif self.confirmation_needed:
             self.draw_countdown()
         else:
             self.draw_screens_and_widgets()
-        self.draw_status_label()
+            self.draw_status_label()
 
     def draw_status_label(self):
         text = None
         color = (200, 200, 200, 255)
 
         if self.error_message:
             self.error_message_duration -= 1
```

### Comparing `wlr_layout_ui-1.4.4/src/wlr_layout_ui/screens.py` & `wlr_layout_ui-1.4.5/src/wlr_layout_ui/screens.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.4/src/wlr_layout_ui/shapes.py` & `wlr_layout_ui-1.4.5/src/wlr_layout_ui/shapes.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.4/src/wlr_layout_ui/utils.py` & `wlr_layout_ui-1.4.5/src/wlr_layout_ui/utils.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.4/src/wlr_layout_ui/widgets.py` & `wlr_layout_ui-1.4.5/src/wlr_layout_ui/widgets.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.4/PKG-INFO` & `wlr_layout_ui-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wlr-layout-ui
-Version: 1.4.4
+Version: 1.4.5
 Summary: A tiny GUI to configure screen layouts on wayland
 Home-page: https://github.com/fdev31/wlr-layout-ui
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

