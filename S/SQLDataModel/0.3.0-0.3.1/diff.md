# Comparing `tmp/SQLDataModel-0.3.0.tar.gz` & `tmp/SQLDataModel-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLDataModel-0.3.0.tar", last modified: Sun Mar 31 21:23:43 2024, max compression
+gzip compressed data, was "SQLDataModel-0.3.1.tar", last modified: Mon Apr  1 18:24:10 2024, max compression
```

## Comparing `SQLDataModel-0.3.0.tar` & `SQLDataModel-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 21:23:43.368372 SQLDataModel-0.3.0/
--rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 SQLDataModel-0.3.0/LICENSE
--rw-rw-rw-   0        0        0    27189 2024-03-31 21:23:43.352372 SQLDataModel-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    25317 2024-03-28 21:22:17.000000 SQLDataModel-0.3.0/README.md
--rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 SQLDataModel-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-31 21:23:43.369374 SQLDataModel-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2312 2024-03-31 21:21:43.000000 SQLDataModel-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 21:23:41.677289 SQLDataModel-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-31 21:23:42.917947 SQLDataModel-0.3.0/src/SQLDataModel/
--rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 SQLDataModel-0.3.0/src/SQLDataModel/ANSIColor.py
--rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 SQLDataModel-0.3.0/src/SQLDataModel/HTMLParser.py
--rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 SQLDataModel-0.3.0/src/SQLDataModel/JSONEncoder.py
--rw-rw-rw-   0        0        0   535691 2024-03-31 21:20:22.000000 SQLDataModel-0.3.0/src/SQLDataModel/SQLDataModel.py
--rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 SQLDataModel-0.3.0/src/SQLDataModel/StandardDeviation.py
--rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 SQLDataModel-0.3.0/src/SQLDataModel/__init__.py
--rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 SQLDataModel-0.3.0/src/SQLDataModel/converters.py
--rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 SQLDataModel-0.3.0/src/SQLDataModel/demo.py
--rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 SQLDataModel-0.3.0/src/SQLDataModel/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-31 21:23:43.211400 SQLDataModel-0.3.0/src/SQLDataModel/extensions/
--rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 SQLDataModel-0.3.0/src/SQLDataModel/extensions/__init__.py
--rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 SQLDataModel-0.3.0/src/SQLDataModel/extensions/str_utils.c
-drwxrwxrwx   0        0        0        0 2024-03-31 21:23:43.336546 SQLDataModel-0.3.0/src/SQLDataModel.egg-info/
--rw-rw-rw-   0        0        0    27189 2024-03-31 21:23:41.000000 SQLDataModel-0.3.0/src/SQLDataModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-03-31 21:23:41.000000 SQLDataModel-0.3.0/src/SQLDataModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 21:23:41.000000 SQLDataModel-0.3.0/src/SQLDataModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-03-31 21:23:41.000000 SQLDataModel-0.3.0/src/SQLDataModel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-31 21:23:43.243553 SQLDataModel-0.3.0/tests/
--rw-rw-rw-   0        0        0    39789 2024-03-31 20:56:05.000000 SQLDataModel-0.3.0/tests/test_Future.py
--rw-rw-rw-   0        0        0    39792 2024-03-31 20:56:14.000000 SQLDataModel-0.3.0/tests/test_SQLDataModel.py
+drwxrwxrwx   0        0        0        0 2024-04-01 18:24:10.122908 SQLDataModel-0.3.1/
+-rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 SQLDataModel-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0    27189 2024-04-01 18:24:10.113045 SQLDataModel-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    25317 2024-03-28 21:22:17.000000 SQLDataModel-0.3.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 SQLDataModel-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 18:24:10.124608 SQLDataModel-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2312 2024-04-01 18:23:39.000000 SQLDataModel-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 18:24:08.607600 SQLDataModel-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 18:24:09.793080 SQLDataModel-0.3.1/src/SQLDataModel/
+-rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 SQLDataModel-0.3.1/src/SQLDataModel/ANSIColor.py
+-rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 SQLDataModel-0.3.1/src/SQLDataModel/HTMLParser.py
+-rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 SQLDataModel-0.3.1/src/SQLDataModel/JSONEncoder.py
+-rw-rw-rw-   0        0        0   542058 2024-04-01 18:10:49.000000 SQLDataModel-0.3.1/src/SQLDataModel/SQLDataModel.py
+-rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 SQLDataModel-0.3.1/src/SQLDataModel/StandardDeviation.py
+-rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 SQLDataModel-0.3.1/src/SQLDataModel/__init__.py
+-rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 SQLDataModel-0.3.1/src/SQLDataModel/converters.py
+-rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 SQLDataModel-0.3.1/src/SQLDataModel/demo.py
+-rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 SQLDataModel-0.3.1/src/SQLDataModel/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-01 18:24:10.017827 SQLDataModel-0.3.1/src/SQLDataModel/extensions/
+-rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 SQLDataModel-0.3.1/src/SQLDataModel/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 SQLDataModel-0.3.1/src/SQLDataModel/extensions/str_utils.c
+drwxrwxrwx   0        0        0        0 2024-04-01 18:24:10.104983 SQLDataModel-0.3.1/src/SQLDataModel.egg-info/
+-rw-rw-rw-   0        0        0    27189 2024-04-01 18:24:08.000000 SQLDataModel-0.3.1/src/SQLDataModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-04-01 18:24:08.000000 SQLDataModel-0.3.1/src/SQLDataModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 18:24:08.000000 SQLDataModel-0.3.1/src/SQLDataModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-01 18:24:08.000000 SQLDataModel-0.3.1/src/SQLDataModel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 18:24:10.035830 SQLDataModel-0.3.1/tests/
+-rw-rw-rw-   0        0        0    41796 2024-04-01 18:10:53.000000 SQLDataModel-0.3.1/tests/test_Future.py
+-rw-rw-rw-   0        0        0    41799 2024-04-01 18:10:54.000000 SQLDataModel-0.3.1/tests/test_SQLDataModel.py
```

### Comparing `SQLDataModel-0.3.0/LICENSE` & `SQLDataModel-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.0/PKG-INFO` & `SQLDataModel-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.0
+Version: 0.3.1
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
```

### Comparing `SQLDataModel-0.3.0/README.md` & `SQLDataModel-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.0/setup.py` & `SQLDataModel-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='SQLDataModel',  
-     version='0.3.0',
+     version='0.3.1',
      scripts=['src/SQLDataModel/SQLDataModel.py'] ,
      author='Ante Tonkovic-Capin',
      author_email='antetc@icloud.com',
      description='SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.',
      keywords='SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package',
      license_file='LICENSE',
      long_description=long_description,
