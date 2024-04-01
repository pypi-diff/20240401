# Comparing `tmp/ReferenceDataAccess-0.1.0.tar.gz` & `tmp/ReferenceDataAccess-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReferenceDataAccess-0.1.0.tar", last modified: Thu Mar 28 12:15:12 2024, max compression
+gzip compressed data, was "ReferenceDataAccess-0.1.1.tar", last modified: Mon Apr  1 14:54:20 2024, max compression
```

## Comparing `ReferenceDataAccess-0.1.0.tar` & `ReferenceDataAccess-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 murali    (1000) murali    (1000)        0 2024-03-28 12:15:12.400840 ReferenceDataAccess-0.1.0/
--rw-r--r--   0 murali    (1000) murali    (1000)       33 2023-11-16 07:11:42.000000 ReferenceDataAccess-0.1.0/MANIFEST.in
--rw-r--r--   0 murali    (1000) murali    (1000)    16499 2024-03-28 12:15:12.400840 ReferenceDataAccess-0.1.0/PKG-INFO
--rw-r--r--   0 murali    (1000) murali    (1000)    16064 2024-01-12 13:51:10.000000 ReferenceDataAccess-0.1.0/README.md
-drwxr-xr-x   0 murali    (1000) murali    (1000)        0 2024-03-28 12:15:12.390840 ReferenceDataAccess-0.1.0/ReferenceDataAccess.egg-info/
--rw-r--r--   0 murali    (1000) murali    (1000)    16499 2024-03-28 12:15:12.000000 ReferenceDataAccess-0.1.0/ReferenceDataAccess.egg-info/PKG-INFO
--rw-r--r--   0 murali    (1000) murali    (1000)      372 2024-03-28 12:15:12.000000 ReferenceDataAccess-0.1.0/ReferenceDataAccess.egg-info/SOURCES.txt
--rw-r--r--   0 murali    (1000) murali    (1000)        1 2024-03-28 12:15:12.000000 ReferenceDataAccess-0.1.0/ReferenceDataAccess.egg-info/dependency_links.txt
--rw-r--r--   0 murali    (1000) murali    (1000)        9 2024-03-28 12:15:12.000000 ReferenceDataAccess-0.1.0/ReferenceDataAccess.egg-info/requires.txt
--rw-r--r--   0 murali    (1000) murali    (1000)       11 2024-03-28 12:15:12.000000 ReferenceDataAccess-0.1.0/ReferenceDataAccess.egg-info/top_level.txt
-drwxr-xr-x   0 murali    (1000) murali    (1000)        0 2024-03-28 12:15:12.390840 ReferenceDataAccess-0.1.0/dataAccess/
--rw-r--r--   0 murali    (1000) murali    (1000)    11246 2024-03-28 10:44:06.000000 ReferenceDataAccess-0.1.0/dataAccess/EquityApi.py
--rw-r--r--   0 murali    (1000) murali    (1000)    11577 2024-03-12 12:56:47.000000 ReferenceDataAccess-0.1.0/dataAccess/EtdApi.py
--rw-r--r--   0 murali    (1000) murali    (1000)    10938 2023-11-16 07:11:51.000000 ReferenceDataAccess-0.1.0/dataAccess/EtdHistoryApi.py
--rw-r--r--   0 murali    (1000) murali    (1000)    21825 2023-11-16 07:11:51.000000 ReferenceDataAccess-0.1.0/dataAccess/EtdUtil.py
--rw-r--r--   0 murali    (1000) murali    (1000)       91 2023-11-16 07:11:52.000000 ReferenceDataAccess-0.1.0/dataAccess/__init__.py
--rw-r--r--   0 murali    (1000) murali    (1000)       79 2024-03-28 12:15:12.400840 ReferenceDataAccess-0.1.0/setup.cfg
--rw-r--r--   0 murali    (1000) murali    (1000)     1474 2024-03-28 12:14:33.000000 ReferenceDataAccess-0.1.0/setup.py
+drwxr-xr-x   0 murali    (1000) murali    (1000)        0 2024-04-01 14:54:20.453189 ReferenceDataAccess-0.1.1/
+-rw-r--r--   0 murali    (1000) murali    (1000)       33 2023-11-16 07:11:42.000000 ReferenceDataAccess-0.1.1/MANIFEST.in
+-rw-r--r--   0 murali    (1000) murali    (1000)    16499 2024-04-01 14:54:20.453189 ReferenceDataAccess-0.1.1/PKG-INFO
+-rw-r--r--   0 murali    (1000) murali    (1000)    16064 2024-01-12 13:51:10.000000 ReferenceDataAccess-0.1.1/README.md
+drwxr-xr-x   0 murali    (1000) murali    (1000)        0 2024-04-01 14:54:20.453189 ReferenceDataAccess-0.1.1/ReferenceDataAccess.egg-info/
+-rw-r--r--   0 murali    (1000) murali    (1000)    16499 2024-04-01 14:54:20.000000 ReferenceDataAccess-0.1.1/ReferenceDataAccess.egg-info/PKG-INFO
+-rw-r--r--   0 murali    (1000) murali    (1000)      372 2024-04-01 14:54:20.000000 ReferenceDataAccess-0.1.1/ReferenceDataAccess.egg-info/SOURCES.txt
+-rw-r--r--   0 murali    (1000) murali    (1000)        1 2024-04-01 14:54:20.000000 ReferenceDataAccess-0.1.1/ReferenceDataAccess.egg-info/dependency_links.txt
+-rw-r--r--   0 murali    (1000) murali    (1000)        9 2024-04-01 14:54:20.000000 ReferenceDataAccess-0.1.1/ReferenceDataAccess.egg-info/requires.txt
+-rw-r--r--   0 murali    (1000) murali    (1000)       11 2024-04-01 14:54:20.000000 ReferenceDataAccess-0.1.1/ReferenceDataAccess.egg-info/top_level.txt
+drwxr-xr-x   0 murali    (1000) murali    (1000)        0 2024-04-01 14:54:20.453189 ReferenceDataAccess-0.1.1/dataAccess/
+-rw-r--r--   0 murali    (1000) murali    (1000)    11246 2024-03-28 10:44:06.000000 ReferenceDataAccess-0.1.1/dataAccess/EquityApi.py
+-rw-r--r--   0 murali    (1000) murali    (1000)    11577 2024-03-12 12:56:47.000000 ReferenceDataAccess-0.1.1/dataAccess/EtdApi.py
+-rw-r--r--   0 murali    (1000) murali    (1000)    10938 2023-11-16 07:11:51.000000 ReferenceDataAccess-0.1.1/dataAccess/EtdHistoryApi.py
+-rw-r--r--   0 murali    (1000) murali    (1000)    21827 2024-04-01 14:53:37.000000 ReferenceDataAccess-0.1.1/dataAccess/EtdUtil.py
+-rw-r--r--   0 murali    (1000) murali    (1000)       91 2023-11-16 07:11:52.000000 ReferenceDataAccess-0.1.1/dataAccess/__init__.py
+-rw-r--r--   0 murali    (1000) murali    (1000)       79 2024-04-01 14:54:20.453189 ReferenceDataAccess-0.1.1/setup.cfg
+-rw-r--r--   0 murali    (1000) murali    (1000)     1474 2024-04-01 14:54:14.000000 ReferenceDataAccess-0.1.1/setup.py
```

### Comparing `ReferenceDataAccess-0.1.0/PKG-INFO` & `ReferenceDataAccess-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReferenceDataAccess
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python library to easily fetch reference data from RduAccess and integrate it with your python application
 Author: Jay Sangoi
 Author-email: jay.sangoi@gmail.com
 License: MIT
 Keywords: stocks,market,finance,RduAccess,quotes,derivatives,equity,fixed income,Mifid,shares,Reference Data,isin,sedol,id_bb_global
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `ReferenceDataAccess-0.1.0/README.md` & `ReferenceDataAccess-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ReferenceDataAccess-0.1.0/ReferenceDataAccess.egg-info/PKG-INFO` & `ReferenceDataAccess-0.1.1/ReferenceDataAccess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReferenceDataAccess
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python library to easily fetch reference data from RduAccess and integrate it with your python application
 Author: Jay Sangoi
 Author-email: jay.sangoi@gmail.com
 License: MIT
 Keywords: stocks,market,finance,RduAccess,quotes,derivatives,equity,fixed income,Mifid,shares,Reference Data,isin,sedol,id_bb_global
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `ReferenceDataAccess-0.1.0/dataAccess/EquityApi.py` & `ReferenceDataAccess-0.1.1/dataAccess/EquityApi.py`

 * *Files identical despite different names*

### Comparing `ReferenceDataAccess-0.1.0/dataAccess/EtdApi.py` & `ReferenceDataAccess-0.1.1/dataAccess/EtdApi.py`

 * *Files identical despite different names*

### Comparing `ReferenceDataAccess-0.1.0/dataAccess/EtdHistoryApi.py` & `ReferenceDataAccess-0.1.1/dataAccess/EtdHistoryApi.py`

 * *Files identical despite different names*

### Comparing `ReferenceDataAccess-0.1.0/dataAccess/EtdUtil.py` & `ReferenceDataAccess-0.1.1/dataAccess/EtdUtil.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 def convert_json_to_df(key, input_key, json_data, fetchUnderlying: False, columnList=[]):
     df = pd.json_normalize(json_data)
     msg = df.get('message')
     product_dict = {}
     if isinstance(msg, pd.Series):
         message = msg.loc[0]
