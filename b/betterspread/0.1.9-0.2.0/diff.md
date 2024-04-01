# Comparing `tmp/betterspread-0.1.9.tar.gz` & `tmp/betterspread-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterspread-0.1.9.tar", max compression
+gzip compressed data, was "betterspread-0.2.0.tar", max compression
```

## Comparing `betterspread-0.1.9.tar` & `betterspread-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      990 2024-03-06 13:50:58.175957 betterspread-0.1.9/README.md
--rw-r--r--   0        0        0      216 2024-03-06 23:15:52.699049 betterspread-0.1.9/betterspread/__init__.py
--rw-r--r--   0        0        0     2408 2024-03-06 23:15:45.465755 betterspread-0.1.9/betterspread/cell.py
--rw-r--r--   0        0        0      419 2024-03-06 13:50:58.176278 betterspread-0.1.9/betterspread/connection.py
--rw-r--r--   0        0        0     2085 2024-03-06 23:15:45.464721 betterspread-0.1.9/betterspread/row.py
--rw-r--r--   0        0        0     1552 2024-03-06 17:46:16.681869 betterspread-0.1.9/betterspread/sheet.py
--rw-r--r--   0        0        0     1114 2024-03-06 13:50:58.176550 betterspread-0.1.9/betterspread/style.py
--rw-r--r--   0        0        0     3009 2024-03-06 17:45:01.276798 betterspread-0.1.9/betterspread/tab.py
--rw-r--r--   0        0        0      581 2024-03-06 23:15:52.702121 betterspread-0.1.9/betterspread/utils.py
--rw-r--r--   0        0        0      661 2024-03-06 23:16:29.271997 betterspread-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 betterspread-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      990 2024-03-06 13:50:58.175957 betterspread-0.2.0/README.md
+-rw-r--r--   0        0        0      216 2024-03-06 23:15:52.699049 betterspread-0.2.0/betterspread/__init__.py
+-rw-r--r--   0        0        0     2412 2024-04-01 21:56:52.317830 betterspread-0.2.0/betterspread/cell.py
+-rw-r--r--   0        0        0      419 2024-03-06 13:50:58.176278 betterspread-0.2.0/betterspread/connection.py
+-rw-r--r--   0        0        0     2085 2024-04-01 21:58:03.606643 betterspread-0.2.0/betterspread/row.py
+-rw-r--r--   0        0        0     1552 2024-03-06 17:46:16.681869 betterspread-0.2.0/betterspread/sheet.py
+-rw-r--r--   0        0        0     1114 2024-03-06 13:50:58.176550 betterspread-0.2.0/betterspread/style.py
+-rw-r--r--   0        0        0     3009 2024-03-06 17:45:01.276798 betterspread-0.2.0/betterspread/tab.py
+-rw-r--r--   0        0        0      581 2024-03-06 23:15:52.702121 betterspread-0.2.0/betterspread/utils.py
+-rw-r--r--   0        0        0      661 2024-04-01 21:58:35.837167 betterspread-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 betterspread-0.2.0/PKG-INFO
```

### Comparing `betterspread-0.1.9/README.md` & `betterspread-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `betterspread-0.1.9/betterspread/cell.py` & `betterspread-0.2.0/betterspread/cell.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,16 +60,16 @@
                 label=self.label,
                 row_index=self.row_index,
                 row=self.row,
             )
 
         await run_in_executor(
             self.tab.update,
+            [[value]],
             f"{self.label}{self.row_index}",
-            value,
             value_input_option=input_formats.get(input_format, "raw"),
             response_value_render_option=render_formats.get(render_format, "formatted"),
         )
         return Cell(
             value, self.tab, self.label, self.row_index, self.cell_index, self.row
         )
```

### Comparing `betterspread-0.1.9/betterspread/row.py` & `betterspread-0.2.0/betterspread/row.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         )
         empty_items = self.convert_to_cell(list(map(lambda _: "", self.items)))
         self.items = empty_items
         super().__init__(empty_items)
 
     async def update(self, values: list, start: str = "A", *args, **kwargs):
         await run_in_executor(
-            self.tab.update, f"{start}{self.row_index}", [values], *args, **kwargs
+            self.tab.update, [values], f"{start}{self.row_index}", *args, **kwargs
         )
         self.items = self.convert_to_cell(values)
         super().__init__(self.items)
 
     async def style(self, obj: Union[Style, CellFormat]):
         style = obj.raw if isinstance(obj, Style) else obj
         await run_in_executor(
```

### Comparing `betterspread-0.1.9/betterspread/sheet.py` & `betterspread-0.2.0/betterspread/sheet.py`

 * *Files identical despite different names*

### Comparing `betterspread-0.1.9/betterspread/style.py` & `betterspread-0.2.0/betterspread/style.py`

 * *Files identical despite different names*

### Comparing `betterspread-0.1.9/betterspread/tab.py` & `betterspread-0.2.0/betterspread/tab.py`

 * *Files identical despite different names*

### Comparing `betterspread-0.1.9/betterspread/utils.py` & `betterspread-0.2.0/betterspread/utils.py`

 * *Files identical despite different names*

### Comparing `betterspread-0.1.9/pyproject.toml` & `betterspread-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "betterspread"
-version = "0.1.9"
+version = "0.2.0"
 description = ""
 authors = ["Md Shahriyar Alam <contact@shahriyar.dev>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.urls]
 homepage = "https://github.com/shahriyardx/betterspread"
```

### Comparing `betterspread-0.1.9/PKG-INFO` & `betterspread-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterspread
-Version: 0.1.9
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Md Shahriyar Alam
 Author-email: contact@shahriyar.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

