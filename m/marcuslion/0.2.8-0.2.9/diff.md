# Comparing `tmp/marcuslion-0.2.8.tar.gz` & `tmp/marcuslion-0.2.9.tar.gz`

## Comparing `marcuslion-0.2.8.tar` & `marcuslion-0.2.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 marcuslion-0.2.8/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 marcuslion-0.2.8/.idea/misc.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 marcuslion-0.2.8/.idea/ml-lib-python.iml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 marcuslion-0.2.8/.idea/modules.xml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 marcuslion-0.2.8/.idea/vcs.xml
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 marcuslion-0.2.8/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 marcuslion-0.2.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 marcuslion-0.2.8/src/marcuslion/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 marcuslion-0.2.8/src/marcuslion/marcuslion.py
--rw-r--r--   0        0        0    31684 2020-02-02 00:00:00.000000 marcuslion-0.2.8/src/marcuslion/resources/marcus_lion_logo.jpg
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 marcuslion-0.2.8/tests/ml_lib_test.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 marcuslion-0.2.8/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 marcuslion-0.2.8/LICENSE
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 marcuslion-0.2.8/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 marcuslion-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 marcuslion-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 marcuslion-0.2.9/.idea/.gitignore
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 marcuslion-0.2.9/.idea/misc.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 marcuslion-0.2.9/.idea/ml-lib-python.iml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 marcuslion-0.2.9/.idea/modules.xml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 marcuslion-0.2.9/.idea/vcs.xml
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 marcuslion-0.2.9/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 marcuslion-0.2.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 marcuslion-0.2.9/src/marcuslion/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 marcuslion-0.2.9/src/marcuslion/marcuslion.py
+-rw-r--r--   0        0        0    31684 2020-02-02 00:00:00.000000 marcuslion-0.2.9/src/marcuslion/resources/marcus_lion_logo.jpg
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 marcuslion-0.2.9/tests/ml_lib_test.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 marcuslion-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 marcuslion-0.2.9/LICENSE
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 marcuslion-0.2.9/README.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 marcuslion-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 marcuslion-0.2.9/PKG-INFO
```

### Comparing `marcuslion-0.2.8/.idea/workspace.xml` & `marcuslion-0.2.9/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `marcuslion-0.2.8/src/marcuslion/__init__.py` & `marcuslion-0.2.9/src/marcuslion/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
 import pandas as pd
 import urllib3
 import ssl
 import io
-from skimage import io
+from skimage import io as skio
 import os.path
 
 logger = logging.getLogger()
 # logger.setLevel(logging.DEBUG)
 logger.addHandler(logging.StreamHandler())
 
 logger.info("Start marcuslion lib")
 resource_path = os.path.join(os.path.split(__file__)[0], "resources")
-image = io.imread(resource_path + "/marcus_lion_logo.jpg")
-io.imshow(image)
+image = skio.imread(resource_path + "/marcus_lion_logo.jpg")
+skio.imshow(image)
 
 pd.set_option('display.max_rows', 500)
 pd.set_option('display.max_columns', 500)
 pd.set_option('display.width', 2000)
 
 
 def ml_addone(number):
```

### Comparing `marcuslion-0.2.8/src/marcuslion/resources/marcus_lion_logo.jpg` & `marcuslion-0.2.9/src/marcuslion/resources/marcus_lion_logo.jpg`

 * *Files identical despite different names*

### Comparing `marcuslion-0.2.8/.gitignore` & `marcuslion-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `marcuslion-0.2.8/LICENSE` & `marcuslion-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `marcuslion-0.2.8/README.md` & `marcuslion-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `marcuslion-0.2.8/pyproject.toml` & `marcuslion-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "marcuslion"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="Marc", email="support@marcuslion.com" },
 ]
 description = "Marcus Lion Python library package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `marcuslion-0.2.8/PKG-INFO` & `marcuslion-0.2.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marcuslion
-Version: 0.2.8
+Version: 0.2.9
 Summary: Marcus Lion Python library package
 Project-URL: Homepage, https://github.com/Marcus-Lion/ml-lib-python.git
 Project-URL: Bug Tracker, https://github.com/Marcus-Lion/ml-lib-python.git/issues
 Author-email: Marc <support@marcuslion.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

