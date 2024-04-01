# Comparing `tmp/dynamic_graphs_with_pygame-1.0.8.tar.gz` & `tmp/dynamic_graphs_with_pygame-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_graphs_with_pygame-1.0.8.tar", last modified: Sat Mar 30 15:42:17 2024, max compression
+gzip compressed data, was "dynamic_graphs_with_pygame-1.0.9.tar", last modified: Mon Apr  1 11:41:59 2024, max compression
```

## Comparing `dynamic_graphs_with_pygame-1.0.8.tar` & `dynamic_graphs_with_pygame-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)        0 2024-03-30 15:42:17.917328 dynamic_graphs_with_pygame-1.0.8/
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)     1092 2024-03-27 15:32:27.000000 dynamic_graphs_with_pygame-1.0.8/LICENSE
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)     4092 2024-03-30 15:42:17.915327 dynamic_graphs_with_pygame-1.0.8/PKG-INFO
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)     3545 2024-03-28 10:16:11.000000 dynamic_graphs_with_pygame-1.0.8/README.md
-drwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)        0 2024-03-30 15:42:17.852316 dynamic_graphs_with_pygame-1.0.8/dynamic_graphs_with_pygame/
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)       81 2024-03-29 14:04:41.000000 dynamic_graphs_with_pygame-1.0.8/dynamic_graphs_with_pygame/__init__.py
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)    27869 2024-03-29 13:27:05.000000 dynamic_graphs_with_pygame-1.0.8/dynamic_graphs_with_pygame/dyn_graphs.py
-drwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)        0 2024-03-30 15:42:17.904315 dynamic_graphs_with_pygame-1.0.8/dynamic_graphs_with_pygame.egg-info/
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)     4092 2024-03-30 15:42:17.000000 dynamic_graphs_with_pygame-1.0.8/dynamic_graphs_with_pygame.egg-info/PKG-INFO
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)      355 2024-03-30 15:42:17.000000 dynamic_graphs_with_pygame-1.0.8/dynamic_graphs_with_pygame.egg-info/SOURCES.txt
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)        1 2024-03-30 15:42:17.000000 dynamic_graphs_with_pygame-1.0.8/dynamic_graphs_with_pygame.egg-info/dependency_links.txt
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)       13 2024-03-30 15:42:17.000000 dynamic_graphs_with_pygame-1.0.8/dynamic_graphs_with_pygame.egg-info/requires.txt
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)       27 2024-03-30 15:42:17.000000 dynamic_graphs_with_pygame-1.0.8/dynamic_graphs_with_pygame.egg-info/top_level.txt
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)       38 2024-03-30 15:42:17.917328 dynamic_graphs_with_pygame-1.0.8/setup.cfg
--rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)      992 2024-03-30 15:41:48.000000 dynamic_graphs_with_pygame-1.0.8/setup.py
+drwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)        0 2024-04-01 11:41:59.647888 dynamic_graphs_with_pygame-1.0.9/
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)     1092 2024-03-27 15:32:27.000000 dynamic_graphs_with_pygame-1.0.9/LICENSE
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)     4092 2024-04-01 11:41:59.646890 dynamic_graphs_with_pygame-1.0.9/PKG-INFO
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)     3545 2024-03-28 10:16:11.000000 dynamic_graphs_with_pygame-1.0.9/README.md
+drwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)        0 2024-04-01 11:41:59.587889 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame/
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)       81 2024-03-29 14:04:41.000000 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame/__init__.py
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)    27822 2024-04-01 11:40:25.000000 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame/dyn_graphs.py
+drwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)        0 2024-04-01 11:41:59.635889 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame.egg-info/
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)     4092 2024-04-01 11:41:59.000000 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame.egg-info/PKG-INFO
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)      355 2024-04-01 11:41:59.000000 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame.egg-info/SOURCES.txt
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)        1 2024-04-01 11:41:59.000000 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame.egg-info/dependency_links.txt
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)       13 2024-04-01 11:41:59.000000 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame.egg-info/requires.txt
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)       27 2024-04-01 11:41:59.000000 dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame.egg-info/top_level.txt
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)       38 2024-04-01 11:41:59.648889 dynamic_graphs_with_pygame-1.0.9/setup.cfg
+-rwxrwxrwx   0 linuxchrisbotos  (1000) linuxchrisbotos  (1000)      992 2024-04-01 11:41:19.000000 dynamic_graphs_with_pygame-1.0.9/setup.py
```

### Comparing `dynamic_graphs_with_pygame-1.0.8/LICENSE` & `dynamic_graphs_with_pygame-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamic_graphs_with_pygame-1.0.8/PKG-INFO` & `dynamic_graphs_with_pygame-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic_graphs_with_pygame
-Version: 1.0.8
+Version: 1.0.9
 Summary: A class for drawing dynamic graphs using Pygame.
 Home-page: https://github.com/ChrisBotos/Dynamic_Graphs_with_Pygame
 Author: Christos Botos
 Author-email: hcty02@gmail.com
 License: UNKNOWN
 Project-URL: LinkedIn, https://www.linkedin.com/in/your_username/
 Keywords: pygame graphs dynamic visualization
