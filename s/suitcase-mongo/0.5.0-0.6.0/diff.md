# Comparing `tmp/suitcase-mongo-0.5.0.tar.gz` & `tmp/suitcase-mongo-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suitcase-mongo-0.5.0.tar", last modified: Tue Feb  6 18:31:13 2024, max compression
+gzip compressed data, was "suitcase-mongo-0.6.0.tar", last modified: Mon Apr  1 16:19:17 2024, max compression
```

## Comparing `suitcase-mongo-0.5.0.tar` & `suitcase-mongo-0.6.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-02-06 18:31:13.836199 suitcase-mongo-0.5.0/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1584 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/LICENSE
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      376 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/MANIFEST.in
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1079 2024-02-06 18:31:13.836199 suitcase-mongo-0.5.0/PKG-INFO
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      796 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/README.md
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-02-06 18:31:13.832199 suitcase-mongo-0.5.0/docs/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      673 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/docs/Makefile
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      797 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/docs/make.bat
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-02-06 18:31:13.832199 suitcase-mongo-0.5.0/docs/source/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6305 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/docs/source/conf.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      371 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/docs/source/index.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       96 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/docs/source/installation.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      266 2024-02-05 21:56:26.000000 suitcase-mongo-0.5.0/docs/source/release-history.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      109 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/docs/source/usage.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       84 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/requirements.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      214 2024-02-06 18:31:13.836199 suitcase-mongo-0.5.0/setup.cfg
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2257 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/setup.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-02-06 18:31:13.828199 suitcase-mongo-0.5.0/suitcase/
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-02-06 18:31:13.832199 suitcase-mongo-0.5.0/suitcase/mongo_embedded/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    22994 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/suitcase/mongo_embedded/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    18470 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/suitcase/mongo_embedded/_version.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       90 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/suitcase/mongo_embedded/conftest.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-02-06 18:31:13.832199 suitcase-mongo-0.5.0/suitcase/mongo_embedded/tests/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/suitcase/mongo_embedded/tests/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      254 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/suitcase/mongo_embedded/tests/conftest.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      615 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/suitcase/mongo_embedded/tests/fixtures.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7787 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/suitcase/mongo_embedded/tests/tests.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-02-06 18:31:13.836199 suitcase-mongo-0.5.0/suitcase/mongo_normalized/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    13203 2024-02-05 21:56:30.000000 suitcase-mongo-0.5.0/suitcase/mongo_normalized/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      497 2024-02-06 18:31:13.836199 suitcase-mongo-0.5.0/suitcase/mongo_normalized/_version.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-02-06 18:31:13.836199 suitcase-mongo-0.5.0/suitcase/mongo_normalized/tests/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/suitcase/mongo_normalized/tests/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      254 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/suitcase/mongo_normalized/tests/conftest.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      619 2024-02-02 20:33:39.000000 suitcase-mongo-0.5.0/suitcase/mongo_normalized/tests/fixtures.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7696 2024-02-05 21:56:30.000000 suitcase-mongo-0.5.0/suitcase/mongo_normalized/tests/tests.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-02-06 18:31:13.836199 suitcase-mongo-0.5.0/suitcase_mongo.egg-info/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1079 2024-02-06 18:31:13.000000 suitcase-mongo-0.5.0/suitcase_mongo.egg-info/PKG-INFO
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      943 2024-02-06 18:31:13.000000 suitcase-mongo-0.5.0/suitcase_mongo.egg-info/SOURCES.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        1 2024-02-06 18:31:13.000000 suitcase-mongo-0.5.0/suitcase_mongo.egg-info/dependency_links.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       30 2024-02-06 18:31:13.000000 suitcase-mongo-0.5.0/suitcase_mongo.egg-info/requires.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        9 2024-02-06 18:31:13.000000 suitcase-mongo-0.5.0/suitcase_mongo.egg-info/top_level.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    68573 2024-02-05 21:56:26.000000 suitcase-mongo-0.5.0/versioneer.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-04-01 16:19:17.579128 suitcase-mongo-0.6.0/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1584 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/LICENSE
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      376 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/MANIFEST.in
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1079 2024-04-01 16:19:17.579128 suitcase-mongo-0.6.0/PKG-INFO
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      796 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/README.md
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-04-01 16:19:17.579128 suitcase-mongo-0.6.0/docs/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      673 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/docs/Makefile
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      797 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/docs/make.bat
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-04-01 16:19:17.579128 suitcase-mongo-0.6.0/docs/source/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6305 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/docs/source/conf.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      371 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/docs/source/index.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       96 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/docs/source/installation.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      266 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/docs/source/release-history.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      109 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/docs/source/usage.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       84 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/requirements.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      214 2024-04-01 16:19:17.579128 suitcase-mongo-0.6.0/setup.cfg
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2257 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/setup.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-04-01 16:19:17.579128 suitcase-mongo-0.6.0/suitcase/
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-04-01 16:19:17.579128 suitcase-mongo-0.6.0/suitcase/mongo_embedded/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    22994 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/suitcase/mongo_embedded/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    18470 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/suitcase/mongo_embedded/_version.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       90 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/suitcase/mongo_embedded/conftest.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-04-01 16:19:17.579128 suitcase-mongo-0.6.0/suitcase/mongo_embedded/tests/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/suitcase/mongo_embedded/tests/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      254 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/suitcase/mongo_embedded/tests/conftest.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      615 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/suitcase/mongo_embedded/tests/fixtures.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7787 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/suitcase/mongo_embedded/tests/tests.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-04-01 16:19:17.579128 suitcase-mongo-0.6.0/suitcase/mongo_normalized/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    13171 2024-04-01 14:20:31.000000 suitcase-mongo-0.6.0/suitcase/mongo_normalized/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      497 2024-04-01 16:19:17.579128 suitcase-mongo-0.6.0/suitcase/mongo_normalized/_version.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-04-01 16:19:17.579128 suitcase-mongo-0.6.0/suitcase/mongo_normalized/tests/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/suitcase/mongo_normalized/tests/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      277 2024-04-01 14:20:31.000000 suitcase-mongo-0.6.0/suitcase/mongo_normalized/tests/conftest.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1147 2024-04-01 14:20:31.000000 suitcase-mongo-0.6.0/suitcase/mongo_normalized/tests/fixtures.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7864 2024-04-01 14:20:31.000000 suitcase-mongo-0.6.0/suitcase/mongo_normalized/tests/tests.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2024-04-01 16:19:17.579128 suitcase-mongo-0.6.0/suitcase_mongo.egg-info/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1079 2024-04-01 16:19:17.000000 suitcase-mongo-0.6.0/suitcase_mongo.egg-info/PKG-INFO
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      943 2024-04-01 16:19:17.000000 suitcase-mongo-0.6.0/suitcase_mongo.egg-info/SOURCES.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        1 2024-04-01 16:19:17.000000 suitcase-mongo-0.6.0/suitcase_mongo.egg-info/dependency_links.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       30 2024-04-01 16:19:17.000000 suitcase-mongo-0.6.0/suitcase_mongo.egg-info/requires.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        9 2024-04-01 16:19:17.000000 suitcase-mongo-0.6.0/suitcase_mongo.egg-info/top_level.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    68573 2023-09-11 16:35:10.000000 suitcase-mongo-0.6.0/versioneer.py
```

### Comparing `suitcase-mongo-0.5.0/LICENSE` & `suitcase-mongo-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `suitcase-mongo-0.5.0/PKG-INFO` & `suitcase-mongo-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suitcase-mongo
-Version: 0.5.0
+Version: 0.6.0
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `suitcase-mongo-0.5.0/README.md` & `suitcase-mongo-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `suitcase-mongo-0.5.0/docs/Makefile` & `suitcase-mongo-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `suitcase-mongo-0.5.0/docs/make.bat` & `suitcase-mongo-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `suitcase-mongo-0.5.0/docs/source/conf.py` & `suitcase-mongo-0.6.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `suitcase-mongo-0.5.0/setup.py` & `suitcase-mongo-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `suitcase-mongo-0.5.0/suitcase/mongo_embedded/__init__.py` & `suitcase-mongo-0.6.0/suitcase/mongo_embedded/__init__.py`

 * *Files identical despite different names*