```

### Comparing `SQLDataModel-0.3.0/src/SQLDataModel/ANSIColor.py` & `SQLDataModel-0.3.1/src/SQLDataModel/ANSIColor.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.0/src/SQLDataModel/HTMLParser.py` & `SQLDataModel-0.3.1/src/SQLDataModel/HTMLParser.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.0/src/SQLDataModel/JSONEncoder.py` & `SQLDataModel-0.3.1/src/SQLDataModel/JSONEncoder.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.0/src/SQLDataModel/SQLDataModel.py` & `SQLDataModel-0.3.1/src/SQLDataModel/SQLDataModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,23 +385,23 @@
         self.sql_idx = "idx"
         """``str``: The index column name applied to the sqlite3 in-memory representation of the model. Default is ``'idx'``"""
         self.sql_model = "sdm"
         """``str``: The table name applied to the sqlite3 in-memory representation of the model. Default is ``'sdm'``"""
         self.display_max_rows = display_max_rows
         """``int``: The maximum number of rows to display. Default is 1,000 rows."""
         self.min_column_width = min_column_width
-        """``int``: The minimum column width in characters to use for string representations of the data. Default is 4."""
+        """``int``: The minimum column width in characters to use for string representations of the data. Default is 3."""
         self.max_column_width = max_column_width