```

### Comparing `dynamic_graphs_with_pygame-1.0.8/README.md` & `dynamic_graphs_with_pygame-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dynamic_graphs_with_pygame-1.0.8/dynamic_graphs_with_pygame/dyn_graphs.py` & `dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame/dyn_graphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         - x_tick_marks: The number of x-axis tick marks.
         - y_tick_marks: The number of y-axis tick marks.
         - y_amplifier: The amplification factor for y-values.
         - graph_tick_marks_font: The font for graph tick_marks.
         - graph_tick_marks_text_color: The color of graph tick_mark text.
         - graph_tick_marks_text_space_from_x_axis: Space between text and x-axis.
         - graph_tick_marks_text_space_from_y_axis: Space between text and y-axis.
-        - move_zero_along_x_axis: The number of bins to move the (y==0 & x==0) point to the right or to the left.
+        - move_zero_along_x_axis: The number of values (not bins) to move the (y==0 & x==0) point to the right or to the left.
         - bin_array_is_given_as_x_values: A boolean indicating whether bin_array is given as x_values.
         - have_extra_bin: A boolean indicating whether to include an extra bin when x_values are not perfectly divided into bins.
         """
 
 
         """Comments about specific perhaps confusing parameters"""
         # The x_values can be a numpy array or a python list.
@@ -96,15 +96,15 @@
         # Look at the draw_rect_alpha function in this class for a clever way of drawing semi_transparent objects in pygame.
         #
         # The tick_marks parameters account for the amount of tick_marks along a specific axis.
         #
         # The y_amplifier is a variable that is multiplied with all the y values.
         #
         # The move_zero_along_x_axis parameter allows you to move the (y==0 & x==0) point to the right or to the left.
-        # It is measured in bins, its value showing the start of the bin that should start from 0 to bin_size.
+        # It is measured in actual value not bins.
         #
         # The extra bin accounts for the case where the x_values are not perfectly divided into the bins.
         # For example: raw_x_values = [1,3,0,4,1] with bin_size = 2.
         # The resulting bin_array would be [4,4] ,in case have_extra_bin is False.
         # The resulting bin_array would be [4,4,1] ,in case have_extra_bin is True.
```

### Comparing `dynamic_graphs_with_pygame-1.0.8/dynamic_graphs_with_pygame.egg-info/PKG-INFO` & `dynamic_graphs_with_pygame-1.0.9/dynamic_graphs_with_pygame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-graphs-with-pygame
-Version: 1.0.8
+Version: 1.0.9
 Summary: A class for drawing dynamic graphs using Pygame.
 Home-page: https://github.com/ChrisBotos/Dynamic_Graphs_with_Pygame
 Author: Christos Botos
 Author-email: hcty02@gmail.com
 License: UNKNOWN
 Project-URL: LinkedIn, https://www.linkedin.com/in/your_username/
 Keywords: pygame graphs dynamic visualization
```

### Comparing `dynamic_graphs_with_pygame-1.0.8/setup.py` & `dynamic_graphs_with_pygame-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="dynamic_graphs_with_pygame",
-    version="1.0.8",
+    version="1.0.9",
     description="A class for drawing dynamic graphs using Pygame.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Christos Botos",
     author_email="hcty02@gmail.com",
     url="https://github.com/ChrisBotos/Dynamic_Graphs_with_Pygame",
     packages=find_packages(),  # Use find_packages to automatically discover packages
```

