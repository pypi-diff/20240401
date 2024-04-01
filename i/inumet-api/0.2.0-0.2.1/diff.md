# Comparing `tmp/inumet_api-0.2.0.tar.gz` & `tmp/inumet_api-0.2.1.tar.gz`

## Comparing `inumet_api-0.2.0.tar` & `inumet_api-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 inumet_api-0.2.0/src/inumet_api/__init__.py
--rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 inumet_api-0.2.0/src/inumet_api/api.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 inumet_api-0.2.0/.gitignore
--rw-r--r--   0        0        0    18431 2020-02-02 00:00:00.000000 inumet_api-0.2.0/LICENSE
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 inumet_api-0.2.0/README.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 inumet_api-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 inumet_api-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 inumet_api-0.2.1/src/inumet_api/__init__.py
+-rw-r--r--   0        0        0     9873 2020-02-02 00:00:00.000000 inumet_api-0.2.1/src/inumet_api/api.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 inumet_api-0.2.1/.gitignore
+-rw-r--r--   0        0        0    18431 2020-02-02 00:00:00.000000 inumet_api-0.2.1/LICENSE
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 inumet_api-0.2.1/README.md
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 inumet_api-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 inumet_api-0.2.1/PKG-INFO
```

### Comparing `inumet_api-0.2.0/src/inumet_api/api.py` & `inumet_api-0.2.1/src/inumet_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
             station = stationsCoords.query([(lat,long)])
             if int(station[0]) < 60:
                 self.station = self.estaciones()[int(station[1])].get('id')
             else:
                 stationsCoords = spatial.KDTree(all_sts)
                 station = stationsCoords.query([(lat,long)])
                 self.station = self.estaciones()[int(station[1])].get('id')
+            self.stationName = self.estaciones()[int(station[1])].get('NombreEstacion')
             zonesCoords = spatial.KDTree([(x.get('latitud'),x.get('longitud')) for x in self.zonas()])
             zone = zonesCoords.query([(lat,long)])
             self.zone = self.zonas()[int(zone[1])].get('idInt')
         else:
             if station != "":
                 self.station = [x['id'] for x in self.estaciones() if x['NombreEstacion'] == station][0]
             if depto != "":
```

### Comparing `inumet_api-0.2.0/.gitignore` & `inumet_api-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `inumet_api-0.2.0/LICENSE` & `inumet_api-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inumet_api-0.2.0/README.md` & `inumet_api-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `inumet_api-0.2.0/pyproject.toml` & `inumet_api-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "inumet_api"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Aron Kahrs", email="aronkahrs.us@gmail.com" },
 ]
 description = "INUMET Api wrapper for python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `inumet_api-0.2.0/PKG-INFO` & `inumet_api-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: inumet_api
-Version: 0.2.0
+Version: 0.2.1
 Summary: INUMET Api wrapper for python
 Project-URL: Homepage, https://github.com/aronkahrs-us/inumet-api
 Project-URL: Issues, https://github.com/aronkahrs-us/inumet-api/issues
 Author-email: Aron Kahrs <aronkahrs.us@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

