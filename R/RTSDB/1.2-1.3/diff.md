# Comparing `tmp/RTSDB-1.2.tar.gz` & `tmp/RTSDB-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RTSDB-1.2.tar", last modified: Mon Apr  1 09:40:01 2024, max compression
+gzip compressed data, was "RTSDB-1.3.tar", last modified: Mon Apr  1 09:42:17 2024, max compression
```

## Comparing `RTSDB-1.2.tar` & `RTSDB-1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 09:40:01.010573 RTSDB-1.2/
--rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTSDB-1.2/LICENCE
--rw-rw-rw-   0        0        0     7014 2024-04-01 09:40:01.010573 RTSDB-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6321 2024-04-01 09:19:36.000000 RTSDB-1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 09:40:01.007553 RTSDB-1.2/RTSDB.egg-info/
--rw-rw-rw-   0        0        0     7014 2024-04-01 09:40:00.000000 RTSDB-1.2/RTSDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-04-01 09:40:00.000000 RTSDB-1.2/RTSDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 09:40:00.000000 RTSDB-1.2/RTSDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-01 09:40:00.000000 RTSDB-1.2/RTSDB.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-01 09:40:01.010067 RTSDB-1.2/RTSDataBase/
--rw-rw-rw-   0        0        0    11975 2024-04-01 09:39:49.000000 RTSDB-1.2/RTSDataBase/RTSDB.py
--rw-rw-rw-   0        0        0       21 2024-04-01 08:52:47.000000 RTSDB-1.2/RTSDataBase/__init__.py
--rw-rw-rw-   0        0        0      600 2024-03-31 19:14:15.000000 RTSDB-1.2/RTSDataBase/exceptions.py
--rw-rw-rw-   0        0        0      569 2024-03-31 15:51:44.000000 RTSDB-1.2/RTSDataBase/typotest.py
--rw-rw-rw-   0        0        0       42 2024-04-01 09:40:01.010573 RTSDB-1.2/setup.cfg
--rw-rw-rw-   0        0        0      861 2024-04-01 09:39:59.000000 RTSDB-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:42:17.683014 RTSDB-1.3/
+-rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTSDB-1.3/LICENCE
+-rw-rw-rw-   0        0        0     7014 2024-04-01 09:42:17.682512 RTSDB-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6321 2024-04-01 09:19:36.000000 RTSDB-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 09:42:17.679495 RTSDB-1.3/RTSDB.egg-info/
+-rw-rw-rw-   0        0        0     7014 2024-04-01 09:42:17.000000 RTSDB-1.3/RTSDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-04-01 09:42:17.000000 RTSDB-1.3/RTSDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 09:42:17.000000 RTSDB-1.3/RTSDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-01 09:42:17.000000 RTSDB-1.3/RTSDB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 09:42:17.682008 RTSDB-1.3/RTSDataBase/
+-rw-rw-rw-   0        0        0    12011 2024-04-01 09:41:59.000000 RTSDB-1.3/RTSDataBase/RTSDB.py
+-rw-rw-rw-   0        0        0       21 2024-04-01 08:52:47.000000 RTSDB-1.3/RTSDataBase/__init__.py
+-rw-rw-rw-   0        0        0      600 2024-03-31 19:14:15.000000 RTSDB-1.3/RTSDataBase/exceptions.py
+-rw-rw-rw-   0        0        0      569 2024-03-31 15:51:44.000000 RTSDB-1.3/RTSDataBase/typotest.py
+-rw-rw-rw-   0        0        0       42 2024-04-01 09:42:17.683014 RTSDB-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      861 2024-04-01 09:42:04.000000 RTSDB-1.3/setup.py
```

### Comparing `RTSDB-1.2/LICENCE` & `RTSDB-1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `RTSDB-1.2/PKG-INFO` & `RTSDB-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTSDB
-Version: 1.2
+Version: 1.3
 Summary: Create yourself a simple database with this package.
 Home-page: https://github.com/RandomTimeLP/RTS_DataBase/
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: database
 Platform: UNKNOWN
```

### Comparing `RTSDB-1.2/README.md` & `RTSDB-1.3/README.md`

 * *Files identical despite different names*

### Comparing `RTSDB-1.2/RTSDB.egg-info/PKG-INFO` & `RTSDB-1.3/RTSDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTSDB
-Version: 1.2
+Version: 1.3
 Summary: Create yourself a simple database with this package.
 Home-page: https://github.com/RandomTimeLP/RTS_DataBase/
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: database
 Platform: UNKNOWN
```

### Comparing `RTSDB-1.2/RTSDataBase/RTSDB.py` & `RTSDB-1.3/RTSDataBase/RTSDB.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,19 +109,19 @@
         
         unique_fields = [field for field, state in zip(self.header["fields"], self.header["states"]) if state in  ["unique", "ul"]]
         index_fields = [field for field, state in zip(self.header["fields"], self.header["states"]) if state == "index"]
         try:
             for ex_record in self.data:
                 for u_field in unique_fields:
                     if record.get(u_field) is not None and record.get(u_field) == ex_record[u_field]:
-                        raise ValueError(f"⚠️  Warning: Record with >>> {u_field}={record[u_field]} <<< already exists in: {self.filename}")
+                        raise ValueError(f"⚠️  Warning: Record with >>> {u_field}={record[u_field]} <<< already exists in the database file: {self.filename}")
 
                 for i_field in index_fields:
                     if record.get(i_field) is not None and record.get(i_field) == ex_record[i_field]:
-                        raise ValueError(f"⚠️  Warning: Record with the value >>> {record[i_field]} <<< already exists in index field in: {self.filename}")
+                        raise ValueError(f"⚠️  Warning: Record with the value >>> {record[i_field]} <<< already exists in index field in the database file: {self.filename}")
         except Exception as e:
             print(e)
             return
         self._validate_create(record)
         
         existing_ids = [record["__id"] for record in self.data]
         new_id = 1 if not existing_ids else max(existing_ids) + 1
```

### Comparing `RTSDB-1.2/RTSDataBase/exceptions.py` & `RTSDB-1.3/RTSDataBase/exceptions.py`

 * *Files identical despite different names*

### Comparing `RTSDB-1.2/RTSDataBase/typotest.py` & `RTSDB-1.3/RTSDataBase/typotest.py`

 * *Files identical despite different names*

### Comparing `RTSDB-1.2/setup.py` & `RTSDB-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RTSDB',
-    version='1.2',
+    version='1.3',
     packages=find_packages(),
     description='Create yourself a simple database with this package.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='MIT with required credit to the author.',
```

