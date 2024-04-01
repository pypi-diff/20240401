# Comparing `tmp/TimeFeatures-1.0.8.tar.gz` & `tmp/TimeFeatures-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimeFeatures-1.0.8.tar", last modified: Sat Feb 24 17:35:06 2024, max compression
+gzip compressed data, was "TimeFeatures-1.0.9.tar", last modified: Mon Feb 26 18:59:23 2024, max compression
```

## Comparing `TimeFeatures-1.0.8.tar` & `TimeFeatures-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-02-24 17:35:06.254248 TimeFeatures-1.0.8/
--rw-rw-rw-   0        0        0    35149 2024-02-23 01:30:50.000000 TimeFeatures-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     2671 2024-02-24 17:35:06.254248 TimeFeatures-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1736 2024-02-23 03:49:26.000000 TimeFeatures-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-02-24 17:35:06.252721 TimeFeatures-1.0.8/TimeFeatures.egg-info/
--rw-rw-rw-   0        0        0     2671 2024-02-24 17:35:06.000000 TimeFeatures-1.0.8/TimeFeatures.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      556 2024-02-24 17:35:06.000000 TimeFeatures-1.0.8/TimeFeatures.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-24 17:35:06.000000 TimeFeatures-1.0.8/TimeFeatures.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-02-24 17:35:06.000000 TimeFeatures-1.0.8/TimeFeatures.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2024-02-24 17:35:06.000000 TimeFeatures-1.0.8/TimeFeatures.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-02-24 17:35:06.259859 TimeFeatures-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1363 2024-02-24 17:34:11.000000 TimeFeatures-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-24 17:35:06.221583 TimeFeatures-1.0.8/timefeatures/
-drwxrwxrwx   0        0        0        0 2024-02-24 17:35:06.244015 TimeFeatures-1.0.8/timefeatures/widgets/
--rw-rw-rw-   0        0        0      110 2024-02-07 23:22:42.000000 TimeFeatures-1.0.8/timefeatures/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-24 17:35:06.251197 TimeFeatures-1.0.8/timefeatures/widgets/icons/
--rw-rw-rw-   0        0        0      573 2023-09-29 18:46:52.000000 TimeFeatures-1.0.8/timefeatures/widgets/icons/graphgenerator.svg
--rw-rw-rw-   0        0        0      666 2023-09-29 18:47:16.000000 TimeFeatures-1.0.8/timefeatures/widgets/icons/savedatadb.svg
--rw-rw-rw-   0        0        0      782 2024-02-06 01:51:26.000000 TimeFeatures-1.0.8/timefeatures/widgets/icons/timefeature-xs.svg
--rw-rw-rw-   0        0        0      759 2023-09-29 14:24:41.000000 TimeFeatures-1.0.8/timefeatures/widgets/icons/timefeature.svg
--rw-rw-rw-   0        0        0    10884 2024-02-24 14:31:48.000000 TimeFeatures-1.0.8/timefeatures/widgets/owsavetodb.py
--rw-rw-rw-   0        0        0     5607 2024-02-24 17:31:58.000000 TimeFeatures-1.0.8/timefeatures/widgets/owtfgraphgenerator.py
--rw-rw-rw-   0        0        0    67683 2024-02-24 17:23:01.000000 TimeFeatures-1.0.8/timefeatures/widgets/owtimefeatureconstructor.py
+drwxrwxrwx   0        0        0        0 2024-02-26 18:59:23.511297 TimeFeatures-1.0.9/
+-rw-rw-rw-   0        0        0    35149 2024-02-23 01:30:50.000000 TimeFeatures-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2671 2024-02-26 18:59:23.511297 TimeFeatures-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1736 2024-02-23 03:49:26.000000 TimeFeatures-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-02-26 18:59:23.509329 TimeFeatures-1.0.9/TimeFeatures.egg-info/
+-rw-rw-rw-   0        0        0     2671 2024-02-26 18:59:23.000000 TimeFeatures-1.0.9/TimeFeatures.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2024-02-26 18:59:23.000000 TimeFeatures-1.0.9/TimeFeatures.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-26 18:59:23.000000 TimeFeatures-1.0.9/TimeFeatures.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-02-26 18:59:23.000000 TimeFeatures-1.0.9/TimeFeatures.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2024-02-26 18:59:23.000000 TimeFeatures-1.0.9/TimeFeatures.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-02-26 18:59:23.517280 TimeFeatures-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1363 2024-02-26 18:58:38.000000 TimeFeatures-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-26 18:59:23.455122 TimeFeatures-1.0.9/timefeatures/
+drwxrwxrwx   0        0        0        0 2024-02-26 18:59:23.500908 TimeFeatures-1.0.9/timefeatures/widgets/
+-rw-rw-rw-   0        0        0      110 2024-02-07 23:22:42.000000 TimeFeatures-1.0.9/timefeatures/widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-26 18:59:23.507327 TimeFeatures-1.0.9/timefeatures/widgets/icons/
+-rw-rw-rw-   0        0        0      573 2023-09-29 18:46:52.000000 TimeFeatures-1.0.9/timefeatures/widgets/icons/graphgenerator.svg
+-rw-rw-rw-   0        0        0      666 2023-09-29 18:47:16.000000 TimeFeatures-1.0.9/timefeatures/widgets/icons/savedatadb.svg
+-rw-rw-rw-   0        0        0      782 2024-02-06 01:51:26.000000 TimeFeatures-1.0.9/timefeatures/widgets/icons/timefeature-xs.svg
+-rw-rw-rw-   0        0        0      759 2023-09-29 14:24:41.000000 TimeFeatures-1.0.9/timefeatures/widgets/icons/timefeature.svg
+-rw-rw-rw-   0        0        0    11440 2024-02-26 18:54:44.000000 TimeFeatures-1.0.9/timefeatures/widgets/owsavetodb.py
+-rw-rw-rw-   0        0        0     5607 2024-02-24 17:31:58.000000 TimeFeatures-1.0.9/timefeatures/widgets/owtfgraphgenerator.py
+-rw-rw-rw-   0        0        0    67683 2024-02-26 18:51:02.000000 TimeFeatures-1.0.9/timefeatures/widgets/owtimefeatureconstructor.py
```

### Comparing `TimeFeatures-1.0.8/LICENSE` & `TimeFeatures-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `TimeFeatures-1.0.8/PKG-INFO` & `TimeFeatures-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeFeatures
-Version: 1.0.8
+Version: 1.0.9
 Summary: Timefeatures add-on for Orange 3 data mining software.
 Home-page: https://github.com/alervgr/Orange-TimeFeatures
 Author: Alejandro Rivas García
 Author-email: alejandrorivasgarcia@gmail.com
 License: GPL3+
 Keywords: orange3 add-on,timefeatures,graph,time series,data mining,graph visualization,orange,addon,synthetic data
 Classifier: Development Status :: 4 - Beta
```

