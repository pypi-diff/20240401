# Comparing `tmp/databarge-2.0.1.tar.gz` & `tmp/databarge-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databarge-2.0.1.tar", last modified: Sun Mar 31 16:44:31 2024, max compression
+gzip compressed data, was "databarge-2.0.2.tar", last modified: Mon Apr  1 20:41:32 2024, max compression
```

## Comparing `databarge-2.0.1.tar` & `databarge-2.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 16:44:31.685666 databarge-2.0.1/
--rw-rw-rw-   0        0        0     1092 2024-03-27 12:25:58.000000 databarge-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     4463 2024-03-31 16:44:31.685666 databarge-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3852 2024-03-31 14:33:54.000000 databarge-2.0.1/README.md
--rw-rw-rw-   0        0        0      722 2024-03-31 16:42:51.000000 databarge-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-31 16:44:31.685666 databarge-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      440 2024-03-31 16:42:28.000000 databarge-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:44:31.638891 databarge-2.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-31 16:44:31.670037 databarge-2.0.1/src/databarge/
--rw-rw-rw-   0        0        0      241 2024-03-31 16:40:31.000000 databarge-2.0.1/src/databarge/__init__.py
--rw-rw-rw-   0        0        0     2764 2024-03-31 16:37:11.000000 databarge-2.0.1/src/databarge/connections.py
--rw-rw-rw-   0        0        0     2400 2024-03-31 16:37:55.000000 databarge-2.0.1/src/databarge/dimensions.py
--rw-rw-rw-   0        0        0     3718 2024-03-31 16:37:47.000000 databarge-2.0.1/src/databarge/execution.py
--rw-rw-rw-   0        0        0      371 2024-03-27 12:34:35.000000 databarge-2.0.1/src/databarge/functions.py
--rw-rw-rw-   0        0        0    16064 2024-03-31 16:38:11.000000 databarge-2.0.1/src/databarge/transfers.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:44:31.685666 databarge-2.0.1/src/databarge.egg-info/
--rw-rw-rw-   0        0        0     4463 2024-03-31 16:44:31.000000 databarge-2.0.1/src/databarge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2024-03-31 16:44:31.000000 databarge-2.0.1/src/databarge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 16:44:31.000000 databarge-2.0.1/src/databarge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-03-31 16:44:31.000000 databarge-2.0.1/src/databarge.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 20:41:32.668252 databarge-2.0.2/
+-rw-rw-rw-   0        0        0     1092 2024-03-27 12:25:58.000000 databarge-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4598 2024-04-01 20:41:32.668252 databarge-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4001 2024-04-01 19:38:59.000000 databarge-2.0.2/README.md
+-rw-rw-rw-   0        0        0      708 2024-04-01 20:41:17.000000 databarge-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 20:41:32.668252 databarge-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      426 2024-04-01 20:41:25.000000 databarge-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:41:32.610915 databarge-2.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 20:41:32.668252 databarge-2.0.2/src/databarge/
+-rw-rw-rw-   0        0        0      241 2024-03-31 16:40:31.000000 databarge-2.0.2/src/databarge/__init__.py
+-rw-rw-rw-   0        0        0     2764 2024-03-31 16:37:11.000000 databarge-2.0.2/src/databarge/connections.py
+-rw-rw-rw-   0        0        0     2400 2024-03-31 16:37:55.000000 databarge-2.0.2/src/databarge/dimensions.py
+-rw-rw-rw-   0        0        0     3718 2024-03-31 16:37:47.000000 databarge-2.0.2/src/databarge/execution.py
+-rw-rw-rw-   0        0        0      371 2024-03-27 12:34:35.000000 databarge-2.0.2/src/databarge/functions.py
+-rw-rw-rw-   0        0        0    16160 2024-04-01 19:36:55.000000 databarge-2.0.2/src/databarge/transfers.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:41:32.668252 databarge-2.0.2/src/databarge.egg-info/
+-rw-rw-rw-   0        0        0     4598 2024-04-01 20:41:32.000000 databarge-2.0.2/src/databarge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2024-04-01 20:41:32.000000 databarge-2.0.2/src/databarge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 20:41:32.000000 databarge-2.0.2/src/databarge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-01 20:41:32.000000 databarge-2.0.2/src/databarge.egg-info/top_level.txt
```

### Comparing `databarge-2.0.1/LICENSE` & `databarge-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `databarge-2.0.1/PKG-INFO` & `databarge-2.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,8 @@
-Metadata-Version: 2.1
-Name: databarge
-Version: 2.0.1
-Summary: Simple ETL tools and functions for SQL Server
-Home-page: https://github.com/porteverte/databarge
-Author: Porte Verte
-Author-email: Port Verte <porte_verte@outlook.com>
-Project-URL: Homepage, https://github.com/porteverte/databarge
-Project-URL: Issues, https://github.com/porteverte/databarge/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
+**databarge | simple ETL tools for SQL Server**
 
 <h1>About</h1>
 
 This package includes but is not limited to:
 
 1. A class to create a connection to SQL Server.
 2. A class to transfer data from one SQL Server to another.
@@ -29,20 +15,22 @@
 Key notes:
 
 1. The data is transfered in chunks of 10,000 to optimise memory usage
 2. Enabling logging will produce a file that records each chunk of data transfered.
 
 <h1>Dependencies</h1>
 
-**Required**
+**python 3.8 is required for this package**
+
+**Required Packages**
 
 | Package	| Version	| License						|
 |---------------|---------------|-------------------------------------------------------|
 | pandas	| 1.3.5		| OSI Approved :: BSD License				|
-| SQLAlchemy	| 1.3.5		| MIT License (MIT)					|
+| SQLAlchemy	| 1.4.27		| MIT License (MIT)					|
 
 <h1>Config</h>
 
 <h2>Create and populate a local config_params.ini file</h2>
 
 Windows authentication example:
 
@@ -80,14 +68,16 @@
     
     # make connections
     source_connection = SqlServerConnection('MSSQLSVRA', config_params_path)
     destination_connection = SqlServerConnection('MSSQLSVRB', config_params_path)
    
 <h2>Create an ETL class</h2>
 
+**Positional arguments:**
+
     # define positional etl class variables
     source_sql = r'''SELECT * FROM TESTDB.dbo.tbl_test'''
     destination_database = 'TESTDB'
     destination_table = 'tbl_test'
     
     # define optional etl class variables
     xforms = [
@@ -98,25 +88,25 @@
     dtypes = {'test_text':sqlalchemy.types.NVARCHAR(length=100)}
     # destination_schema = 'someschema'
     
     # create etl class
     etl_1 = Etl(source_sql, destination_database, destination_table, source_connection, destination_connection
         , xforms = xforms
         , dtypes = dtypes
-        # , schema=destination_schema
+        # , destination_schema=destination_schema
         , log_path=log_path)
 
 <h2>Create other ETL classes and put them all in a list</h2>
 
     # create other etl classes as required
     
     # create a list of etl classes
     xfers = [
         etl_1
-        , # etl_2
+        # , etl_2
         ]
 
 <h2>Execute the ETL classes</h2>
 
     # iterate through the etl list and execute the etl classes
     for xf in xfers:
         
@@ -131,8 +121,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `databarge-2.0.1/README.md` & `databarge-2.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: databarge
+Version: 2.0.2
+Summary: Simple ETL tools for SQL Server
+Home-page: https://github.com/porteverte/databarge
+Author: Porte Verte
+Author-email: Port Verte <porte_verte@outlook.com>
+Project-URL: Homepage, https://github.com/porteverte/databarge
+Project-URL: Issues, https://github.com/porteverte/databarge/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+**databarge | simple ETL tools for SQL Server**
+
 <h1>About</h1>
 
 This package includes but is not limited to:
 
 1. A class to create a connection to SQL Server.
 2. A class to transfer data from one SQL Server to another.
 3. Functionality to perform basic data transformations.