### Comparing `suitcase-mongo-0.5.0/suitcase/mongo_embedded/_version.py` & `suitcase-mongo-0.6.0/suitcase/mongo_embedded/_version.py`

 * *Files identical despite different names*

### Comparing `suitcase-mongo-0.5.0/suitcase/mongo_embedded/tests/fixtures.py` & `suitcase-mongo-0.6.0/suitcase/mongo_embedded/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `suitcase-mongo-0.5.0/suitcase/mongo_embedded/tests/tests.py` & `suitcase-mongo-0.6.0/suitcase/mongo_embedded/tests/tests.py`

 * *Files identical despite different names*

### Comparing `suitcase-mongo-0.5.0/suitcase/mongo_normalized/__init__.py` & `suitcase-mongo-0.6.0/suitcase/mongo_normalized/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,17 +79,16 @@
             "datum": self._datum_collection,
         }
 
         self._metadatastore_db = mds_db
         self._asset_registry_db = assets_db
         self._ignore_duplicates = ignore_duplicates
         self._resource_uid_unique = resource_uid_unique
-        self._create_indexes()
 
-    def _create_indexes(self):
+    def create_indexes(self):
         """
         Create indexes on the various collections.
 
         If the index already exists, this has no effect.
         """
         self._resource_collection.create_index("uid", unique=self._resource_uid_unique)
         self._resource_collection.create_index("resource_id")  # legacy