-        """``int``: The maximum column width in characters to use for string representations of the data. Default is 32."""
+        """``int``: The maximum column width in characters to use for string representations of the data. Default is 38."""
         self.column_alignment = column_alignment # 'dynamic','left','center','right'
         """``str``: The column alignment to use for string representations of the data, value must be one of ``['dynamic','left','center','right']`` Default is ``'dynamic'``, using right-alignment for numeric columns and left-aligned for all others."""
         self.display_index = display_index
         """``bool``: Determines whether the index column is displayed when string representations of the table are generated. Default is True."""
         self.display_float_precision = display_float_precision
-        """``int``: The floating point precision to use for string representations of the table, does not affect the actual floating point values stored in the model. Default is 4."""
+        """``int``: The floating point precision to use for string representations of the table, does not affect the actual floating point values stored in the model. Default is 2."""
         self.row_count = len(data) if had_data else 0
         """``int``: The current row count of the model."""
         had_idx = True if headers[0] == self.sql_idx else False
         dyn_idx_offset,dyn_idx_bind,dyn_add_idx_insert = (1, "?,", f'"{self.sql_idx}",') if had_idx else (0, "", "")
         headers = headers[dyn_idx_offset:]
         self.headers = headers
         """``list[str]``: The current column names of the model. If not provided, default column names will be used."""
@@ -2369,14 +2369,15 @@
               - ``'.md'``: passed to :meth:`SQLDataModel.from_markdown()` as markdown source data.
               - ``'.parquet'``: passed to :meth:`SQLDataModel.from_parquet()` as parquet source data.
               - ``'.pkl'``: passed to :meth:`SQLDataModel.from_pickle()` as pickle source data.
               - ``'.sdm'``: passed to :meth:`SQLDataModel.from_pickle()` as pickle source data.
               - ``'.tex'``: passed to :meth:`SQLDataModel.from_latex()` as latex source data.
               - ``'.tsv'``: passed to :meth:`SQLDataModel.from_csv()` as csv source data.
               - ``'.txt'``: passed to :meth:`SQLDataModel.from_text()` as text source data.
+              - ``'.xlsx'``: passed to :meth:`SQLDataModel.from_excel()` as excel source data.
 
         Returns:
             ``SQLDataModel``: The SQLDataModel object created from the provided data.
 
         Raises:
             ``TypeError``: If the type of ``data`` is not supported.
             ``ValueError``: If the file extension is not found, unsupported, or if the SQL extension is not supported.
