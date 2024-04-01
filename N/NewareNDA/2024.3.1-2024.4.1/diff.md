# Comparing `tmp/NewareNDA-2024.3.1.tar.gz` & `tmp/NewareNDA-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NewareNDA-2024.3.1.tar", last modified: Fri Mar  1 19:22:42 2024, max compression
+gzip compressed data, was "NewareNDA-2024.4.1.tar", last modified: Mon Apr  1 13:51:41 2024, max compression
```

## Comparing `NewareNDA-2024.3.1.tar` & `NewareNDA-2024.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-03-01 19:22:42.442476 NewareNDA-2024.3.1/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1488 2023-02-02 18:25:45.000000 NewareNDA-2024.3.1/LICENSE
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-03-01 19:22:42.438476 NewareNDA-2024.3.1/NewareNDA/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    11344 2024-02-27 19:28:36.000000 NewareNDA-2024.3.1/NewareNDA/NewareNDA.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    14218 2024-03-01 18:29:25.000000 NewareNDA-2024.3.1/NewareNDA/NewareNDAx.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      101 2023-10-03 15:33:50.000000 NewareNDA-2024.3.1/NewareNDA/__init__.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1645 2024-03-01 18:29:25.000000 NewareNDA-2024.3.1/NewareNDA/dicts.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       28 2024-03-01 18:29:25.000000 NewareNDA-2024.3.1/NewareNDA/version.py
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-03-01 19:22:42.442476 NewareNDA-2024.3.1/NewareNDA.egg-info/
--rw-r--r--   0 cogswell  (1001) cogswell  (1001)     1813 2024-03-01 19:22:42.000000 NewareNDA-2024.3.1/NewareNDA.egg-info/PKG-INFO
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      344 2024-03-01 19:22:42.000000 NewareNDA-2024.3.1/NewareNDA.egg-info/SOURCES.txt
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)        1 2024-03-01 19:22:42.000000 NewareNDA-2024.3.1/NewareNDA.egg-info/dependency_links.txt
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       30 2024-03-01 19:22:42.000000 NewareNDA-2024.3.1/NewareNDA.egg-info/requires.txt
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       10 2024-03-01 19:22:42.000000 NewareNDA-2024.3.1/NewareNDA.egg-info/top_level.txt
--rw-r--r--   0 cogswell  (1001) cogswell  (1001)     1813 2024-03-01 19:22:42.442476 NewareNDA-2024.3.1/PKG-INFO
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1318 2024-03-01 18:29:25.000000 NewareNDA-2024.3.1/README.md
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-03-01 19:22:42.442476 NewareNDA-2024.3.1/bin/
--rwxrwxr-x   0 cogswell  (1001) cogswell  (1001)     1405 2023-10-03 15:33:50.000000 NewareNDA-2024.3.1/bin/NewareNDA-cli.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       38 2024-03-01 19:22:42.442476 NewareNDA-2024.3.1/setup.cfg
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      955 2024-02-05 15:20:31.000000 NewareNDA-2024.3.1/setup.py
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-03-01 19:22:42.442476 NewareNDA-2024.3.1/tests/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      209 2024-02-05 15:31:56.000000 NewareNDA-2024.3.1/tests/test_NewareNDA.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-01 13:51:41.055063 NewareNDA-2024.4.1/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1488 2023-02-02 18:25:45.000000 NewareNDA-2024.4.1/LICENSE
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-01 13:51:41.051063 NewareNDA-2024.4.1/NewareNDA/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    11344 2024-03-26 18:47:09.000000 NewareNDA-2024.4.1/NewareNDA/NewareNDA.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    14809 2024-04-01 13:41:36.000000 NewareNDA-2024.4.1/NewareNDA/NewareNDAx.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      101 2023-10-03 15:33:50.000000 NewareNDA-2024.4.1/NewareNDA/__init__.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1677 2024-04-01 13:48:28.000000 NewareNDA-2024.4.1/NewareNDA/dicts.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       28 2024-04-01 13:48:28.000000 NewareNDA-2024.4.1/NewareNDA/version.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-01 13:51:41.055063 NewareNDA-2024.4.1/NewareNDA.egg-info/
+-rw-r--r--   0 cogswell  (1001) cogswell  (1001)     2271 2024-04-01 13:51:41.000000 NewareNDA-2024.4.1/NewareNDA.egg-info/PKG-INFO
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      344 2024-04-01 13:51:41.000000 NewareNDA-2024.4.1/NewareNDA.egg-info/SOURCES.txt
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)        1 2024-04-01 13:51:41.000000 NewareNDA-2024.4.1/NewareNDA.egg-info/dependency_links.txt
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       40 2024-04-01 13:51:41.000000 NewareNDA-2024.4.1/NewareNDA.egg-info/requires.txt
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       10 2024-04-01 13:51:41.000000 NewareNDA-2024.4.1/NewareNDA.egg-info/top_level.txt
+-rw-r--r--   0 cogswell  (1001) cogswell  (1001)     2271 2024-04-01 13:51:41.055063 NewareNDA-2024.4.1/PKG-INFO
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1734 2024-04-01 13:41:36.000000 NewareNDA-2024.4.1/README.md
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-01 13:51:41.051063 NewareNDA-2024.4.1/bin/
+-rwxrwxr-x   0 cogswell  (1001) cogswell  (1001)     1405 2023-10-03 15:33:50.000000 NewareNDA-2024.4.1/bin/NewareNDA-cli.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       38 2024-04-01 13:51:41.055063 NewareNDA-2024.4.1/setup.cfg
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      968 2024-04-01 13:41:36.000000 NewareNDA-2024.4.1/setup.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-01 13:51:41.055063 NewareNDA-2024.4.1/tests/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      209 2024-03-08 19:10:17.000000 NewareNDA-2024.4.1/tests/test_NewareNDA.py
```

### Comparing `NewareNDA-2024.3.1/LICENSE` & `NewareNDA-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `NewareNDA-2024.3.1/NewareNDA/NewareNDA.py` & `NewareNDA-2024.4.1/NewareNDA/NewareNDA.py`

 * *Files identical despite different names*