### Comparing `TimeFeatures-1.0.8/README.md` & `TimeFeatures-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `TimeFeatures-1.0.8/TimeFeatures.egg-info/PKG-INFO` & `TimeFeatures-1.0.9/TimeFeatures.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeFeatures
-Version: 1.0.8
+Version: 1.0.9
 Summary: Timefeatures add-on for Orange 3 data mining software.
 Home-page: https://github.com/alervgr/Orange-TimeFeatures
 Author: Alejandro Rivas García
 Author-email: alejandrorivasgarcia@gmail.com
 License: GPL3+
 Keywords: orange3 add-on,timefeatures,graph,time series,data mining,graph visualization,orange,addon,synthetic data
 Classifier: Development Status :: 4 - Beta
```

### Comparing `TimeFeatures-1.0.8/TimeFeatures.egg-info/SOURCES.txt` & `TimeFeatures-1.0.9/TimeFeatures.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TimeFeatures-1.0.8/setup.py` & `TimeFeatures-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]    
 
 
 setup(name="TimeFeatures",
       packages=["timefeatures.widgets"],
       package_data={"timefeatures.widgets": ["icons/*.svg", "icons/*.png"]},
       entry_points={"orange.widgets": "Time-Features = timefeatures.widgets"},
-      version="1.0.8",
+      version="1.0.9",
       author="Alejandro Rivas García",
       author_email="alejandrorivasgarcia@gmail.com",
       keywords=[
     'orange3 add-on','timefeatures','graph','time series','data mining','graph visualization','orange','addon', 'synthetic data'
 ],
       url="https://github.com/alervgr/Orange-TimeFeatures",
       license="GPL3+",
```

### Comparing `TimeFeatures-1.0.8/timefeatures/widgets/icons/graphgenerator.svg` & `TimeFeatures-1.0.9/timefeatures/widgets/icons/graphgenerator.svg`

 * *Files identical despite different names*

### Comparing `TimeFeatures-1.0.8/timefeatures/widgets/icons/savedatadb.svg` & `TimeFeatures-1.0.9/timefeatures/widgets/icons/savedatadb.svg`

 * *Files identical despite different names*

### Comparing `TimeFeatures-1.0.8/timefeatures/widgets/icons/timefeature-xs.svg` & `TimeFeatures-1.0.9/timefeatures/widgets/icons/timefeature-xs.svg`

 * *Files identical despite different names*

### Comparing `TimeFeatures-1.0.8/timefeatures/widgets/icons/timefeature.svg` & `TimeFeatures-1.0.9/timefeatures/widgets/icons/timefeature.svg`

 * *Files identical despite different names*

### Comparing `TimeFeatures-1.0.8/timefeatures/widgets/owsavetodb.py` & `TimeFeatures-1.0.9/timefeatures/widgets/owsavetodb.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from Orange.data.sql.table import SqlTable, LARGE_TABLE, AUTO_DL_LIMIT
 from Orange.widgets import gui
 from Orange.widgets.settings import Setting
 from Orange.widgets.utils.itemmodels import PyListModel
 from Orange.widgets.utils.owbasesql import OWBaseSql
 from Orange.widgets.utils.sql import check_sql_input
 from Orange.widgets.utils.widgetpreview import WidgetPreview
-from Orange.widgets.widget import Msg
+from Orange.widgets.widget import Msg, OWWidget
 from PyQt5.QtGui import QPixmap, QStandardItem
 from PyQt5.QtWidgets import QGridLayout, QLineEdit, QPushButton, QSizePolicy, QLabel
 from orangewidget.utils.signals import Input
 
 MAX_DL_LIMIT = 1000000
 
 
@@ -38,15 +38,15 @@
     def data(self, index, role=Qt.DisplayRole):
         row = index.row()
         if role == Qt.DisplayRole:
             return self[row].display_name
         return super().data(index, role)
 
 
-class owsavetodb(OWBaseSql):
+class owsavetodb(OWBaseSql, OWWidget):
     name = "Save to DB"
     description = "Save a dataset into a DB."
     icon = "icons/savedatadb.svg"
     priority = 2240
     keywords = "sql table, save, data, db, dataset"
 
     class Inputs:
@@ -135,14 +135,15 @@
             placeholderText="Table name...", toolTip="Table name")
         layoutA.addWidget(self.tableName, 3, 0)
         self.btn_savedata = QPushButton(
             "Save", toolTip="Save a dataset into a DB",
             minimumWidth=120
         )
         self.btn_savedata.clicked.connect(self.saveData)