@@ -2429,36 +2430,38 @@
         """
         if not isinstance(data, (list, tuple, str, dict)) and (type(data).__name__ not in ('ndarray','DataFrame')):
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(data).__name__}', argument for ``data`` must be one of 'list', 'tuple', 'str', 'dict' or a supported external object type")
             )
         supported_ext = ('.csv','.html','.json','.md','.parquet','.pkl','.sdm','.tex','.tsv','.txt','.xlsx')
         ext_operation = {
-             '.csv': SQLDataModel.from_csv
-            ,'.html': SQLDataModel.from_html
-            ,'.json': SQLDataModel.from_json
-            ,'.md': SQLDataModel.from_markdown
-            ,'.parquet': SQLDataModel.from_parquet
-            ,'.pkl': SQLDataModel.from_pickle
-            ,'.sdm': SQLDataModel.from_pickle
-            ,'.tex': SQLDataModel.from_latex
-            ,'.tsv': SQLDataModel.from_csv
-            ,'.txt': SQLDataModel.from_text
-            ,'.xlsx': SQLDataModel.from_excel
+             '.csv': cls.from_csv
+            ,'.html': cls.from_html
+            ,'.json': cls.from_json
+            ,'.md': cls.from_markdown
+            ,'.parquet': cls.from_parquet
+            ,'.pkl': cls.from_pickle
+            ,'.sdm': cls.from_pickle
+            ,'.tex': cls.from_latex
+            ,'.tsv': cls.from_csv
+            ,'.txt': cls.from_text
+            ,'.xlsx': cls.from_excel
         }
         if isinstance(data, dict):
             if all(value in ('None','int','float','str','bytes','date','datetime','NoneType','bool') for value in data.values()):
-                return SQLDataModel(dtypes=data, **kwargs)
+                return cls(dtypes=data, **kwargs)
             else:
-                return SQLDataModel.from_dict(data, **kwargs)            
+                return cls.from_dict(data, **kwargs)            
         elif isinstance(data, (list,tuple)):
-            if len(data) == 1:
-                return SQLDataModel(headers=data, **kwargs)
+            if len(data) == 1 and not isinstance(data[0], dict):
+                return cls(headers=data, **kwargs)
+            elif len(data) >= 1 and isinstance(data[0], dict):
+                return cls.from_json(json_source=data, **kwargs)
             else:
-                return SQLDataModel(data=data, **kwargs)
+                return cls(data=data, **kwargs)
         elif isinstance(data, str):
             if data.startswith('http'):
                 return ext_operation['.html'](data, **kwargs)
             if os.path.exists(data):
                 ext = os.path.splitext(data)[-1]
                 if not ext:
                     raise ValueError(
@@ -2472,15 +2475,15 @@
                     else:
                         raise ValueError(
                             SQLDataModel.ErrorFormat(f"ValueError: unsupported file extension '{ext}', see documentation for a list of supported file types")
                         )
                 return ext_operation[ext.lower()](data, **kwargs)
             html_pattern = r'</table>'
             latex_pattern = r'\\begin\{tabular\}'
-            markdown_pattern = r'\| *(:?-{3,}:? *\|)+'
+            markdown_pattern = r'\|?:?-+:?\|:?-+:?\|?' # changed from: r'\| *(:?-{3,}:? *\|)+'
             json_pattern = r'\{.*\}'
             if bool(re.search(html_pattern, data)):
                 return ext_operation['.html'](data, **kwargs)
             elif bool(re.search(latex_pattern, data)):
                 return ext_operation['.tex'](data, **kwargs)
             elif bool(re.search(markdown_pattern, data)):
                 return ext_operation['.md'](data, **kwargs)
@@ -2488,23 +2491,23 @@
                 try:
                     json.loads(data)
                     is_json = True
                 except Exception:
                     is_json = False
                 if is_json:
                     return ext_operation['.json'](data, **kwargs)
-            return SQLDataModel.from_text(data, **kwargs)
+            return cls.from_text(data, **kwargs)
         else:
             arg_type = type(data).__name__
             if arg_type == 'ndarray':
-                return SQLDataModel.from_numpy(data, **kwargs)
+                return cls.from_numpy(data, **kwargs)
             elif arg_type == 'DataFrame':
-                return SQLDataModel.from_pandas(data, **kwargs)
+                return cls.from_pandas(data, **kwargs)
             elif arg_type == 'Table':
-                return SQLDataModel.from_pyarrow(data, **kwargs)
+                return cls.from_pyarrow(data, **kwargs)
             else:
                 raise TypeError(
                     SQLDataModel.ErrorFormat(f"TypeError: unsupported type '{arg_type}', current supported external types are 'numpy.ndarray' or 'pandas.DataFrame' objects")
                 )
     
     @classmethod
     def from_dict(cls, data:dict|list, **kwargs) -> SQLDataModel:
@@ -7534,14 +7537,60 @@
             self._update_model_metadata(update_row_meta=True)
             return
         else:
             return type(self)((*self.data(),*other), self.headers, display_max_rows=self.display_max_rows, min_column_width=self.min_column_width, max_column_width=self.max_column_width, column_alignment=self.column_alignment, display_color=self.display_color, display_index=self.display_index, display_float_precision=self.display_float_precision)
 
     def count(self) -> SQLDataModel:
         """