### Comparing `NewareNDA-2024.3.1/NewareNDA/NewareNDAx.py` & `NewareNDA-2024.4.1/NewareNDA/NewareNDAx.py`

 * *Files 5% similar despite different names*

```diff
@@ -137,14 +137,15 @@
     chg = df['Charge_Energy(mWh)'].ffill() + \
         inc.where(df['Current(mA)'] > 0, 0).shift()
     dch = df['Discharge_Energy(mWh)'].ffill() + \
         inc.where(df['Current(mA)'] < 0, 0).shift()
     df['Charge_Energy(mWh)'] = df['Charge_Energy(mWh)'].where(nan_mask, chg)
     df['Discharge_Energy(mWh)'] = df['Discharge_Energy(mWh)'].where(nan_mask, dch)
 
+
 def _read_data_ndc(file):
     with open(file, 'rb') as f:
         mm = mmap.mmap(f.fileno(), 0, access=mmap.ACCESS_READ)
         mm_size = mm.size()
 
         # Identify the beginning of the data section
         record_len = 4096
@@ -247,66 +248,91 @@
     with open(file, 'rb') as f:
         mm = mmap.mmap(f.fileno(), 0, access=mmap.ACCESS_READ)
 
         # Get ndc file version
         [ndc_version] = struct.unpack('<B', mm[2:3])
         logging.info(f"NDC version: {ndc_version}")
 
-        if ndc_version == 11:
+        if ndc_version == 5:
+            return _read_ndc_5(mm)
+        elif ndc_version == 11:
             return _read_ndc_11(mm)
 
         # Identify the beginning of the data section
         record_len = 94
         offset = 0
         identifier = mm[517:525]
         id_byte = slice(0, 1)
         rec_byte = slice(0, 1)
-        if identifier == b'\x00\x00\x00\x00\x00\x00\x00\x00':
-            record_len = 90
-            offset = 4
-            identifier = mm[4225:4229]
-            id_byte = slice(3, 4)
-            rec_byte = slice(7, 8)
 
         # Read data records
         output = []
         aux = []
         header = mm.find(identifier)
         while header != -1:
             mm.seek(header - offset)
             bytes = mm.read(record_len)
             if bytes[rec_byte] == b'\x55':
-                if _valid_record(bytes):
-                    output.append(_bytes_to_list_ndc(bytes))
+                output.append(_bytes_to_list_ndc(bytes))
             elif bytes[rec_byte] == b'\x65':
                 aux.append(_aux_bytes_65_to_list_ndc(bytes))
             elif bytes[rec_byte] == b'\x74':
                 aux.append(_aux_bytes_74_to_list_ndc(bytes))
             else:
                 logging.warning("Unknown record type: "+bytes[rec_byte].hex())
 
             header = mm.find(identifier, header - offset + record_len)
 
     # Create DataFrame and sort by Index
     df = pd.DataFrame(output, columns=rec_columns)
-    df.drop_duplicates(subset='Index', inplace=True)
-
-    if not df['Index'].is_monotonic_increasing:
-        df.sort_values('Index', inplace=True)
-
-    df.reset_index(drop=True, inplace=True)
 
     # Postprocessing
     aux_df = pd.DataFrame([])
     df = df.astype(dtype=dtype_dict)
     if identifier[id_byte] == b'\x65':
         aux_df = pd.DataFrame(aux, columns=['Index', 'Aux', 'V', 'T'])
     elif identifier[id_byte] == b'\x74':
         aux_df = pd.DataFrame(aux, columns=['Index', 'Aux', 'V', 'T', 't'])
-    aux_df.drop_duplicates(subset='Index', inplace=True)
+
+    return df, aux_df
+
+
+def _read_ndc_5(mm):
+    """Helper function that reads records and aux data from ndc version 5"""
+    mm_size = mm.size()
+    record_len = 4096
+    header = 4096
+    rec_byte = slice(7, 8)
+
+    # Read data records
+    output = []
+    aux65 = []
+    aux74 = []
+    mm.seek(header)
+    while mm.tell() < mm_size:
+        bytes = mm.read(record_len)
+        for i in struct.iter_unpack('<87s', bytes[125:-56]):
+            if i[0][rec_byte] == b'\x55':
+                output.append(_bytes_to_list_ndc(i[0]))
+            if i[0][rec_byte] == b'\x65':
+                aux65.append(_aux_bytes_65_to_list_ndc(i[0]))
+            elif i[0][rec_byte] == b'\x74':
+                aux74.append(_aux_bytes_74_to_list_ndc(i[0]))
+
+    # Create DataFrames
+    df = pd.DataFrame(output, columns=rec_columns)
+
+    # Concat aux65 and aux74 if they both contain data
+    aux_df = pd.DataFrame(aux65, columns=['Index', 'Aux', 'V', 'T'])
+    aux74_df = pd.DataFrame(aux74, columns=['Index', 'Aux', 'V', 'T', 't'])
+    if (not aux_df.empty) & (not aux74_df.empty):
+        aux_df = pd.concat([aux_df, aux74_df.drop(columns=['t'])])
+    elif (not aux74_df.empty):
+        aux_df = aux74_df
+
     return df, aux_df
 
 
 def _read_ndc_11(mm):
     """Helper function that reads aux data from ndc version 11"""
     mm_size = mm.size()
     record_len = 4096
@@ -323,20 +349,14 @@
 
     # Create DataFrame
     aux_df = pd.DataFrame(aux, columns=['V', 'T'])
     aux_df['Index'] = aux_df.index + 1
     return None, aux_df
 
 
-def _valid_record(bytes):
-    """Helper function to identify a valid record"""
-    [Status] = struct.unpack('<B', bytes[17:18])
-    return (Status != 0) & (Status != 255)
-
-
 def _bytes_to_list_ndc(bytes):
     """Helper function for interpreting an ndc byte string"""
 
     # Extract fields from byte string
     [Index, Cycle] = struct.unpack('<II', bytes[8:16])
     [Step] = struct.unpack('<B', bytes[16:17])
     [Status] = struct.unpack('<B', bytes[17:18])
```