+        self.btn_savedata.setEnabled(False)
         layoutA.addWidget(self.btn_savedata, 3, 2)
         self._add_backend_controls()
 
     def _add_backend_controls(self):
         box = self.serverbox
         self.backends = BackendModel(Backend.available_backends())
         self.backendcombo = QComboBox(box)
@@ -175,14 +176,15 @@
             with self.backend.execute_sql_query(query):
                 pass
         except BackendError as ex:
             self.Error.connection(str(ex))
 
     def create_table(self, table_name):
 
+        contBar = 0
         contMetasOriginales = 0
         cont = 0
         variables = []
         tiene_class = 0
 
         if self.data.domain.class_var:
             variables.append(self.data.domain.class_var)
@@ -220,29 +222,43 @@
 
         insert_query = f"INSERT INTO {table_name} VALUES ("
         for i in range(len(variables)):
             insert_query += "%s,"
         insert_query = insert_query[:-1]  # Eliminar la coma final
         insert_query += ")"
 
+        self.progressBarInit()
+
         for instance in self.data:
             data_row = []
+            contBar += 1
+
+            if contBar*4 == len(self.data):
+                self.progressBarSet(25)
+            elif contBar*2 == len(self.data):
+                self.progressBarSet(50)
+            elif contBar == len(self.data)-(len(self.data)/4):
+                self.progressBarSet(75)
+            elif contBar == len(self.data):
+                self.progressBarSet(100)
+
             for i in range(len(variables)):
                 if cont > 0:
                     i -= cont
                 data_row.append(instance[i].value)
             if self.data.domain.class_var:
                 class_value = data_row[-1]  # Obtiene el valor de la clase
                 del data_row[-1]  # Elimina la clase de su posición anterior
                 data_row.insert(0, class_value)  # Inserta la clase al principio de la lista
             try:
                 with self.backend.execute_sql_query(insert_query, params=data_row):
                     pass
             except BackendError as ex:
                 self.Error.connection(str(ex))
+            self.progressBarFinished()
 
     def saveData(self):
 
         self.clear()
 
         if self.tableName.text() == "":
             self.Error.connection("Table name must be filled.")
```

### Comparing `TimeFeatures-1.0.8/timefeatures/widgets/owtfgraphgenerator.py` & `TimeFeatures-1.0.9/timefeatures/widgets/owtfgraphgenerator.py`

 * *Files identical despite different names*

### Comparing `TimeFeatures-1.0.8/timefeatures/widgets/owtimefeatureconstructor.py` & `TimeFeatures-1.0.9/timefeatures/widgets/owtimefeatureconstructor.py`

 * *Files identical despite different names*