+        Returns a new ``SQLDataModel`` containing the counts of non-null values for each column in a row-wise orientation.
+
+        Returns:
+            ``SQLDataModel``: A new SQLDataModel containing the counts of non-null values in each column.
+
+        Example::
+            
+            from SQLDataModel import SQLDataModel
+
+            # Sample data with missing values
+            headers = ['Name', 'Age', 'Gender', 'Tenure']
+            data = [
+                ('Alice', 25, 'Female', 1.0),
+                ('Bob', None, 'Male', 2.7),
+                ('Charlie', 30, 'Male', None),
+                ('David', None, 'Male', 3.8)
+            ]   
+
+            # Create the model
+            sdm = SQLDataModel(data, headers)
+
+            # Get counts
+            counts = sdm.count()
+
+            # View result
+            print(counts)
+
+        This will output the count of all non-null values for each column:
+
+        ```shell
+            ┌──────┬─────┬────────┬────────┐
+            │ Name │ Age │ Gender │ Tenure │
+            ├──────┼─────┼────────┼────────┤
+            │    4 │   2 │      4 │      3 │
+            └──────┴─────┴────────┴────────┘
+            [1 rows x 4 columns]
+        ```
+
+        Note:
+            - See :meth:`SQLDataModel.column_counts()` for column-wise count of unique, null and total values for each column.
+        """
+        fetch_stmt = " ".join(("select",",".join([f"""sum(case when "{col}" is null then 0 else 1 end) as "{col}" """ for col in self.headers]),f'from "{self.sql_model}"'))
+        return self.execute_fetch(fetch_stmt, dtypes={col:'int' for col in self.headers})
+
+    def column_counts(self) -> SQLDataModel:
+        """
         Returns a new ``SQLDataModel`` containing the total counts and unique values for each column in the model for both null and non-null values.
 
         Metrics:
             - ``'column'`` contains the names of the columns counted.
             - ``'na'`` contains the total number of null values in the column.
             - ``'unique'`` contains the total number of unique values in the column.
             - ``'count'`` contains the total number of non-null values in the column.
@@ -7562,15 +7611,15 @@
                 ('Alice', 25, 'Female')
             ]
 
             # Create the model
             sdm = SQLDataModel(data, headers)
 
             # Get the value count information
-            count_model = sdm.count()
+            count_model = sdm.column_counts()
 
             # View the count information
             print(count_model)
 
         This will output:
         
         ```shell            
@@ -7579,14 +7628,21 @@
             ├────────┼──────┼────────┼───────┼───────┤
             │ Name   │    0 │      2 │     3 │     3 │
             │ Age    │    0 │      2 │     3 │     3 │
             │ Gender │    1 │      1 │     2 │     3 │
             └────────┴──────┴────────┴───────┴───────┘
             [3 rows x 5 columns]
         ```
+
+        Change Log:
+            - Version 0.3.1 (2024-04-01):
+                - Renamed method from ``counts`` to ``column_counts`` for more precise definition.
+
+        Note:
+            - See :meth:`SQLDataModel.count()` for the count of non-null values for each column in a row-wise orientation.
         """
         fetch_stmt = " UNION ALL ".join([f"""select '{col}' as 'column', sum(case when "{col}" is null then 1 else 0 end) as 'na', count(distinct "{col}") as 'unique', count("{col}") as 'count',sum(case when "{col}" is null then 1 else 1 end) as 'total' from "{self.sql_model}" """ for col in self.headers])
         return self.execute_fetch(fetch_stmt)
 
     def deduplicate(self, subset:list[str]=None, reset_index:bool=True, keep_first:bool=True, inplace:bool=True) -> None|SQLDataModel:
         """
         Removes duplicate rows from the SQLDataModel based on the specified subset of columns. Deduplication occurs inplace by default, otherwise use ``inplace=False`` to return a new ``SQLDataModel``.
@@ -7917,14 +7973,108 @@
         except ValueError as e:
             raise ValueError(
                 SQLDataModel.ErrorFormat(f'ValueError: {e}, rename header or use `normalize_headers()` method to fix')
             ) from None
         res = self.sql_db_conn.execute(self._generate_sql_stmt(index=include_idx_col))
         yield from (Row(*x) for x in res.fetchall())
     