-        contract_dict = {'sucess': False, 'failed_message': message}
+        contract_dict = {'success': False, 'failed_message': message}
         product_dict[input_key] = contract_dict
     else:
         for index, row in df.iterrows():
             """product_list.append(row['basics.name'])
             product_list.append(row['basics.roundLotSz'])
             product_list.append(row['ids.clrngCd'])
             """
@@ -115,15 +115,15 @@
                 c_tradelines = contract['tradeLines']['tradeLine']
 
                 for c_tradeline in c_tradelines:
                     contract_dict = {}
 
                     ct_basics = c_tradeline['basics']
 
-                    contract_dict['sucess'] = True
+                    contract_dict['success'] = True
                     # print(ct_basics.get('segTp'))
                     if 'exchCd' in columnList:    contract_dict['exchCd'] = ct_basics.get('exchCd')
                     if 'lstngCycleTp' in columnList:    contract_dict['lstngCycleTp'] = ct_basics.get('lstngCycleTp')
                     if 'omic' in columnList:    contract_dict['omic'] = ct_basics.get('omic')
                     if 'segTp' in columnList:    contract_dict['segTp'] = ct_basics.get('segTp')
                     if 'smic' in columnList:    contract_dict['smic'] = ct_basics.get('smic')
                     if 'tckSz' in columnList:    contract_dict['tckSz'] = ct_basics.get('tckSz')
```

### Comparing `ReferenceDataAccess-0.1.0/setup.py` & `ReferenceDataAccess-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
     
 setuptools.setup(
     name="ReferenceDataAccess", 
-    version="0.1.0",
+    version="0.1.1",
     author="Jay Sangoi",
     author_email="jay.sangoi@gmail.com",
     license='MIT',
     description='A python library to easily fetch reference data from RduAccess and integrate it with your python application',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

