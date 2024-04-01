# Comparing `tmp/speedtab-0.2.1.1.tar.gz` & `tmp/speedtab-0.2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.2.1.1.tar", max compression
+gzip compressed data, was "speedtab-0.2.1.2.tar", max compression
```

## Comparing `speedtab-0.2.1.1.tar` & `speedtab-0.2.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2024-03-22 18:01:47.096789 speedtab-0.2.1.1/pyproject.toml
--rw-r--r--   0        0        0      382 2023-12-14 09:13:27.273500 speedtab-0.2.1.1/speedtab/__init__.py
--rw-r--r--   0        0        0    87055 2024-03-22 18:01:12.044690 speedtab-0.2.1.1/speedtab/client.py
--rw-r--r--   0        0        0     7739 2023-12-14 09:47:11.439768 speedtab-0.2.1.1/speedtab/enums.py
--rw-r--r--   0        0        0     1824 2023-12-14 09:47:11.343768 speedtab-0.2.1.1/speedtab/formats.py
--rw-r--r--   0        0        0      783 2024-03-22 18:02:05.162852 speedtab-0.2.1.1/setup.py
--rw-r--r--   0        0        0      808 2024-03-22 18:02:05.162852 speedtab-0.2.1.1/PKG-INFO
+-rw-r--r--   0        0        0      567 2024-04-01 10:37:15.231563 speedtab-0.2.1.2/pyproject.toml
+-rw-r--r--   0        0        0      382 2023-12-14 09:13:27.273500 speedtab-0.2.1.2/speedtab/__init__.py
+-rw-r--r--   0        0        0    87045 2024-04-01 10:37:08.371206 speedtab-0.2.1.2/speedtab/client.py
+-rw-r--r--   0        0        0     7739 2023-12-14 09:47:11.439768 speedtab-0.2.1.2/speedtab/enums.py
+-rw-r--r--   0        0        0     1824 2023-12-14 09:47:11.343768 speedtab-0.2.1.2/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2024-04-01 10:37:57.023689 speedtab-0.2.1.2/setup.py
+-rw-r--r--   0        0        0      808 2024-04-01 10:37:57.024690 speedtab-0.2.1.2/PKG-INFO
```

### Comparing `speedtab-0.2.1.1/pyproject.toml` & `speedtab-0.2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.2.1.1"
+version = "0.2.1.2"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.2.1.1/speedtab/client.py` & `speedtab-0.2.1.2/speedtab/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1388,15 +1388,15 @@
         self.sheet_name = sheet_name
         self.sheet_id = sheet_id
         self._task_queue = task_query
         self.sheets = sheets
         cells = parse_range(cells)
 
         self.start_data_cell = f'{sheet_name}!{col_num_to_string(cells[1])}{num_to_string(cells[0])}'
-        self.data_cell = self.start_data_cell + f':{col_num_to_string(cells[3])}{num_to_string(cells[2] if cells[2] is not None else self.sheets.get(self.sheet_name).get("max_row"))}'
+        self.data_cell = self.start_data_cell + f':{col_num_to_string(cells[3])}{str(cells[2] if cells[2] is not None else self.sheets.get(self.sheet_name).get("max_row"))}'
         self.work_zone = dict([(key, val + SHIFT_DIM.get(key) if val is not None else val)
                                for key, val in zip(SHIFT_DIM.keys(), cells)]
                               + [('sheetId', self.sheet_id)])
 
         super().__init__(self.sheet_id, self._task_queue, self.work_zone, self.start_data_cell, self.base,
                          self.data_cell)
```

### Comparing `speedtab-0.2.1.1/speedtab/enums.py` & `speedtab-0.2.1.2/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.2.1.1/speedtab/formats.py` & `speedtab-0.2.1.2/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.2.1.1/setup.py` & `speedtab-0.2.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.2.1.1',
+    'version': '0.2.1.2',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.2.1.1/PKG-INFO` & `speedtab-0.2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.2.1.1
+Version: 0.2.1.2
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