@@ -13,20 +31,22 @@
 Key notes:
 
 1. The data is transfered in chunks of 10,000 to optimise memory usage
 2. Enabling logging will produce a file that records each chunk of data transfered.
 
 <h1>Dependencies</h1>
 
-**Required**
+**python 3.8 is required for this package**
+
+**Required Packages**
 
 | Package	| Version	| License						|
 |---------------|---------------|-------------------------------------------------------|
 | pandas	| 1.3.5		| OSI Approved :: BSD License				|
-| SQLAlchemy	| 1.3.5		| MIT License (MIT)					|
+| SQLAlchemy	| 1.4.27		| MIT License (MIT)					|
 
 <h1>Config</h>
 
 <h2>Create and populate a local config_params.ini file</h2>
 
 Windows authentication example:
 
@@ -64,14 +84,16 @@
     
     # make connections
     source_connection = SqlServerConnection('MSSQLSVRA', config_params_path)
     destination_connection = SqlServerConnection('MSSQLSVRB', config_params_path)
    
 <h2>Create an ETL class</h2>
 
+**Positional arguments:**
+
     # define positional etl class variables
     source_sql = r'''SELECT * FROM TESTDB.dbo.tbl_test'''
     destination_database = 'TESTDB'
     destination_table = 'tbl_test'
     
     # define optional etl class variables
     xforms = [
@@ -82,25 +104,25 @@
     dtypes = {'test_text':sqlalchemy.types.NVARCHAR(length=100)}
     # destination_schema = 'someschema'
     
     # create etl class
     etl_1 = Etl(source_sql, destination_database, destination_table, source_connection, destination_connection
         , xforms = xforms
         , dtypes = dtypes
-        # , schema=destination_schema
+        # , destination_schema=destination_schema
         , log_path=log_path)
 
 <h2>Create other ETL classes and put them all in a list</h2>
 
     # create other etl classes as required
     
     # create a list of etl classes
     xfers = [
         etl_1
-        , # etl_2
+        # , etl_2
         ]
 
 <h2>Execute the ETL classes</h2>
 
     # iterate through the etl list and execute the etl classes
     for xf in xfers:
         
@@ -115,8 +137,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `databarge-2.0.1/pyproject.toml` & `databarge-2.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "databarge"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
   { name="Port Verte", email="porte_verte@outlook.com" },
 ]
-description = "Simple ETL tools and functions for SQL Server"
+description = "Simple ETL tools for SQL Server"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `databarge-2.0.1/src/databarge/connections.py` & `databarge-2.0.2/src/databarge/connections.py`

 * *Files identical despite different names*

### Comparing `databarge-2.0.1/src/databarge/dimensions.py` & `databarge-2.0.2/src/databarge/dimensions.py`

 * *Files identical despite different names*

### Comparing `databarge-2.0.1/src/databarge/execution.py` & `databarge-2.0.2/src/databarge/execution.py`

 * *Files identical despite different names*

### Comparing `databarge-2.0.1/src/databarge/transfers.py` & `databarge-2.0.2/src/databarge/transfers.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,18 +209,18 @@
         for key, value in kwargs.items():
             if key == 'xforms':
                 self.xforms = value                
         self.dtypes = None
         for key, value in kwargs.items():
             if key == 'dtypes':
                 self.dtypes = value        
-        self.schema = 'dbo'
+        self.destination_schema = 'dbo'
         for key, value in kwargs.items():
-            if key == 'schema':
-                self.schema = value
+            if key == 'destination_schema':
+                self.destination_schema = value
         self.log_path = None
         for key, value in kwargs.items():
             if key == 'log_path':
                 self.log_path = value
 
         # set other variables
         self.log_text = None 
@@ -235,15 +235,15 @@
         else:
             print(datetime.datetime.now().strftime("%d/%m/%Y: %H:%M:%S") + ': ' + log_text)
         
         my_sql = "USE " + self.dest_db
         self.dest_conn.cursor.execute(my_sql)
         self.dest_conn.connection.commit()
 
-        my_sql = "IF EXISTS (SELECT * FROM sys.objects WHERE object_id = OBJECT_ID(N'[" + self.schema + "].[" + self.dest_tbl + "]') AND type in (N'U')) TRUNCATE TABLE [" + self.schema + "].[" + self.dest_tbl + "]"
+        my_sql = "IF EXISTS (SELECT * FROM sys.objects WHERE object_id = OBJECT_ID(N'[" + self.destination_schema + "].[" + self.dest_tbl + "]') AND type in (N'U')) TRUNCATE TABLE [" + self.destination_schema + "].[" + self.dest_tbl + "]"
         self.dest_conn.cursor.execute(my_sql)
         self.dest_conn.connection.commit()
         
         log_text = "truncation of " + self.dest_tbl + " finished"
         if self.log_path != None:
             self.__write_to_log(log_text)
         else:
@@ -259,15 +259,15 @@
         else:
             print(datetime.datetime.now().strftime("%d/%m/%Y: %H:%M:%S") + ': ' + log_text)
         
         my_sql = "USE " + self.dest_db
         self.dest_conn.cursor.execute(my_sql)
         self.dest_conn.connection.commit()
         
-        my_sql = "IF EXISTS (SELECT * FROM sys.objects WHERE object_id = OBJECT_ID(N'[" + self.schema + "].[" + self.dest_tbl + "]') AND type in (N'U')) DROP TABLE [" + self.schema + "].[" + self.dest_tbl + "]"
+        my_sql = "IF EXISTS (SELECT * FROM sys.objects WHERE object_id = OBJECT_ID(N'[" + self.destination_schema + "].[" + self.dest_tbl + "]') AND type in (N'U')) DROP TABLE [" + self.destination_schema + "].[" + self.dest_tbl + "]"
         self.dest_conn.cursor.execute(my_sql)
         self.dest_conn.connection.commit()
         
         log_text = "dropping of " + self.dest_tbl + " finished"
         if self.log_path != None:
             self.__write_to_log(log_text)
         else:
@@ -296,15 +296,15 @@
             for t in self.xforms:
                 exec(t)
             
             # use the desired database -- use ENGINE.execute -- and do NOT commit this line -- otherwise the default database will be used
             self.dest_conn.engine.execute("USE " + self.dest_db)
             
             # export the chunk to sql server
-            df.to_sql(self.dest_tbl, self.dest_conn.engine, if_exists='append', index=False, schema=self.schema, dtype=self.dtypes)
+            df.to_sql(self.dest_tbl, self.dest_conn.engine, if_exists='append', index=False, schema=self.destination_schema, dtype=self.dtypes)
             
             # tell the log file which chunk of which table has just finished
             log_text = 'transfer to ' + self.dest_tbl + ': chunk ' + str(i) + ' finished'
             if self.log_path != None:
                 self.__write_to_log(log_text)
             else:
                 print(datetime.datetime.now().strftime("%d/%m/%Y: %H:%M:%S") + ': ' + log_text)
```

### Comparing `databarge-2.0.1/src/databarge.egg-info/PKG-INFO` & `databarge-2.0.2/src/databarge.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: databarge
-Version: 2.0.1
-Summary: Simple ETL tools and functions for SQL Server
+Version: 2.0.2
+Summary: Simple ETL tools for SQL Server
 Home-page: https://github.com/porteverte/databarge
 Author: Porte Verte
 Author-email: Port Verte <porte_verte@outlook.com>
 Project-URL: Homepage, https://github.com/porteverte/databarge
 Project-URL: Issues, https://github.com/porteverte/databarge/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+**databarge | simple ETL tools for SQL Server**
+
 <h1>About</h1>
 
 This package includes but is not limited to:
 
 1. A class to create a connection to SQL Server.
 2. A class to transfer data from one SQL Server to another.
 3. Functionality to perform basic data transformations.
@@ -29,20 +31,22 @@
 Key notes:
 
 1. The data is transfered in chunks of 10,000 to optimise memory usage
 2. Enabling logging will produce a file that records each chunk of data transfered.
 
 <h1>Dependencies</h1>
 
-**Required**
+**python 3.8 is required for this package**
+
+**Required Packages**
 
 | Package	| Version	| License						|
 |---------------|---------------|-------------------------------------------------------|
 | pandas	| 1.3.5		| OSI Approved :: BSD License				|
-| SQLAlchemy	| 1.3.5		| MIT License (MIT)					|
+| SQLAlchemy	| 1.4.27		| MIT License (MIT)					|
 
 <h1>Config</h>
 
 <h2>Create and populate a local config_params.ini file</h2>
 
 Windows authentication example:
 
@@ -80,14 +84,16 @@
     
     # make connections
     source_connection = SqlServerConnection('MSSQLSVRA', config_params_path)
     destination_connection = SqlServerConnection('MSSQLSVRB', config_params_path)
    
 <h2>Create an ETL class</h2>
 
+**Positional arguments:**
+
     # define positional etl class variables
     source_sql = r'''SELECT * FROM TESTDB.dbo.tbl_test'''
     destination_database = 'TESTDB'
     destination_table = 'tbl_test'
     
     # define optional etl class variables
     xforms = [
@@ -98,25 +104,25 @@
     dtypes = {'test_text':sqlalchemy.types.NVARCHAR(length=100)}
     # destination_schema = 'someschema'
     
     # create etl class
     etl_1 = Etl(source_sql, destination_database, destination_table, source_connection, destination_connection
         , xforms = xforms
         , dtypes = dtypes
-        # , schema=destination_schema
+        # , destination_schema=destination_schema
         , log_path=log_path)
 
 <h2>Create other ETL classes and put them all in a list</h2>
 
     # create other etl classes as required
     
     # create a list of etl classes
     xfers = [
         etl_1
-        , # etl_2
+        # , etl_2
         ]
 
 <h2>Execute the ETL classes</h2>
 
     # iterate through the etl list and execute the etl classes
     for xf in xfers:
```

