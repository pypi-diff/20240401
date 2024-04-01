# Comparing `tmp/RTSDB-1.3.tar.gz` & `tmp/RTSDB-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RTSDB-1.3.tar", last modified: Mon Apr  1 09:42:17 2024, max compression
+gzip compressed data, was "RTSDB-1.4.tar", last modified: Mon Apr  1 12:52:36 2024, max compression
```

## Comparing `RTSDB-1.3.tar` & `RTSDB-1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 09:42:17.683014 RTSDB-1.3/
--rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTSDB-1.3/LICENCE
--rw-rw-rw-   0        0        0     7014 2024-04-01 09:42:17.682512 RTSDB-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6321 2024-04-01 09:19:36.000000 RTSDB-1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 09:42:17.679495 RTSDB-1.3/RTSDB.egg-info/
--rw-rw-rw-   0        0        0     7014 2024-04-01 09:42:17.000000 RTSDB-1.3/RTSDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-04-01 09:42:17.000000 RTSDB-1.3/RTSDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 09:42:17.000000 RTSDB-1.3/RTSDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-01 09:42:17.000000 RTSDB-1.3/RTSDB.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-01 09:42:17.682008 RTSDB-1.3/RTSDataBase/
--rw-rw-rw-   0        0        0    12011 2024-04-01 09:41:59.000000 RTSDB-1.3/RTSDataBase/RTSDB.py
--rw-rw-rw-   0        0        0       21 2024-04-01 08:52:47.000000 RTSDB-1.3/RTSDataBase/__init__.py
--rw-rw-rw-   0        0        0      600 2024-03-31 19:14:15.000000 RTSDB-1.3/RTSDataBase/exceptions.py
--rw-rw-rw-   0        0        0      569 2024-03-31 15:51:44.000000 RTSDB-1.3/RTSDataBase/typotest.py
--rw-rw-rw-   0        0        0       42 2024-04-01 09:42:17.683014 RTSDB-1.3/setup.cfg
--rw-rw-rw-   0        0        0      861 2024-04-01 09:42:04.000000 RTSDB-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:52:36.946221 RTSDB-1.4/
+-rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTSDB-1.4/LICENCE
+-rw-rw-rw-   0        0        0     7014 2024-04-01 12:52:36.945720 RTSDB-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6321 2024-04-01 09:45:01.000000 RTSDB-1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 12:52:36.943198 RTSDB-1.4/RTSDB.egg-info/
+-rw-rw-rw-   0        0        0     7014 2024-04-01 12:52:36.000000 RTSDB-1.4/RTSDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-04-01 12:52:36.000000 RTSDB-1.4/RTSDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 12:52:36.000000 RTSDB-1.4/RTSDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-01 12:52:36.000000 RTSDB-1.4/RTSDB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 12:52:36.945220 RTSDB-1.4/RTSDataBase/
+-rw-rw-rw-   0        0        0    12012 2024-04-01 12:51:50.000000 RTSDB-1.4/RTSDataBase/RTSDB.py
+-rw-rw-rw-   0        0        0       21 2024-04-01 08:52:47.000000 RTSDB-1.4/RTSDataBase/__init__.py
+-rw-rw-rw-   0        0        0      600 2024-03-31 19:14:15.000000 RTSDB-1.4/RTSDataBase/exceptions.py
+-rw-rw-rw-   0        0        0      569 2024-03-31 15:51:44.000000 RTSDB-1.4/RTSDataBase/typotest.py
+-rw-rw-rw-   0        0        0       42 2024-04-01 12:52:36.946221 RTSDB-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      861 2024-04-01 12:52:30.000000 RTSDB-1.4/setup.py
```

### Comparing `RTSDB-1.3/LICENCE` & `RTSDB-1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `RTSDB-1.3/PKG-INFO` & `RTSDB-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTSDB
-Version: 1.3
+Version: 1.4
 Summary: Create yourself a simple database with this package.
 Home-page: https://github.com/RandomTimeLP/RTS_DataBase/
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: database
 Platform: UNKNOWN
```

### Comparing `RTSDB-1.3/README.md` & `RTSDB-1.4/README.md`

 * *Files identical despite different names*

### Comparing `RTSDB-1.3/RTSDB.egg-info/PKG-INFO` & `RTSDB-1.4/RTSDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTSDB
-Version: 1.3
+Version: 1.4
 Summary: Create yourself a simple database with this package.
 Home-page: https://github.com/RandomTimeLP/RTS_DataBase/
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: database
 Platform: UNKNOWN
```

### Comparing `RTSDB-1.3/RTSDataBase/RTSDB.py` & `RTSDB-1.4/RTSDataBase/RTSDB.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
     # See **Delete a record** in the README.md
     def delete(self, id):
         self.data = [record for record in self.data if record.get('__id') != id]
         self._save()
 
     # See **Search records** in the README.md
     def find(self, query, fieldname="__any", case_sensitive=True, allow_typo=False):
-        print("Finding > Query: ",query, "Fieldname: ",fieldname, "Case sensitiv: ",case_sensitive, "Allow typo: ",allow_typo)
+        #print("Finding > Query: ",query, "Fieldname: ",fieldname, "Case sensitiv: ",case_sensitive, "Allow typo: ",allow_typo)
         matches = []
         for record in self.data:
             # fieldname = "__any" means that the query will be searched in all fields except "__id"
             # if fieldname is not "__any" the query will be searched in the specified field except "__id"
             if fieldname == "__any":
                 fields = [field for field in record if field != "__id"]
             elif fieldname == "__id":
```

### Comparing `RTSDB-1.3/RTSDataBase/exceptions.py` & `RTSDB-1.4/RTSDataBase/exceptions.py`

 * *Files identical despite different names*

### Comparing `RTSDB-1.3/RTSDataBase/typotest.py` & `RTSDB-1.4/RTSDataBase/typotest.py`

 * *Files identical despite different names*

### Comparing `RTSDB-1.3/setup.py` & `RTSDB-1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RTSDB',
-    version='1.3',
+    version='1.4',
     packages=find_packages(),
     description='Create yourself a simple database with this package.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='MIT with required credit to the author.',
```

