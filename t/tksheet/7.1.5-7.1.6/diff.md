# Comparing `tmp/tksheet-7.1.5.tar.gz` & `tmp/tksheet-7.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-7.1.5.tar", last modified: Sat Mar 30 19:46:45 2024, max compression
+gzip compressed data, was "tksheet-7.1.6.tar", last modified: Mon Apr  1 18:46:23 2024, max compression
```

## Comparing `tksheet-7.1.5.tar` & `tksheet-7.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-03-30 19:46:45.658224 tksheet-7.1.5/
--rw-rw-r--   0 rg        (1000) rg        (1000)     1101 2024-01-20 17:50:45.000000 tksheet-7.1.5/LICENSE.txt
--rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-03-30 19:46:45.658224 tksheet-7.1.5/PKG-INFO
--rw-rw-r--   0 rg        (1000) rg        (1000)     3914 2024-01-30 18:05:54.000000 tksheet-7.1.5/README.md
--rw-rw-r--   0 rg        (1000) rg        (1000)     1064 2024-03-28 19:13:12.000000 tksheet-7.1.5/pyproject.toml
--rw-rw-r--   0 rg        (1000) rg        (1000)       38 2024-03-30 19:46:45.658224 tksheet-7.1.5/setup.cfg
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-03-30 19:46:45.658224 tksheet-7.1.5/tksheet/
--rw-rw-r--   0 rg        (1000) rg        (1000)     1874 2024-03-28 19:13:12.000000 tksheet-7.1.5/tksheet/__init__.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    51594 2024-01-25 08:44:04.000000 tksheet-7.1.5/tksheet/colors.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    99272 2024-03-30 19:40:33.000000 tksheet-7.1.5/tksheet/column_headers.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    10037 2024-01-25 08:44:04.000000 tksheet-7.1.5/tksheet/formatters.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    39245 2024-03-30 18:36:12.000000 tksheet-7.1.5/tksheet/functions.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   318511 2024-03-30 19:37:07.000000 tksheet-7.1.5/tksheet/main_table.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    13604 2024-03-30 16:31:45.000000 tksheet-7.1.5/tksheet/other_classes.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   103990 2024-03-30 19:38:50.000000 tksheet-7.1.5/tksheet/row_index.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   256866 2024-03-30 18:50:14.000000 tksheet-7.1.5/tksheet/sheet.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    11906 2024-03-19 09:32:45.000000 tksheet-7.1.5/tksheet/sheet_options.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     6681 2024-03-30 19:35:35.000000 tksheet-7.1.5/tksheet/text_editor.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    13398 2024-03-19 10:12:20.000000 tksheet-7.1.5/tksheet/themes.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     8275 2024-02-08 18:45:37.000000 tksheet-7.1.5/tksheet/top_left_rectangle.py
--rw-rw-r--   0 rg        (1000) rg        (1000)      340 2024-01-25 08:44:04.000000 tksheet-7.1.5/tksheet/types.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     2092 2024-03-23 14:39:32.000000 tksheet-7.1.5/tksheet/vars.py
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-03-30 19:46:45.658224 tksheet-7.1.5/tksheet.egg-info/
--rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-03-30 19:46:45.000000 tksheet-7.1.5/tksheet.egg-info/PKG-INFO
--rw-rw-r--   0 rg        (1000) rg        (1000)      481 2024-03-30 19:46:45.000000 tksheet-7.1.5/tksheet.egg-info/SOURCES.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)        1 2024-03-30 19:46:45.000000 tksheet-7.1.5/tksheet.egg-info/dependency_links.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)        8 2024-03-30 19:46:45.000000 tksheet-7.1.5/tksheet.egg-info/top_level.txt
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-01 18:46:23.587094 tksheet-7.1.6/
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1101 2024-01-20 17:50:45.000000 tksheet-7.1.6/LICENSE.txt
+-rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-04-01 18:46:23.587094 tksheet-7.1.6/PKG-INFO
+-rw-rw-r--   0 rg        (1000) rg        (1000)     3914 2024-01-30 18:05:54.000000 tksheet-7.1.6/README.md
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1064 2024-03-31 10:01:25.000000 tksheet-7.1.6/pyproject.toml
+-rw-rw-r--   0 rg        (1000) rg        (1000)       38 2024-04-01 18:46:23.587094 tksheet-7.1.6/setup.cfg
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-01 18:46:23.583094 tksheet-7.1.6/tksheet/
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1874 2024-03-31 10:01:25.000000 tksheet-7.1.6/tksheet/__init__.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    51594 2024-01-25 08:44:04.000000 tksheet-7.1.6/tksheet/colors.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    99449 2024-04-01 08:20:52.000000 tksheet-7.1.6/tksheet/column_headers.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    10037 2024-01-25 08:44:04.000000 tksheet-7.1.6/tksheet/formatters.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    39610 2024-04-01 08:19:58.000000 tksheet-7.1.6/tksheet/functions.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   321201 2024-04-01 18:36:21.000000 tksheet-7.1.6/tksheet/main_table.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    13604 2024-03-30 16:31:45.000000 tksheet-7.1.6/tksheet/other_classes.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   104750 2024-04-01 18:30:11.000000 tksheet-7.1.6/tksheet/row_index.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   257417 2024-04-01 18:28:12.000000 tksheet-7.1.6/tksheet/sheet.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    11906 2024-03-19 09:32:45.000000 tksheet-7.1.6/tksheet/sheet_options.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     6681 2024-03-30 19:35:35.000000 tksheet-7.1.6/tksheet/text_editor.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    13398 2024-03-19 10:12:20.000000 tksheet-7.1.6/tksheet/themes.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     8275 2024-02-08 18:45:37.000000 tksheet-7.1.6/tksheet/top_left_rectangle.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)      340 2024-01-25 08:44:04.000000 tksheet-7.1.6/tksheet/types.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     2092 2024-03-23 14:39:32.000000 tksheet-7.1.6/tksheet/vars.py
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-01 18:46:23.587094 tksheet-7.1.6/tksheet.egg-info/
+-rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-04-01 18:46:23.000000 tksheet-7.1.6/tksheet.egg-info/PKG-INFO
+-rw-rw-r--   0 rg        (1000) rg        (1000)      481 2024-04-01 18:46:23.000000 tksheet-7.1.6/tksheet.egg-info/SOURCES.txt
+-rw-rw-r--   0 rg        (1000) rg        (1000)        1 2024-04-01 18:46:23.000000 tksheet-7.1.6/tksheet.egg-info/dependency_links.txt
+-rw-rw-r--   0 rg        (1000) rg        (1000)        8 2024-04-01 18:46:23.000000 tksheet-7.1.6/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-7.1.5/LICENSE.txt` & `tksheet-7.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.5/PKG-INFO` & `tksheet-7.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 7.1.5
+Version: 7.1.6
 Summary: Tkinter table / sheet widget
 Author-email: ragardner <github@ragardner.simplelogin.com>
 License: Copyright (c) 2019 ragardner and open source contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `tksheet-7.1.5/README.md` & `tksheet-7.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.5/pyproject.toml` & `tksheet-7.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tksheet"
 description = "Tkinter table / sheet widget"
 readme = "README.md"
-version = "7.1.5"
+version = "7.1.6"
 authors = [{ name = "ragardner", email = "github@ragardner.simplelogin.com" }]
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["tkinter", "table", "widget", "sheet", "grid", "tk"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `tksheet-7.1.5/tksheet/__init__.py` & `tksheet-7.1.6/tksheet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ruff: noqa: F401
 
 """
 tksheet - A Python tkinter table widget
 """
 