### Comparing `NewareNDA-2024.3.1/NewareNDA/dicts.py` & `NewareNDA-2024.4.1/NewareNDA/dicts.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     -1000: 1e-2,
     -500: 1e-3,
     -100: 1e-3,
     -50: 1e-4,
     -25: 1e-4,
     -20: 1e-4,
     -10: 1e-4,
+    -5: 1e-4,
     -2: 1e-5,
     -1: 1e-5,
     0: 0,
     1: 1e-4,
     5: 1e-4,
     10: 1e-3,
     100: 1e-2,
@@ -73,8 +74,9 @@
     1000: 1e-1,
     6000: 1e-1,
     10000: 1e-1,
     12000: 1e-1,
     50000: 1e-1,
     60000: 1e-1,
     100000: 1e-1,
+    200000: 1e-1,
 }
```

### Comparing `NewareNDA-2024.3.1/NewareNDA.egg-info/PKG-INFO` & `NewareNDA-2024.4.1/NewareNDA.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: NewareNDA
-Version: 2024.3.1
+Version: 2024.4.1
 Summary: Neware nda binary file reader.
 Home-page: https://github.com/Solid-Energy-Systems/NewareNDA
 Author: Daniel Cogswell
 Author-email: danielcogswell@ses.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pyarrow; extra == "test"
