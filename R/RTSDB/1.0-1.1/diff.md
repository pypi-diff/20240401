# Comparing `tmp/RTSDB-1.0.tar.gz` & `tmp/RTSDB-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RTSDB-1.0.tar", last modified: Mon Apr  1 09:12:55 2024, max compression
+gzip compressed data, was "RTSDB-1.1.tar", last modified: Mon Apr  1 09:37:08 2024, max compression
```

## Comparing `RTSDB-1.0.tar` & `RTSDB-1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 09:12:55.255179 RTSDB-1.0/
--rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTSDB-1.0/LICENCE
--rw-rw-rw-   0        0        0     7020 2024-04-01 09:12:55.255179 RTSDB-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6321 2024-04-01 09:03:22.000000 RTSDB-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 09:12:55.252121 RTSDB-1.0/RTSDB.egg-info/
--rw-rw-rw-   0        0        0     7020 2024-04-01 09:12:55.000000 RTSDB-1.0/RTSDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-04-01 09:12:55.000000 RTSDB-1.0/RTSDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 09:12:55.000000 RTSDB-1.0/RTSDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-01 09:12:55.000000 RTSDB-1.0/RTSDB.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-01 09:12:55.254679 RTSDB-1.0/RTSDataBase/
--rw-rw-rw-   0        0        0    11847 2024-04-01 09:02:34.000000 RTSDB-1.0/RTSDataBase/RTSDB.py
--rw-rw-rw-   0        0        0       21 2024-04-01 08:52:47.000000 RTSDB-1.0/RTSDataBase/__init__.py
--rw-rw-rw-   0        0        0      600 2024-03-31 19:14:15.000000 RTSDB-1.0/RTSDataBase/exceptions.py
--rw-rw-rw-   0        0        0      569 2024-03-31 15:51:44.000000 RTSDB-1.0/RTSDataBase/typotest.py
--rw-rw-rw-   0        0        0       42 2024-04-01 09:12:55.256182 RTSDB-1.0/setup.cfg
--rw-rw-rw-   0        0        0      867 2024-04-01 09:12:53.000000 RTSDB-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:37:08.945581 RTSDB-1.1/
+-rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTSDB-1.1/LICENCE
+-rw-rw-rw-   0        0        0     7014 2024-04-01 09:37:08.945081 RTSDB-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6321 2024-04-01 09:19:36.000000 RTSDB-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 09:37:08.942028 RTSDB-1.1/RTSDB.egg-info/
+-rw-rw-rw-   0        0        0     7014 2024-04-01 09:37:08.000000 RTSDB-1.1/RTSDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-04-01 09:37:08.000000 RTSDB-1.1/RTSDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 09:37:08.000000 RTSDB-1.1/RTSDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-01 09:37:08.000000 RTSDB-1.1/RTSDB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 09:37:08.944576 RTSDB-1.1/RTSDataBase/
+-rw-rw-rw-   0        0        0    11935 2024-04-01 09:36:40.000000 RTSDB-1.1/RTSDataBase/RTSDB.py
+-rw-rw-rw-   0        0        0       21 2024-04-01 08:52:47.000000 RTSDB-1.1/RTSDataBase/__init__.py
+-rw-rw-rw-   0        0        0      600 2024-03-31 19:14:15.000000 RTSDB-1.1/RTSDataBase/exceptions.py
+-rw-rw-rw-   0        0        0      569 2024-03-31 15:51:44.000000 RTSDB-1.1/RTSDataBase/typotest.py
+-rw-rw-rw-   0        0        0       42 2024-04-01 09:37:08.946081 RTSDB-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      861 2024-04-01 09:37:01.000000 RTSDB-1.1/setup.py
```

### Comparing `RTSDB-1.0/LICENCE` & `RTSDB-1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `RTSDB-1.0/PKG-INFO` & `RTSDB-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: RTSDB
-Version: 1.0
+Version: 1.1
 Summary: Create yourself a simple database with this package.
-Home-page: https://github.com/RandomTimeLP/RTS_Simpeldatabase/
+Home-page: https://github.com/RandomTimeLP/RTS_DataBase/
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: database
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RTSDB-1.0/README.md` & `RTSDB-1.1/README.md`

 * *Files identical despite different names*

### Comparing `RTSDB-1.0/RTSDB.egg-info/PKG-INFO` & `RTSDB-1.1/RTSDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: RTSDB
-Version: 1.0
+Version: 1.1
 Summary: Create yourself a simple database with this package.
-Home-page: https://github.com/RandomTimeLP/RTS_Simpeldatabase/
+Home-page: https://github.com/RandomTimeLP/RTS_DataBase/
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: database
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RTSDB-1.0/RTSDataBase/RTSDB.py` & `RTSDB-1.1/RTSDataBase/RTSDB.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,24 +105,26 @@
     def create(self, record):
         
         if self.header is None:
             raise NotImplementedError(r"⚠️ ERROR: No header set. 'Database.setHeader({...})'")
         
         unique_fields = [field for field, state in zip(self.header["fields"], self.header["states"]) if state in  ["unique", "ul"]]
         index_fields = [field for field, state in zip(self.header["fields"], self.header["states"]) if state == "index"]
+        try:
+            for ex_record in self.data:
+                for u_field in unique_fields:
+                    if record.get(u_field) is not None and record.get(u_field) == ex_record[u_field]:
+                        raise ValueError(f"⚠️  Warning: Record with >>> {u_field}={record[u_field]} <<< already exists")
 
-        for ex_record in self.data:
-            for u_field in unique_fields:
-                if record.get(u_field) is not None and record.get(u_field) == ex_record[u_field]:
-                    raise ValueError(f"⚠️  Warning: Record with >>> {u_field}={record[u_field]} <<< already exists")
-                
-            for i_field in index_fields:
-                if record.get(i_field) is not None and record.get(i_field) == ex_record[i_field]:
-                    raise ValueError(f"⚠️  Warning: Record with the value >>> {record[i_field]} <<< already exists in index field")
-        
+                for i_field in index_fields:
+                    if record.get(i_field) is not None and record.get(i_field) == ex_record[i_field]:
+                        raise ValueError(f"⚠️  Warning: Record with the value >>> {record[i_field]} <<< already exists in index field")
+        except Exception as e:
+            print(e)
+            return
         self._validate_create(record)
         
         existing_ids = [record["__id"] for record in self.data]
         new_id = 1 if not existing_ids else max(existing_ids) + 1
         record["__id"] = new_id
 
         self.data.append(record)
```

### Comparing `RTSDB-1.0/RTSDataBase/exceptions.py` & `RTSDB-1.1/RTSDataBase/exceptions.py`

 * *Files identical despite different names*

### Comparing `RTSDB-1.0/RTSDataBase/typotest.py` & `RTSDB-1.1/RTSDataBase/typotest.py`

 * *Files identical despite different names*

### Comparing `RTSDB-1.0/setup.py` & `RTSDB-1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RTSDB',
-    version='1.0',
+    version='1.1',
     packages=find_packages(),
     description='Create yourself a simple database with this package.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='MIT with required credit to the author.',
-    url='https://github.com/RandomTimeLP/RTS_Simpeldatabase/',
+    url='https://github.com/RandomTimeLP/RTS_DataBase/',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