-__version__ = "7.1.5"
+__version__ = "7.1.6"
 
 from .colors import (
     color_map,
 )
 from .column_headers import ColumnHeaders
 from .formatters import (
     Formatter,
```

### Comparing `tksheet-7.1.5/tksheet/colors.py` & `tksheet-7.1.6/tksheet/colors.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.5/tksheet/column_headers.py` & `tksheet-7.1.6/tksheet/column_headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,22 @@
     partial,
 )
 from itertools import (
     cycle,
     islice,
 )
 from math import ceil, floor
+from typing import Literal
 
 from .colors import (
     color_map,
 )
 from .formatters import is_bool_like, try_to_bool
 from .functions import (
-    consecutive_chunks,
+    consecutive_ranges,
     ev_stack_dict,
     event_dict,
     get_checkbox_points,
     get_n2a,
     is_contiguous,
     try_binding,
 )
@@ -683,18 +684,18 @@
             xpos,
             self.current_height,
             width=3,
             fill=self.PAR.ops.drag_and_drop_bg,
             tag="move_columns",
         )
         self.MT.create_resize_line(xpos, y1, xpos, y2, width=3, fill=self.PAR.ops.drag_and_drop_bg, tag="move_columns")
-        for chunk in consecutive_chunks(cols):
+        for boxst, boxend in consecutive_ranges(cols):
             self.MT.show_ctrl_outline(
-                start_cell=(chunk[0], 0),
-                end_cell=(chunk[-1] + 1, len(self.MT.row_positions) - 1),
+                start_cell=(boxst, 0),
+                end_cell=(boxend, len(self.MT.row_positions) - 1),
                 dash=(),
                 outline=self.PAR.ops.drag_and_drop_bg,
                 delete_on_timer=False,
             )
 
     def hide_resize_and_ctrl_lines(self, ctrl_lines=True):
         self.delete_resize_lines()
@@ -1618,22 +1619,21 @@
         c: int = 0,
         text: object = None,
         state: str = "normal",
         dropdown: bool = False,
     ) -> bool:
         text = None
         extra_func_key = "??"
-        datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
         if event is None or self.MT.event_opens_dropdown_or_checkbox(event):
             if event is not None:
                 if hasattr(event, "keysym") and event.keysym == "Return":
                     extra_func_key = "Return"
                 elif hasattr(event, "keysym") and event.keysym == "F2":
                     extra_func_key = "F2"