```

### Comparing `suitcase-mongo-0.5.0/suitcase/mongo_normalized/tests/tests.py` & `suitcase-mongo-0.6.0/suitcase/mongo_normalized/tests/tests.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 def test_duplicates(db_factory, example_data):
     # Duplicate should not cause exceptions, and should be deduped.
     documents = example_data()
     metadatastore_db = db_factory()
     asset_registry_db = db_factory()
     serializer = Serializer(metadatastore_db, asset_registry_db)
+
     for item in documents:
         serializer(*item)
     for item in documents:
         serializer(*item)
 
     # Modify a document, check that inserting a document with uid,
     # but different content raises.
@@ -164,20 +165,29 @@
 
     indexes = asset_registry_db.datum.index_information()
     assert len(indexes.keys()) == 3
     assert indexes["datum_id_1"]["unique"]
     assert indexes["resource_1"]
 
     indexes = metadatastore_db.run_start.index_information()
-    assert len(indexes.keys()) == 6
+    assert len(indexes.keys()) == 10
+    for index_name in [
+        '_id_',
+        'uid_1',
+        'scan_id_1',
+        'scan_id_-1__id_-1',
+        'time_1__id_-1',
+        'time_-1__id_-1',
+        'time_-1_scan_id_-1',
+        '$**_text',
+        'data_session_1',
+        'data_groups_1',
+    ]:
+        assert index_name in indexes
     assert indexes["uid_1"]["unique"]
-    assert indexes["time_-1_scan_id_-1"]
-    assert indexes["$**_text"]
-    assert indexes["data_session_1"]
-    assert indexes["data_groups_1"]
 
     indexes = metadatastore_db.run_stop.index_information()
     assert len(indexes.keys()) == 5
     assert indexes["uid_1"]["unique"]
     assert indexes["run_start_1"]["unique"]
     assert indexes["time_-1"]
     assert indexes["$**_text"]
@@ -191,16 +201,14 @@
 
     indexes = metadatastore_db.event.index_information()
     assert len(indexes.keys()) == 3
     assert indexes["uid_1"]["unique"]
     assert indexes["descriptor_-1_time_1"]
 
 
-def test_resource_uid_unique(db_factory):
-    db = db_factory()
-    print(type(db))
-    metadatastore_db = db_factory()
-    asset_registry_db = db_factory()
-    Serializer(metadatastore_db, asset_registry_db, resource_uid_unique=True)
+def test_resource_uid_unique(db_factory_no_indexes):
+    metadatastore_db = db_factory_no_indexes()
+    asset_registry_db = db_factory_no_indexes()
+    Serializer(metadatastore_db, asset_registry_db, resource_uid_unique=True).create_indexes()
 
     indexes = asset_registry_db.resource.index_information()
     assert indexes["uid_1"].get("unique")
```

### Comparing `suitcase-mongo-0.5.0/suitcase_mongo.egg-info/PKG-INFO` & `suitcase-mongo-0.6.0/suitcase_mongo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suitcase-mongo
-Version: 0.5.0
+Version: 0.6.0
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `suitcase-mongo-0.5.0/suitcase_mongo.egg-info/SOURCES.txt` & `suitcase-mongo-0.6.0/suitcase_mongo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `suitcase-mongo-0.5.0/versioneer.py` & `suitcase-mongo-0.6.0/versioneer.py`

 * *Files identical despite different names*