+    def min(self) -> SQLDataModel:
+        """
+        Returns a new ``SQLDataModel`` containing the minimum value of all non-null values for each column in a row-wise orientation.
+
+        Returns:
+            ``SQLDataModel``: A new SQLDataModel containing the minimum non-null value for each column.
+
+        Example::
+            
+            from SQLDataModel import SQLDataModel
+
+            # Sample data with missing values
+            headers = ['Name', 'Age', 'Gender', 'Tenure']
+            data = [
+                ('Alice', 25, 'Female', 1.0),
+                ('Bob', None, 'Male', 2.7),
+                ('Charlie', 30, 'Male', None),
+                ('David', None, 'Male', 3.8)
+            ]   
+
+            # Create the model
+            sdm = SQLDataModel(data, headers)
+
+            # Get minimum values
+            min_values = sdm.min()
+
+            # View result
+            print(min_values)
+
+        This will output the minimum value of all non-null values for each column:
+
+        ```shell
+            ┌───────┬─────┬────────┬────────┐
+            │ Name  │ Age │ Gender │ Tenure │
+            ├───────┼─────┼────────┼────────┤
+            │ Alice │  25 │ Female │   1.00 │
+            └───────┴─────┴────────┴────────┘
+            [1 rows x 4 columns]
+        ```
+
+        Note:
+            - See :meth:`SQLDataModel.column_counts()` for column-wise count of unique, null and total values for each column.
+            - See :meth:`SQLDataModel.max()` for returning the maximum values in each column.
+        """
+        fetch_stmt = " ".join(("select",",".join([f"""min("{col}") as "{col}" """ for col in self.headers]),f'from "{self.sql_model}"'))
+        return self.execute_fetch(fetch_stmt) 
+
+    def max(self) -> SQLDataModel:
+        """
+        Returns a new ``SQLDataModel`` containing the maximum value of all non-null values for each column in a row-wise orientation.
+
+        Returns:
+            ``SQLDataModel``: A new SQLDataModel containing the maximum non-null value for each column.
+
+        Example::
+            
+            from SQLDataModel import SQLDataModel
+
+            # Sample data with missing values
+            headers = ['Name', 'Age', 'Gender', 'Tenure']
+            data = [
+                ('Alice', 25, 'Female', 1.0),
+                ('Bob', None, 'Male', 2.7),
+                ('Charlie', 30, 'Male', None),
+                ('David', None, 'Male', 3.8)
+            ]   
+
+            # Create the model
+            sdm = SQLDataModel(data, headers)
+
+            # Get maximum values
+            min_values = sdm.min()
+
+            # View result
+            print(min_values)
+
+        This will output the maximum value of all non-null values for each column:
+
+        ```shell
+            ┌───────┬─────┬────────┬────────┐
+            │ Name  │ Age │ Gender │ Tenure │
+            ├───────┼─────┼────────┼────────┤
+            │ David │  30 │ Male   │   3.80 │
+            └───────┴─────┴────────┴────────┘
+            [1 rows x 4 columns]
+        ```
+
+        Note:
+            - See :meth:`SQLDataModel.column_counts()` for column-wise count of unique, null and total values for each column.
+            - See :meth:`SQLDataModel.min()` for returning the minimum values in each column.
+        """
+        fetch_stmt = " ".join(("select",",".join([f"""max("{col}") as "{col}" """ for col in self.headers]),f'from "{self.sql_model}"'))
+        return self.execute_fetch(fetch_stmt)     
+
     def merge(self, merge_with:SQLDataModel=None, how:Literal["left","right","inner","full outer","cross"]="left", left_on:str=None, right_on:str=None, include_join_column:bool=False) -> SQLDataModel:
         """
         Merges two ``SQLDataModel`` instances based on specified columns and merge type, ``how``, returning the result as a new instance. 
         If the join column shares the same name in both models, ``left_on`` and ``right_on`` column arguments are not required and will be inferred. Otherwise, explicit arguments for both are required.
 
         Parameters:
             ``merge_with`` (SQLDataModel): The SQLDataModel to merge with the current model.
```

### Comparing `SQLDataModel-0.3.0/src/SQLDataModel/StandardDeviation.py` & `SQLDataModel-0.3.1/src/SQLDataModel/StandardDeviation.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.0/src/SQLDataModel/converters.py` & `SQLDataModel-0.3.1/src/SQLDataModel/converters.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.0/src/SQLDataModel/demo.py` & `SQLDataModel-0.3.1/src/SQLDataModel/demo.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.0/src/SQLDataModel/exceptions.py` & `SQLDataModel-0.3.1/src/SQLDataModel/exceptions.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.0/src/SQLDataModel/extensions/str_utils.c` & `SQLDataModel-0.3.1/src/SQLDataModel/extensions/str_utils.c`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.0/src/SQLDataModel.egg-info/PKG-INFO` & `SQLDataModel-0.3.1/src/SQLDataModel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.0
+Version: 0.3.1
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
```

### Comparing `SQLDataModel-0.3.0/src/SQLDataModel.egg-info/SOURCES.txt` & `SQLDataModel-0.3.1/src/SQLDataModel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.0/tests/test_Future.py` & `SQLDataModel-0.3.1/tests/test_SQLDataModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime, os, tempfile, csv, sqlite3, random
 import pytest
 import pandas as pd
 import numpy as np
 from .random_data_generator import data_generator
-from future.SQLDataModel_future import SQLDataModel
+from src.SQLDataModel.SQLDataModel import SQLDataModel
 
 @pytest.fixture
 def sample_data() -> tuple[list[list], list[str]]:
     """Returns sample data in format `(data, headers)` to use for testing."""
     return data_generator(num_rows=120, float_precision=4, num_columns=8, seed=42, return_header_type='list', return_row_type='tuple', return_format='combined')
 
 @pytest.mark.core
@@ -643,8 +643,34 @@
         sdm = SQLDataModel(input_data,input_headers)
         if inplace:
             sdm.drop_column(drop_column, inplace=inplace)
         else:
             sdm = sdm.drop_column(drop_column, inplace=inplace)
         output_headers, output_data = sdm.get_headers(), sdm.data()
         assert output_headers == validation_headers
-        assert output_data == validation_data
+        assert output_data == validation_data
+
+@pytest.mark.core
+def test_count_min_max():
+    headers = ['string', 'int', 'float', 'bool', 'date', 'bytes', 'nonetype', 'datetime']
+    data = [
+         ['hTpigTHKcfoK', -356, -470.239667, None, datetime.date(1967, 5, 18), b'sNLjVGWGaub5', None, datetime.datetime(1954, 3, 9, 14, 15, 55)]
+        ,['mNHnKXaXQv', -565, -506.744985, True, datetime.date(2010, 1, 22), b'ppIeTY', None, datetime.datetime(2018, 2, 15, 17, 6, 3)]
+        ,['nVgx', 342, None, True, datetime.date(1992, 2, 22), b'ViCHq1_nGS', None, datetime.datetime(1983, 9, 27, 0, 5, 59)]
+        ,[None, 22, None, True, datetime.date(2013, 9, 25), b'RzPx3', None, None]
+        ,['sM2wmeOV90', -190, 169.17198, True, datetime.date(1934, 11, 11), None, None, datetime.datetime(1927, 7, 2, 5, 24)]
+        ,['xBZ', 811, None, False, datetime.date(1914, 5, 14), b'1e', None, datetime.datetime(1949, 5, 26, 14, 18, 27)]
+        ,['xnq6', None, -201.19899, True, None, b'rDGS2', None, datetime.datetime(1989, 12, 26, 17, 42, 45)]
+        ,['eNGpCr5QnuVd', 316, -561.358482, None, datetime.date(2022, 12, 24), b'CWXlgA_CSP9', None, datetime.datetime(1962, 3, 7, 9, 13, 3)]
+        ,['Xz', -61, 995.075213, False, datetime.date(1933, 9, 25), None, None, datetime.datetime(1974, 12, 18, 1, 47, 20)]
+        ,['n62', None, 19.052587, False, datetime.date(1922, 9, 4), b'plB', None, datetime.datetime(1907, 1, 19, 15, 32, 58)]
+    ]
+    expected_count = (9, 8, 7, 8, 9, 8, 0, 9)
+    expected_min = ('Xz', -565, -561.358482, '0', datetime.date(1914, 5, 14), b'1e', None, datetime.datetime(1907, 1, 19, 15, 32, 58))
+    expected_max = ('xnq6', 811, 995.075213, '1', datetime.date(2022, 12, 24), b'sNLjVGWGaub5', None, datetime.datetime(2018, 2, 15, 17, 6, 3))    
+    sdm = SQLDataModel(data, headers)
+    output_count = sdm.count().data()
+    output_min = sdm.min().data()
+    output_max = sdm.max().data()
+    assert output_count == expected_count
+    assert output_min == expected_min
+    assert output_max == expected_max
```

### Comparing `SQLDataModel-0.3.0/tests/test_SQLDataModel.py` & `SQLDataModel-0.3.1/tests/test_Future.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime, os, tempfile, csv, sqlite3, random
 import pytest
 import pandas as pd
 import numpy as np
 from .random_data_generator import data_generator
-from src.SQLDataModel.SQLDataModel import SQLDataModel
+from future.SQLDataModel_future import SQLDataModel
 
 @pytest.fixture
 def sample_data() -> tuple[list[list], list[str]]:
     """Returns sample data in format `(data, headers)` to use for testing."""
     return data_generator(num_rows=120, float_precision=4, num_columns=8, seed=42, return_header_type='list', return_row_type='tuple', return_format='combined')
 
 @pytest.mark.core
@@ -643,8 +643,34 @@
         sdm = SQLDataModel(input_data,input_headers)
         if inplace:
             sdm.drop_column(drop_column, inplace=inplace)
         else:
             sdm = sdm.drop_column(drop_column, inplace=inplace)
         output_headers, output_data = sdm.get_headers(), sdm.data()
         assert output_headers == validation_headers
-        assert output_data == validation_data
+        assert output_data == validation_data
+
+@pytest.mark.core
+def test_count_min_max():
+    headers = ['string', 'int', 'float', 'bool', 'date', 'bytes', 'nonetype', 'datetime']
+    data = [
+         ['hTpigTHKcfoK', -356, -470.239667, None, datetime.date(1967, 5, 18), b'sNLjVGWGaub5', None, datetime.datetime(1954, 3, 9, 14, 15, 55)]
+        ,['mNHnKXaXQv', -565, -506.744985, True, datetime.date(2010, 1, 22), b'ppIeTY', None, datetime.datetime(2018, 2, 15, 17, 6, 3)]
+        ,['nVgx', 342, None, True, datetime.date(1992, 2, 22), b'ViCHq1_nGS', None, datetime.datetime(1983, 9, 27, 0, 5, 59)]
+        ,[None, 22, None, True, datetime.date(2013, 9, 25), b'RzPx3', None, None]
+        ,['sM2wmeOV90', -190, 169.17198, True, datetime.date(1934, 11, 11), None, None, datetime.datetime(1927, 7, 2, 5, 24)]
+        ,['xBZ', 811, None, False, datetime.date(1914, 5, 14), b'1e', None, datetime.datetime(1949, 5, 26, 14, 18, 27)]
+        ,['xnq6', None, -201.19899, True, None, b'rDGS2', None, datetime.datetime(1989, 12, 26, 17, 42, 45)]
+        ,['eNGpCr5QnuVd', 316, -561.358482, None, datetime.date(2022, 12, 24), b'CWXlgA_CSP9', None, datetime.datetime(1962, 3, 7, 9, 13, 3)]
+        ,['Xz', -61, 995.075213, False, datetime.date(1933, 9, 25), None, None, datetime.datetime(1974, 12, 18, 1, 47, 20)]
+        ,['n62', None, 19.052587, False, datetime.date(1922, 9, 4), b'plB', None, datetime.datetime(1907, 1, 19, 15, 32, 58)]
+    ]
+    expected_count = (9, 8, 7, 8, 9, 8, 0, 9)
+    expected_min = ('Xz', -565, -561.358482, '0', datetime.date(1914, 5, 14), b'1e', None, datetime.datetime(1907, 1, 19, 15, 32, 58))
+    expected_max = ('xnq6', 811, 995.075213, '1', datetime.date(2022, 12, 24), b'sNLjVGWGaub5', None, datetime.datetime(2018, 2, 15, 17, 6, 3))    
+    sdm = SQLDataModel(data, headers)
+    output_count = sdm.count().data()
+    output_min = sdm.min().data()
+    output_max = sdm.max().data()
+    assert output_count == expected_count
+    assert output_min == expected_min
+    assert output_max == expected_max
```