-            text = self.get_cell_data(datacn, none_to_empty_str=True, redirect_int=True)
+            text = self.get_cell_data(self.MT.datacn(c), none_to_empty_str=True, redirect_int=True)
         elif event is not None and (
             (hasattr(event, "keysym") and event.keysym == "BackSpace") or event.keycode in (8, 855638143)
         ):
             extra_func_key = "BackSpace"
             text = ""
         elif event is not None and (
             (hasattr(event, "char") and event.char.isalpha())
@@ -1675,17 +1675,16 @@
             self.hide_text_editor()
         if not self.MT.see(r=0, c=c, keep_yscroll=True, check_cell_visibility=True):
             self.MT.refresh()
         x = self.MT.col_positions[c] + 1
         y = 0
         w = self.MT.col_positions[c + 1] - x
         h = self.current_height + 1
-        datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
         if text is None:
-            text = self.get_cell_data(datacn, none_to_empty_str=True, redirect_int=True)
+            text = self.get_cell_data(self.MT.datacn(c), none_to_empty_str=True, redirect_int=True)
         bg, fg = self.PAR.ops.header_bg, self.PAR.ops.header_fg
         kwargs = {
             "menu_kwargs": DotDict(
                 {
                     "font": self.PAR.ops.table_font,
                     "foreground": self.PAR.ops.popup_menu_fg,
                     "background": self.PAR.ops.popup_menu_bg,
@@ -1750,15 +1749,15 @@
         curr_height = self.text_editor.window.winfo_height()
         if curr_height < self.MT.min_header_height:
             return
         if (
             not check_lines
             or self.MT.get_lines_cell_height(
                 self.text_editor.window.get_num_lines() + 1,
-                font=self.PAR.ops.header_font,
+                font=self.text_editor.tktext.cget("font"),
             )
             > curr_height
         ):
             new_height = curr_height + self.MT.header_xtra_lines_increment
             space_bot = self.MT.get_space_bot(0)
             if new_height > space_bot:
                 new_height = space_bot
@@ -1770,44 +1769,53 @@
                     self.coords(
                         self.dropdown.canvas_id,
                         self.MT.col_positions[c],
                         new_height - 1,
                     )
                     self.itemconfig(self.dropdown.canvas_id, anchor=anchor, height=win_h)
 
-    def refresh_open_window_positions(self):
+    def refresh_open_window_positions(self, zoom: Literal["in", "out"]):
         if self.text_editor.open:
             c = self.text_editor.column
-            self.text_editor.window.config(height=self.MT.col_positions[c + 1] - self.MT.col_positions[c])
+            self.text_editor.window.config(
+                height=self.current_height,
+                width=self.MT.col_positions[c + 1] - self.MT.col_positions[c] + 1,
+            )
+            self.text_editor.tktext.config(font=self.PAR.ops.header_font)
             self.coords(
                 self.text_editor.canvas_id,
-                0,
                 self.MT.col_positions[c],
+                0,
             )
         if self.dropdown.open:
+            if zoom == "in":
+                self.dropdown.window.zoom_in()
+            elif zoom == "out":
+                self.dropdown.window.zoom_out()
             c = self.dropdown.get_coords()
             if self.text_editor.open:
                 text_editor_h = self.text_editor.window.winfo_height()
                 win_h, anchor = self.get_dropdown_height_anchor(c, text_editor_h)
             else:
-                text_editor_h = self.MT.col_positions[c + 1] - self.MT.col_positions[c]
+                text_editor_h = self.current_height
                 anchor = self.itemcget(self.dropdown.canvas_id, "anchor")
                 # win_h = 0
+            self.dropdown.window.config(width=self.MT.col_positions[c + 1] - self.MT.col_positions[c] + 1)
             if anchor == "nw":
                 self.coords(
                     self.dropdown.canvas_id,
-                    0,
-                    self.MT.col_positions[c] + text_editor_h - 1,
+                    self.MT.col_positions[c],
+                    text_editor_h - 1,
                 )
                 # self.itemconfig(self.dropdown.canvas_id, anchor=anchor, height=win_h)
             elif anchor == "sw":
                 self.coords(
                     self.dropdown.canvas_id,
-                    0,
                     self.MT.col_positions[c],
+                    0,
                 )
                 # self.itemconfig(self.dropdown.canvas_id, anchor=anchor, height=win_h)
 
     def hide_text_editor(self, reason: None | str = None) -> None:
         if self.text_editor.open:
             self.itemconfig(self.text_editor.canvas_id, state="hidden")
             self.text_editor.open = False
@@ -1897,19 +1905,17 @@
         event: dict,
         modified_func: Callable | None,
     ) -> None:
         if modified_func:
             modified_func(event)
         dd_window.search_and_see(event)
 
-    def open_dropdown_window(self, c, datacn=None, event: object = None):
+    def open_dropdown_window(self, c, event: object = None):
         self.hide_text_editor("Escape")
-        if datacn is None:
-            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-        kwargs = self.get_cell_kwargs(datacn, key="dropdown")
+        kwargs = self.get_cell_kwargs(self.MT.datacn(c), key="dropdown")
         if kwargs["state"] == "normal":
             if not self.open_text_editor(event=event, c=c, dropdown=True):
                 return
         win_h, anchor = self.get_dropdown_height_anchor(c)
         win_w = self.MT.col_positions[c + 1] - self.MT.col_positions[c] + 1
         ypos = self.current_height - 1
         reset_kwargs = {
```

### Comparing `tksheet-7.1.5/tksheet/formatters.py` & `tksheet-7.1.6/tksheet/formatters.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.5/tksheet/functions.py` & `tksheet-7.1.6/tksheet/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,14 +241,20 @@
     try:
         iter(o)
         return True
     except Exception:
         return False
 
 
+def int_x_iter(i: Iterator[int] | int) -> Iterator[int]:
+    if isinstance(i, int):
+        return (i,)
+    return i
+
+
 def unpack(t: tuple[object] | tuple[Iterator[object]]) -> tuple[object]:
     if not len(t):
         return t
     if is_iterable(t[0]) and len(t) == 1:
         return t[0]
     return t
 
@@ -341,29 +347,35 @@
     if reverse_gap is not None:
         seq = seq[reverse_gap:]
     if get_st_end:
         return seq[0], seq[-1]
     return seq
 
 
-def consecutive_chunks(seq: list[object]) -> Generator[object]:
-    if not seq:
-        yield seq
+def consecutive_chunks(seq: list[int]) -> Generator[list[int]]:
     start = 0
-    end = 0
-    for index, value in enumerate(seq):
-        if index < len(seq) - 1:
-            if seq[index + 1] > value + 1:
-                end = index + 1
-                yield seq[start:end]
-                start = end
-        else:
+    for index, value in enumerate(seq, 1):
+        try:
+            if seq[index] > value + 1:
+                yield seq[start:(start := index)]
+        except Exception:
             yield seq[start : len(seq)]
 
 
+def consecutive_ranges(seq: Sequence[int]) -> Generator[tuple[int, int]]:
+    start = 0
+    for index, value in enumerate(seq, 1):
+        try:
+            if seq[index] > value + 1:
+                yield seq[start], seq[index - 1] + 1
+                start = index
+        except Exception:
+            yield seq[start], seq[-1] + 1
+
+
 def is_contiguous(seq: list[int]) -> bool:
     itr = iter(seq)
     prev = next(itr)
     return all(i == (prev := prev + 1) for i in itr)
 
 
 def get_last(
```

### Comparing `tksheet-7.1.5/tksheet/main_table.py` & `tksheet-7.1.6/tksheet/main_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,26 +45,27 @@
     format_data,
     get_clipboard_data,
     get_data_with_valid_check,
     is_bool_like,
     try_to_bool,
 )
 from .functions import (
-    consecutive_chunks,
+    consecutive_ranges,
     decompress_load,
     diff_gen,
     diff_list,
     ev_stack_dict,
     event_dict,
     gen_formatted,
     get_checkbox_points,
     get_new_indexes,
     get_seq_without_gaps_at_index,
     index_exists,
     insert_items,
+    int_x_iter,
     is_iterable,
     is_type_int,
     len_to_idx,
     mod_event_val,
     mod_span,
     move_elements_by_mapping,
     pickle_obj,
@@ -956,20 +957,20 @@
                             disp_new_idxs.values(),
                             disp_new_idxs,
                         )
                     ),
                 )
             )
             if create_selections:
-                for chunk in consecutive_chunks(sorted(disp_new_idxs.values())):
+                for boxst, boxend in consecutive_ranges(sorted(disp_new_idxs.values())):
                     self.create_selection_box(
                         0,
-                        chunk[0],
+                        boxst,
                         len(self.row_positions) - 1,
-                        chunk[-1] + 1,
+                        boxend,
                         "columns",
                         run_binding=True,
                     )
         if move_data:
             self.data[:] = [
                 move_elements_by_mapping(
                     r,
@@ -1177,19 +1178,19 @@
                             disp_new_idxs.values(),
                             disp_new_idxs,
                         )
                     ),
                 )
             )
             if create_selections:
-                for chunk in consecutive_chunks(sorted(disp_new_idxs.values())):
+                for boxst, boxend in consecutive_ranges(sorted(disp_new_idxs.values())):
                     self.create_selection_box(
-                        chunk[0],
+                        boxst,
                         0,
-                        chunk[-1] + 1,
+                        boxend,
                         len(self.col_positions) - 1,
                         "rows",
                         run_binding=True,
                     )
         if move_data:
             self.data[:] = move_elements_by_mapping(
                 self.data,
@@ -1842,15 +1843,14 @@
                                 r + 1,
                                 0,
                                 r2,
                                 len(self.col_positions) - 1,
                                 "rows",
                                 set_current=resel and to_sel >= r + 1 and to_sel < r2,
                             )
-                    break
         elif isinstance(c, int) and r is None and cell is None:
             for item, box in self.get_selection_items(rows=False, cells=False):
                 r1, c1, r2, c2 = box.coords
                 if c >= c1 and c < c2:
                     resel = self.selected.fill_iid == item
                     to_sel = self.selected.column
                     self.hide_selection_box(item)
@@ -1886,31 +1886,73 @@
                                 0,
                                 c + 1,
                                 len(self.row_positions) - 1,
                                 c2,
                                 "columns",
                                 set_current=resel and to_sel >= c + 1 and to_sel < c2,
                             )
-                    break
         elif (isinstance(r, int) and isinstance(c, int) and cell is None) or cell is not None:
             if cell is not None:
                 r, c = cell[0], cell[1]
             for item, box in self.get_selection_items(reverse=True):
                 r1, c1, r2, c2 = box.coords
                 if r >= r1 and c >= c1 and r < r2 and c < c2:
                     self.hide_selection_box(item)