+Requires-Dist: coveralls; extra == "test"
 
 [![release](https://img.shields.io/github/v/release/Solid-Energy-Systems/NewareNDA)](https://github.com/Solid-Energy-Systems/NewareNDA/releases)
-
+[![NewareNDA regression tests](https://github.com/Solid-Energy-Systems/NewareNDA/actions/workflows/NewareNDA_pytest.yml/badge.svg)](https://github.com/Solid-Energy-Systems/NewareNDA/actions/workflows/NewareNDA_pytest.yml)
+[![Coverage Status](https://coveralls.io/repos/github/Solid-Energy-Systems/NewareNDA/badge.svg?branch=development)](https://coveralls.io/github/Solid-Energy-Systems/NewareNDA?branch=development)
 # NewareNDA
 
 © 2024 Copyright SES AI
 <br>Author: Daniel Cogswell
 <br>Email: danielcogswell@ses.ai
 
 Python module and command line tool for reading and converting Neware nda and ndax battery cycling files. Auxiliary temperature fields are currently supported in both formats.
```

### Comparing `NewareNDA-2024.3.1/PKG-INFO` & `NewareNDA-2024.4.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: NewareNDA
-Version: 2024.3.1
+Version: 2024.4.1
 Summary: Neware nda binary file reader.
 Home-page: https://github.com/Solid-Energy-Systems/NewareNDA
 Author: Daniel Cogswell
 Author-email: danielcogswell@ses.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pyarrow; extra == "test"
+Requires-Dist: coveralls; extra == "test"
 
 [![release](https://img.shields.io/github/v/release/Solid-Energy-Systems/NewareNDA)](https://github.com/Solid-Energy-Systems/NewareNDA/releases)
-
+[![NewareNDA regression tests](https://github.com/Solid-Energy-Systems/NewareNDA/actions/workflows/NewareNDA_pytest.yml/badge.svg)](https://github.com/Solid-Energy-Systems/NewareNDA/actions/workflows/NewareNDA_pytest.yml)
+[![Coverage Status](https://coveralls.io/repos/github/Solid-Energy-Systems/NewareNDA/badge.svg?branch=development)](https://coveralls.io/github/Solid-Energy-Systems/NewareNDA?branch=development)
 # NewareNDA
 
 © 2024 Copyright SES AI
 <br>Author: Daniel Cogswell
 <br>Email: danielcogswell@ses.ai
 
 Python module and command line tool for reading and converting Neware nda and ndax battery cycling files. Auxiliary temperature fields are currently supported in both formats.
```

### Comparing `NewareNDA-2024.3.1/README.md` & `NewareNDA-2024.4.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [![release](https://img.shields.io/github/v/release/Solid-Energy-Systems/NewareNDA)](https://github.com/Solid-Energy-Systems/NewareNDA/releases)
-
+[![NewareNDA regression tests](https://github.com/Solid-Energy-Systems/NewareNDA/actions/workflows/NewareNDA_pytest.yml/badge.svg)](https://github.com/Solid-Energy-Systems/NewareNDA/actions/workflows/NewareNDA_pytest.yml)
+[![Coverage Status](https://coveralls.io/repos/github/Solid-Energy-Systems/NewareNDA/badge.svg?branch=development)](https://coveralls.io/github/Solid-Energy-Systems/NewareNDA?branch=development)
 # NewareNDA
 
 © 2024 Copyright SES AI
 <br>Author: Daniel Cogswell
 <br>Email: danielcogswell@ses.ai
 
 Python module and command line tool for reading and converting Neware nda and ndax battery cycling files. Auxiliary temperature fields are currently supported in both formats.
```

### Comparing `NewareNDA-2024.3.1/bin/NewareNDA-cli.py` & `NewareNDA-2024.4.1/bin/NewareNDA-cli.py`

 * *Files identical despite different names*

### Comparing `NewareNDA-2024.3.1/setup.py` & `NewareNDA-2024.4.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,13 +21,13 @@
     author='Daniel Cogswell',
     author_email='danielcogswell@ses.ai',
     url='https://github.com/Solid-Energy-Systems/NewareNDA',
     license='BSD-3-Clause',
     packages=['NewareNDA'],
     scripts=['bin/NewareNDA-cli.py'],
     install_requires=['pandas'],
-    extras_require={'test': ['pytest', 'pyarrow']},
+    extras_require={'test': ['pytest', 'pyarrow', 'coveralls']},
     python_requires='>=3.6',
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
 )
```