-                    break
         if redraw:
             self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
         sel_event = self.get_select_event(being_drawn_item=self.being_drawn_item)
         if run_binding:
             try_binding(self.deselection_binding_func, sel_event)
         self.PAR.emit_event("<<SheetSelect>>", data=sel_event)
 
-    def page_UP(self, event=None):
+    def deselect_any(
+        self,
+        rows: Iterator[int] | int | None = None,
+        columns: Iterator[int] | int | None = None,
+        redraw: bool = True,
+    ) -> None:
+        rows = int_x_iter(rows)
+        columns = int_x_iter(columns)
+        if is_iterable(rows) and is_iterable(columns):
+            rows = tuple(consecutive_ranges(sorted(rows)))
+            columns = tuple(consecutive_ranges(sorted(columns)))
+            for item, box in self.get_selection_items(reverse=True):
+                r1, c1, r2, c2 = box.coords
+                hidden = False
+                for rows_st, rows_end in rows:
+                    if hidden:
+                        break
+                    for cols_st, cols_end in columns:
+                        if ((rows_end >= r1 and rows_end <= r2) or (rows_st >= r1 and rows_st < r2)) and (
+                            (cols_end >= c1 and cols_end <= c2) or (cols_st >= c1 and cols_st < c2)
+                        ):
+                            hidden = self.hide_selection_box(item)
+                            break
+        elif is_iterable(rows):
+            rows = tuple(consecutive_ranges(sorted(rows)))
+            for item, box in self.get_selection_items(reverse=True):
+                r1, c1, r2, c2 = box.coords
+                for rows_st, rows_end in rows:
+                    if (rows_end >= r1 and rows_end <= r2) or (rows_st >= r1 and rows_st < r2):
+                        self.hide_selection_box(item)
+                        break
+        elif is_iterable(columns):
+            columns = tuple(consecutive_ranges(sorted(columns)))
+            for item, box in self.get_selection_items(reverse=True):
+                r1, c1, r2, c2 = box.coords
+                for cols_st, cols_end in columns:
+                    if (cols_end >= c1 and cols_end <= c2) or (cols_st >= c1 and cols_st < c2):
+                        self.hide_selection_box(item)
+                        break
+        else:
+            self.deselect()
+        if redraw:
+            self.refresh()
+
+    def page_UP(self, event: object = None) -> None:
         height = self.winfo_height()
         top = self.canvasy(0)
         scrollto_y = top - height
         if scrollto_y < 0:
             scrollto_y = 0
         if self.PAR.ops.page_up_down_select_row:
             r = bisect_left(self.row_positions, scrollto_y)
@@ -1931,15 +1973,15 @@
                 self.select_cell(r, c)
         else:
             args = ("moveto", scrollto_y / (self.row_positions[-1] + 100))
             self.yview(*args)
             self.RI.yview(*args)
             self.main_table_redraw_grid_and_text(redraw_row_index=True)
 
-    def page_DOWN(self, event=None):
+    def page_DOWN(self, event: object = None) -> None:
         height = self.winfo_height()
         top = self.canvasy(0)
         scrollto = top + height
         if self.PAR.ops.page_up_down_select_row and self.RI.row_selection_enabled:
             r = bisect_left(self.row_positions, scrollto) - 1
             if self.selected and self.selected.row == r:
                 r += 1
@@ -1961,15 +2003,15 @@
             if scrollto > end + 100:
                 scrollto = end
             args = ("moveto", scrollto / (end + 100))
             self.yview(*args)
             self.RI.yview(*args)
             self.main_table_redraw_grid_and_text(redraw_row_index=True)
 
-    def arrowkey_UP(self, event=None):
+    def arrowkey_UP(self, event: object = None) -> None:
         if not self.selected:
             return
         if self.selected.type_ == "rows":
             r = self.selected.row
             if r and self.RI.row_selection_enabled:
                 if self.cell_completely_visible(r=r - 1, c=0):
                     self.RI.select_row(r - 1, redraw=True)
@@ -1985,15 +2027,15 @@
             elif r and (self.single_selection_enabled or self.toggle_selection_enabled):
                 if self.cell_completely_visible(r=r - 1, c=c):
                     self.select_cell(r - 1, c, redraw=True)
                 else:
                     self.select_cell(r - 1, c)
                     self.see(r - 1, c, keep_xscroll=True, check_cell_visibility=False)
 
-    def arrowkey_DOWN(self, event=None):
+    def arrowkey_DOWN(self, event: object = None) -> None:
         if not self.selected:
             return
         if self.selected.type_ == "rows":
             r = self.selected.row
             if r < len(self.row_positions) - 2 and self.RI.row_selection_enabled:
                 if self.cell_completely_visible(r=min(r + 2, len(self.row_positions) - 2), c=0):
                     self.RI.select_row(r + 1, redraw=True)
@@ -2064,15 +2106,15 @@
                             r + 1,
                             c,
                             keep_xscroll=True,
                             bottom_right_corner=False if self.PAR.ops.arrow_key_down_right_scroll_page else True,
                             check_cell_visibility=False,
                         )
 
-    def arrowkey_LEFT(self, event=None):
+    def arrowkey_LEFT(self, event: object = None) -> None:
         if not self.selected:
             return
         if self.selected.type_ == "columns":
             c = self.selected.column
             if c and self.CH.col_selection_enabled:
                 if self.cell_completely_visible(r=0, c=c - 1):
                     self.CH.select_col(c - 1, redraw=True)
@@ -2096,15 +2138,15 @@
             elif c and (self.single_selection_enabled or self.toggle_selection_enabled):
                 if self.cell_completely_visible(r=r, c=c - 1):
                     self.select_cell(r, c - 1, redraw=True)
                 else:
                     self.select_cell(r, c - 1)
                     self.see(r, c - 1, keep_yscroll=True, check_cell_visibility=False)
 
-    def arrowkey_RIGHT(self, event=None):
+    def arrowkey_RIGHT(self, event: object = None) -> None:
         if not self.selected:
             return
         if self.selected.type_ == "rows":
             r = self.selected.row
             if self.single_selection_enabled or self.toggle_selection_enabled:
                 if self.selected.column == len(self.col_positions) - 2:
                     c = self.selected.column
@@ -3218,33 +3260,37 @@
             self.xview_scroll(-1, "units")
             self.CH.xview_scroll(-1, "units")
             self.x_move_synced_scrolls("moveto", self.xview()[0])
         self.main_table_redraw_grid_and_text(redraw_header=True)
 
     def ctrl_mousewheel(self, event):
         if event.delta < 0 or event.num == 5:
-            if self.PAR.ops.table_font[1] < 2 or self.PAR.ops.index_font[1] < 2 or self.PAR.ops.header_font[1] < 2:
-                return
             self.zoom_out()
         elif event.delta >= 0 or event.num == 4:
             self.zoom_in()
 
     def zoom_in(self, event=None):
         self.zoom_font(
             (self.PAR.ops.table_font[0], self.PAR.ops.table_font[1] + 1, self.PAR.ops.table_font[2]),
+            (self.PAR.ops.index_font[0], self.PAR.ops.index_font[1] + 1, self.PAR.ops.index_font[2]),
             (self.PAR.ops.header_font[0], self.PAR.ops.header_font[1] + 1, self.PAR.ops.header_font[2]),
+            "in",
         )
 
     def zoom_out(self, event=None):
+        if self.PAR.ops.table_font[1] < 2 or self.PAR.ops.index_font[1] < 2 or self.PAR.ops.header_font[1] < 2:
+            return
         self.zoom_font(
             (self.PAR.ops.table_font[0], self.PAR.ops.table_font[1] - 1, self.PAR.ops.table_font[2]),
+            (self.PAR.ops.index_font[0], self.PAR.ops.index_font[1] - 1, self.PAR.ops.index_font[2]),
             (self.PAR.ops.header_font[0], self.PAR.ops.header_font[1] - 1, self.PAR.ops.header_font[2]),
+            "out",
         )
 
-    def zoom_font(self, table_font: tuple, header_font: tuple):
+    def zoom_font(self, table_font: tuple, index_font: tuple, header_font: tuple, zoom: Literal["in", "out"]) -> None:
         self.saved_column_widths = {}
         self.saved_row_heights = {}
         # should record position prior to change and then see after change
         y = self.canvasy(0)
         x = self.canvasx(0)
         r = self.identify_row(y=0)
         c = self.identify_col(x=0)
@@ -3258,15 +3304,15 @@
             c_pc = 0.0
         old_min_row_height = int(self.min_row_height)
         old_default_row_height = int(self.get_default_row_height())
         self.set_table_font(
             table_font,
             reset_row_positions=False,
         )
-        self.set_index_font(table_font)
+        self.set_index_font(index_font)
         self.set_header_font(header_font)
         if self.PAR.ops.set_cell_sizes_on_zoom:
             self.set_all_cell_sizes_to_text()
             self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
         elif not self.PAR.ops.set_cell_sizes_on_zoom:
             default_row_height = self.get_default_row_height()
             self.row_positions = list(
@@ -3286,26 +3332,26 @@
                             for h in self.gen_row_heights()
                         ),
                     )
                 )
             )
             self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
             self.recreate_all_selection_boxes()
-        self.refresh_open_window_positions()
-        self.RI.refresh_open_window_positions()
-        self.CH.refresh_open_window_positions()
+        self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
+        self.refresh_open_window_positions(zoom=zoom)
+        self.RI.refresh_open_window_positions(zoom=zoom)
+        self.CH.refresh_open_window_positions(zoom=zoom)
         self.see(
             r,
             c,
             check_cell_visibility=False,
-            redraw=False,
+            redraw=True,
             r_pc=r_pc,
             c_pc=c_pc,
         )
-        self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
 
     def get_txt_w(self, txt, font=None):
         self.txt_measure_canvas.itemconfig(
             self.txt_measure_canvas_text,
             text=txt,
             font=self.PAR.ops.table_font if font is None else font,
         )
@@ -4203,20 +4249,20 @@
             self._headers = insert_items(self._headers, header, self.CH.fix_header)
         self.adjust_options_post_add_columns(
             cols=tuple(reversed(columns)),
             create_ops=create_ops,
         )
         if create_selections:
             self.deselect("all")
-            for chunk in consecutive_chunks(tuple(reversed(column_widths))):
+            for boxst, boxend in consecutive_ranges(tuple(reversed(column_widths))):
                 self.create_selection_box(
                     0,
-                    chunk[0],
+                    boxst,
                     len(self.row_positions) - 1,
-                    chunk[-1] + 1,
+                    boxend,
                     "columns",
                     run_binding=True,
                 )
         event_data["added"]["columns"] = {
             "table": columns,
             "header": header,
             "column_widths": column_widths,
@@ -4332,19 +4378,19 @@
             )
         self.adjust_options_post_add_rows(
             rows=tuple(reversed(rows)),
             create_ops=create_ops,
         )
         if create_selections:
             self.deselect("all")
-            for chunk in consecutive_chunks(tuple(reversed(row_heights))):
+            for boxst, boxend in consecutive_ranges(tuple(reversed(row_heights))):
                 self.create_selection_box(
-                    chunk[0],
+                    boxst,
                     0,
-                    chunk[-1] + 1,
+                    boxend,
                     len(self.col_positions) - 1,
                     "rows",
                     run_binding=True,
                 )
         event_data["added"]["rows"] = {
             "table": rows,
             "index": index,
@@ -5616,15 +5662,15 @@
         boxes: dict,
         selected: tuple = tuple(),
     ) -> None:
         for (r1, c1, r2, c2), v in boxes.items():
             if r2 < len(self.row_positions) and c2 < len(self.col_positions):
                 self.create_selection_box(r1, c1, r2, c2, v, run_binding=True)
         if selected:
-            self.set_currently_selected(selected.row, selected.column, box=selected.coords)
+            self.set_currently_selected(selected.row, selected.column, box=selected.box)
 
     def set_currently_selected(
         self,
         r: int | None = None,
         c: int | None = None,
         item: int | None = None,
         box: tuple[int, int, int, int] | None = None,
@@ -5772,25 +5818,26 @@
 
     def hide_box(self, item: int | None) -> None:
         if isinstance(item, int):
             self.disp_boxes.discard(item)
             self.hidd_boxes.add(item)
             self.itemconfig(item, state="hidden")
 
-    def hide_selection_box(self, item: int | None, set_current: bool = True) -> None:
+    def hide_selection_box(self, item: int | None, set_current: bool = True) -> bool:
         if item is None:
             return
         box = self.selection_boxes.pop(item)
         self.hide_box(box.fill_iid)
         self.hide_box(box.bd_iid)
         self.RI.hide_box(box.index)
         self.CH.hide_box(box.header)
         if self.selected.fill_iid == item:
             self.hide_selected()
             self.set_current_to_last()
+        return True
 
     def hide_selected(self) -> None:
         if self.selected:
             self.hide_box(self.selected.iid)
             self.selected = tuple()
 
     def create_selection_box(
@@ -6368,21 +6415,19 @@
         extra_func_key = "??"
         if event is None or self.event_opens_dropdown_or_checkbox(event):
             if event is not None:
                 if hasattr(event, "keysym") and event.keysym == "Return":
                     extra_func_key = "Return"
                 elif hasattr(event, "keysym") and event.keysym == "F2":
                     extra_func_key = "F2"
-            datarn = r if self.all_rows_displayed else self.displayed_rows[r]
-            datacn = c if self.all_columns_displayed else self.displayed_columns[c]
             if event is not None and (hasattr(event, "keysym") and event.keysym == "BackSpace"):
                 extra_func_key = "BackSpace"
                 text = ""
             else:
-                text = f"{self.get_cell_data(datarn, datacn, none_to_empty_str = True)}"
+                text = f"{self.get_cell_data(self.datarn(r), self.datacn(c), none_to_empty_str = True)}"
         elif event is not None and (
             (hasattr(event, "char") and event.char.isalpha())
             or (hasattr(event, "char") and event.char.isdigit())
             or (hasattr(event, "char") and event.char in symbols_set)
         ):
             extra_func_key = event.char
             text = event.char
@@ -6418,17 +6463,15 @@
         if not self.see(r=r, c=c, check_cell_visibility=True):
             self.refresh()
         x = self.col_positions[c]
         y = self.row_positions[r]
         w = self.col_positions[c + 1] - x + 1
         h = self.row_positions[r + 1] - y + 1
         if text is None:
-            text = f"""{self.get_cell_data(r if self.all_rows_displayed else self.displayed_rows[r],
-                                           c if self.all_columns_displayed else self.displayed_columns[c],
-                                           none_to_empty_str = True)}"""
+            text = f"{self.get_cell_data(self.datarn(r), self.datacn(c), none_to_empty_str = True)}"
         bg, fg = self.PAR.ops.table_bg, self.PAR.ops.table_fg
         kwargs = {
             "menu_kwargs": DotDict(
                 {
                     "font": self.PAR.ops.table_font,
                     "foreground": self.PAR.ops.popup_menu_fg,
                     "background": self.PAR.ops.popup_menu_bg,
@@ -6479,15 +6522,22 @@
         c: int = 0,
         event: object = None,
         check_lines: bool = True,
     ) -> None:
         curr_height = self.text_editor.window.winfo_height()
         if curr_height < self.min_row_height:
             return
-        if not check_lines or self.get_lines_cell_height(self.text_editor.window.get_num_lines() + 1) > curr_height:
+        if (
+            not check_lines
+            or self.get_lines_cell_height(
+                self.text_editor.window.get_num_lines() + 1,
+                font=self.text_editor.tktext.cget("font"),
+            )
+            > curr_height
+        ):
             new_height = curr_height + self.table_xtra_lines_increment
             space_bot = self.get_space_bot(r)
             if new_height > space_bot:
                 new_height = space_bot
             if new_height != curr_height:
                 self.text_editor.window.config(height=new_height)
                 if self.dropdown.open and self.dropdown.get_coords() == (r, c):
@@ -6504,32 +6554,38 @@
                         self.coords(
                             self.dropdown.canvas_id,
                             self.col_positions[c],
                             self.row_positions[r],
                         )
                         self.itemconfig(self.dropdown.canvas_id, anchor=anchor, height=win_h)
 
-    def refresh_open_window_positions(self):
+    def refresh_open_window_positions(self, zoom: Literal["in", "out"]):
         if self.text_editor.open:
             r, c = self.text_editor.coords
             self.text_editor.window.config(height=self.row_positions[r + 1] - self.row_positions[r])
+            self.text_editor.tktext.config(font=self.PAR.ops.table_font)
             self.coords(
                 self.text_editor.canvas_id,
                 self.col_positions[c],
                 self.row_positions[r],
             )
         if self.dropdown.open:
+            if zoom == "in":
+                self.dropdown.window.zoom_in()
+            elif zoom == "out":
+                self.dropdown.window.zoom_out()
             r, c = self.dropdown.get_coords()
             if self.text_editor.open:
                 text_editor_h = self.text_editor.window.winfo_height()
                 win_h, anchor = self.get_dropdown_height_anchor(r, c, text_editor_h)
             else:
-                text_editor_h = self.row_positions[r + 1] - self.row_positions[r]
+                text_editor_h = self.row_positions[r + 1] - self.row_positions[r] + 1
                 anchor = self.itemcget(self.dropdown.canvas_id, "anchor")
                 # win_h = 0
+            self.dropdown.window.config(width=self.col_positions[c + 1] - self.col_positions[c] + 1)
             if anchor == "nw":
                 self.coords(
                     self.dropdown.canvas_id,
                     self.col_positions[c],
                     self.row_positions[r] + text_editor_h - 1,
                 )
                 # self.itemconfig(self.dropdown.canvas_id, anchor=anchor, height=win_h)
@@ -6544,15 +6600,14 @@
     def hide_text_editor(self, reason: None | str = None) -> None:
         if self.text_editor.open:
             self.itemconfig(self.text_editor.canvas_id, state="hidden")
             self.text_editor.open = False
         if reason == "Escape":
             self.focus_set()
 
-    # c is displayed col
     def close_text_editor(
         self,
         editor_info: tuple | None = None,
     ) -> str | None:
         # checking if text editor should be closed or not
         focused = self.focus_get()
         try:
@@ -6667,16 +6722,15 @@
         if editor_info[2] != "FocusOut":
             self.focus_set()
         return "break"
 
     def tab_key(self, event: object = None) -> str:
         if not self.selected:
             return
-        r = self.selected.row
-        c = self.selected.column
+        r, c = self.selected.row, self.selected.column
         r1, c1, r2, c2 = self.selection_boxes[self.selected.fill_iid].coords
         numcols = c2 - c1
         numrows = r2 - r1
         if numcols == 1 and numrows == 1:
             new_r = r
             new_c = c + 1 if c < len(self.col_positions) - 2 else c
             self.select_cell(new_r, new_c)
@@ -6799,15 +6853,15 @@
             "ops": self.PAR.ops,
             "outline_color": self.get_selected_box_bg_fg(type_="cells")[1],
             "align": self.get_cell_align(r, c),
             "values": kwargs["values"],
         }
         if self.dropdown.window:
             self.dropdown.window.reset(**reset_kwargs)
-            self.itemconfig(self.dropdown.canvas_id, state="normal")
+            self.itemconfig(self.dropdown.canvas_id, state="normal", anchor=anchor)
             self.coords(self.dropdown.canvas_id, self.col_positions[c], ypos)
         else:
             self.dropdown.window = self.PAR.dropdown_class(
                 self.winfo_toplevel(),
                 **reset_kwargs,
                 close_dropdown_window=self.close_dropdown_window,
                 search_function=kwargs["search_function"],
@@ -7096,44 +7150,49 @@
                 self.set_cell_data(r, c, value=self.data[r][c])
 
     def delete_all_formatting(self, clear_values: bool = False) -> None:
         self.delete_cell_format("all", clear_values=clear_values)
         self.delete_row_format("all", clear_values=clear_values)
         self.delete_column_format("all", clear_values=clear_values)
 
-    def delete_cell_format(self, datarn: str | int = "all", datacn: int = 0, clear_values: bool = False) -> None:
+    def delete_cell_format(
+        self,
+        datarn: Literal["all"] | int = "all",
+        datacn: int = 0,
+        clear_values: bool = False,
+    ) -> None:
         if isinstance(datarn, str) and datarn.lower() == "all":
             itr = gen_formatted(self.cell_options)
         else:
             itr = ((datarn, datacn),)
         get_val = self.get_value_for_empty_cell
         for key in itr:
             try:
                 del self.cell_options[key]["format"]
             except Exception:
                 continue
             if clear_values:
                 self.set_cell_data(*key, get_val(*key), expand_sheet=False)
 
-    def delete_row_format(self, datarn: str | int = "all", clear_values: bool = False) -> None:
+    def delete_row_format(self, datarn: Literal["all"] | int = "all", clear_values: bool = False) -> None:
         if isinstance(datarn, str) and datarn.lower() == "all":
             itr = gen_formatted(self.row_options)
         else:
             itr = (datarn,)
         get_val = self.get_value_for_empty_cell
         for datarn in itr:
             try:
                 del self.row_options[datarn]["format"]
             except Exception:
                 continue
             if clear_values:
                 for datacn in range(len(self.data[datarn])):
                     self.set_cell_data(datarn, datacn, get_val(datarn, datacn), expand_sheet=False)
 
-    def delete_column_format(self, datacn: str | int = "all", clear_values: bool = False) -> None:
+    def delete_column_format(self, datacn: Literal["all"] | int = "all", clear_values: bool = False) -> None:
         if isinstance(datacn, str) and datacn.lower() == "all":
             itr = gen_formatted(self.col_options)
         else:
             itr = (datacn,)
         get_val = self.get_value_for_empty_cell
         for datacn in itr:
             try:
```

### Comparing `tksheet-7.1.5/tksheet/other_classes.py` & `tksheet-7.1.6/tksheet/other_classes.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.5/tksheet/row_index.py` & `tksheet-7.1.6/tksheet/row_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     cycle,
     islice,
 )
 from math import (
     ceil,
     floor,
 )
+from typing import Literal
 
 from .colors import (
     color_map,
 )
 from .formatters import (
     is_bool_like,
     try_to_bool,
@@ -862,14 +863,16 @@
                 datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
                 canvasy = self.canvasy(event.y)
                 if self.event_over_dropdown(r, datarn, event, canvasy) or self.event_over_checkbox(
                     r, datarn, event, canvasy
                 ):
                     self.open_cell(event)
                 elif (iid := self.event_over_tree_arrow(r, canvasy, event.x)) is not None:
+                    if self.MT.selection_boxes:
+                        self.select_row(r, redraw=False)
                     self.PAR.item(iid, open_=iid not in self.tree_open_ids)
             else:
                 self.mouseclick_outside_editor_or_dropdown_all_canvases(inside=True)
             self.b1_pressed_loc = None
             self.closed_dropdown = None
         self.dragged_row = None
         self.currently_resizing_width = False
@@ -1010,19 +1013,18 @@
         datarn = row if self.MT.all_rows_displayed else self.MT.displayed_rows[row]
         if height is None:
             if self.MT.all_columns_displayed:
                 if displayed_only:
                     x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
                     start_col, end_col = self.MT.get_visible_columns(x1, x2)
                 else:
-                    start_col, end_col = (
-                        0,
-                        len(self.MT.data[row]) if self.MT.data else 0,
-                    )
-                iterable = range(start_col, end_col)
+                    if not self.MT.data or datarn >= len(self.MT.data):
+                        iterable = range(0, 0)
+                    else:
+                        iterable = range(0, len(self.MT.data[datarn]))
             else:
                 if displayed_only:
                     x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
                     start_col, end_col = self.MT.get_visible_columns(x1, x2)
                 else:
                     start_col, end_col = 0, len(self.MT.displayed_columns)
                 iterable = self.MT.displayed_columns[start_col:end_col]
@@ -1708,16 +1710,15 @@
         extra_func_key = "??"
         if event is None or self.MT.event_opens_dropdown_or_checkbox(event):
             if event is not None:
                 if hasattr(event, "keysym") and event.keysym == "Return":
                     extra_func_key = "Return"
                 elif hasattr(event, "keysym") and event.keysym == "F2":
                     extra_func_key = "F2"
-            datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-            text = self.get_cell_data(datarn, none_to_empty_str=True, redirect_int=True)
+            text = self.get_cell_data(self.MT.datarn(r), none_to_empty_str=True, redirect_int=True)
         elif event is not None and (
             (hasattr(event, "keysym") and event.keysym == "BackSpace") or event.keycode in (8, 855638143)
         ):
             extra_func_key = "BackSpace"
             text = ""
         elif event is not None and (
             (hasattr(event, "char") and event.char.isalpha())
@@ -1757,17 +1758,16 @@
             self.hide_text_editor()
         if not self.MT.see(r=r, c=0, keep_yscroll=True, check_cell_visibility=True):
             self.MT.refresh()
         x = 0
         y = self.MT.row_positions[r]
         w = self.current_width + 1
         h = self.MT.row_positions[r + 1] - y + 1
-        datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
         if text is None:
-            text = self.get_cell_data(datarn, none_to_empty_str=True, redirect_int=True)
+            text = self.get_cell_data(self.MT.datarn(r), none_to_empty_str=True, redirect_int=True)
         bg, fg = self.PAR.ops.index_bg, self.PAR.ops.index_fg
         kwargs = {
             "menu_kwargs": DotDict(
                 {
                     "font": self.PAR.ops.table_font,
                     "foreground": self.PAR.ops.popup_menu_fg,
                     "background": self.PAR.ops.popup_menu_bg,
@@ -1816,15 +1816,15 @@
         curr_height = self.text_editor.window.winfo_height()
         if curr_height < self.MT.min_row_height:
             return
         if (
             not check_lines
             or self.MT.get_lines_cell_height(
                 self.text_editor.window.get_num_lines() + 1,
-                font=self.PAR.ops.index_font,
+                font=self.text_editor.tktext.cget("font"),
             )
             > curr_height
         ):
             new_height = curr_height + self.MT.index_xtra_lines_increment
             space_bot = self.MT.get_space_bot(r)
             if new_height > space_bot:
                 new_height = space_bot
@@ -1847,32 +1847,38 @@
                         self.coords(
                             self.dropdown.canvas_id,
                             self.MT.col_positions[c],
                             self.MT.row_positions[r],
                         )
                         self.itemconfig(self.dropdown.canvas_id, anchor=anchor, height=win_h)
 
-    def refresh_open_window_positions(self):
+    def refresh_open_window_positions(self, zoom: Literal["in", "out"]):
         if self.text_editor.open:
             r = self.text_editor.row
             self.text_editor.window.config(height=self.MT.row_positions[r + 1] - self.MT.row_positions[r])
+            self.text_editor.tktext.config(font=self.PAR.ops.index_font)
             self.coords(
                 self.text_editor.canvas_id,
                 0,
                 self.MT.row_positions[r],
             )
         if self.dropdown.open:
+            if zoom == "in":
+                self.dropdown.window.zoom_in()
+            elif zoom == "out":
+                self.dropdown.window.zoom_out()
             r = self.dropdown.get_coords()
             if self.text_editor.open:
                 text_editor_h = self.text_editor.window.winfo_height()
                 win_h, anchor = self.get_dropdown_height_anchor(r, text_editor_h)
             else:
-                text_editor_h = self.MT.row_positions[r + 1] - self.MT.row_positions[r]
+                text_editor_h = self.MT.row_positions[r + 1] - self.MT.row_positions[r] + 1
                 anchor = self.itemcget(self.dropdown.canvas_id, "anchor")
                 # win_h = 0
+            self.dropdown.window.config(width=self.current_width + 1)
             if anchor == "nw":
                 self.coords(
                     self.dropdown.canvas_id,
                     0,
                     self.MT.row_positions[r] + text_editor_h - 1,
                 )
                 # self.itemconfig(self.dropdown.canvas_id, anchor=anchor, height=win_h)
@@ -1952,60 +1958,71 @@
                 )  # end of cell
             else:
                 win_h += self.MT.min_row_height
             if i == 5:
                 break
         if win_h > 500:
             win_h = 500
-        space_bot = self.MT.get_space_bot(0, text_editor_h)
+        space_bot = self.MT.get_space_bot(r, text_editor_h)
+        space_top = int(self.MT.row_positions[r])
+        anchor = "nw"
         win_h2 = int(win_h)
         if win_h > space_bot:
-            win_h = space_bot - 1
+            if space_bot >= space_top:
+                anchor = "nw"
+                win_h = space_bot - 1
+            elif space_top > space_bot:
+                anchor = "sw"
+                win_h = space_top - 1
         if win_h < self.MT.index_txt_height + 5:
             win_h = self.MT.index_txt_height + 5
         elif win_h > win_h2:
             win_h = win_h2
-        return win_h, "nw"
+        return win_h, anchor
 
     def dropdown_text_editor_modified(
         self,
         dd_window: object,
         event: dict,
         modified_func: Callable | None,
     ) -> None:
         if modified_func:
             modified_func(event)
         dd_window.search_and_see(event)
 
     # r is displayed row
-    def open_dropdown_window(self, r, datarn=None, event: object = None):
+    def open_dropdown_window(self, r, event: object = None):
         self.hide_text_editor("Escape")
-        if datarn is None:
-            datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-        kwargs = self.get_cell_kwargs(datarn, key="dropdown")
+        kwargs = self.get_cell_kwargs(self.MT.datarn(r), key="dropdown")
         if kwargs["state"] == "normal":
             if not self.open_text_editor(event=event, r=r, dropdown=True):
                 return
         win_h, anchor = self.get_dropdown_height_anchor(r)
-        win_w = self.current_width
-        ypos = self.MT.row_positions[r + 1]
+        win_w = self.current_width + 1
+        if anchor == "nw":
+            if kwargs["state"] == "normal":
+                ypos = self.MT.row_positions[r] + self.text_editor.window.winfo_height() - 1
+            else:
+                ypos = self.MT.row_positions[r + 1]
+        else:
+            ypos = self.MT.row_positions[r]
         reset_kwargs = {
             "r": r,
             "c": 0,
             "width": win_w,
             "height": win_h,
             "font": self.PAR.ops.index_font,
             "ops": self.PAR.ops,
             "outline_color": self.PAR.ops.popup_menu_fg,
             "align": self.get_cell_align(r),
             "values": kwargs["values"],
         }
         if self.dropdown.window:
             self.dropdown.window.reset(**reset_kwargs)
-            self.itemconfig(self.dropdown.canvas_id, state="normal")
+            self.itemconfig(self.dropdown.canvas_id, state="normal", anchor=anchor)
             self.coords(self.dropdown.canvas_id, 0, ypos)
         else:
             self.dropdown.window = self.PAR.dropdown_class(
                 self.winfo_toplevel(),
                 **reset_kwargs,
                 single_index="r",
                 close_dropdown_window=self.close_dropdown_window,
```

### Comparing `tksheet-7.1.5/tksheet/sheet.py` & `tksheet-7.1.6/tksheet/sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1088,14 +1088,22 @@
             self.CH.focus_set()
         elif canvas in ("row_index", "index"):
             self.RI.focus_set()
         elif canvas in ("topleft", "top_left"):
             self.TL.focus_set()
         return self
 
+    def zoom_in(self) -> Sheet:
+        self.MT.zoom_in()
+        return self
+
+    def zoom_out(self) -> Sheet:
+        self.MT.zoom_out()
+        return self
+
     @property
     def event(self) -> EventDataDict:
         return self.last_event_data
 
     # Span objects
 
     def span(
@@ -3170,14 +3178,24 @@
         cell: tuple[int, int] | None = None,
         redraw: bool = True,
     ) -> Sheet:
         self.MT.deselect(r=row, c=column, cell=cell, redraw=False)
         self.set_refresh_timer(redraw)
         return self
 
+    def deselect_any(
+        self,
+        rows: Iterator[int] | int | None,
+        columns: Iterator[int] | int | None,
+        redraw: bool = True,
+    ) -> Sheet:
+        self.MT.deselect_any(rows=rows, columns=columns, redraw=False)
+        self.set_refresh_timer(redraw)
+        return self
+
     # Row Heights and Column Widths
 
     def default_column_width(self, width: int | None = None) -> int:
         if isinstance(width, int):
             self.ops.default_column_width = width
         return self.ops.default_column_width
 
@@ -3773,14 +3791,16 @@
                 itr=self.MT.gen_row_heights,
                 to_pop=to_pop,
                 save_to=self.MT.saved_row_heights,
             ),
         )
         if deselect_all:
             self.MT.deselect(redraw=False)
+        else:
+            self.MT.deselect_any(rows=rows, redraw=False)
         self.set_refresh_timer(redraw)
         return self
 
     # uses data indexes
     def show_rows(
         self,
         rows: int | Iterator[int],
```

### Comparing `tksheet-7.1.5/tksheet/sheet_options.py` & `tksheet-7.1.6/tksheet/sheet_options.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.5/tksheet/text_editor.py` & `tksheet-7.1.6/tksheet/text_editor.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.5/tksheet/themes.py` & `tksheet-7.1.6/tksheet/themes.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.5/tksheet/top_left_rectangle.py` & `tksheet-7.1.6/tksheet/top_left_rectangle.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.5/tksheet/vars.py` & `tksheet-7.1.6/tksheet/vars.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.5/tksheet.egg-info/PKG-INFO` & `tksheet-7.1.6/tksheet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 7.1.5
+Version: 7.1.6
 Summary: Tkinter table / sheet widget
 Author-email: ragardner <github@ragardner.simplelogin.com>
 License: Copyright (c) 2019 ragardner and open source contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

