# Comparing `tmp/stelladb-0.2.4.tar.gz` & `tmp/stelladb-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stelladb-0.2.4.tar", last modified: Fri Mar 29 19:40:37 2024, max compression
+gzip compressed data, was "stelladb-0.2.5.tar", last modified: Mon Apr  1 19:23:56 2024, max compression
```

## Comparing `stelladb-0.2.4.tar` & `stelladb-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:40:37.677632 stelladb-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-29 19:39:44.000000 stelladb-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-29 19:40:37.677632 stelladb-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-29 19:39:44.000000 stelladb-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-29 19:40:37.677632 stelladb-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-03-29 19:39:44.000000 stelladb-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:40:37.677632 stelladb-0.2.4/stelladb/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-29 19:39:44.000000 stelladb-0.2.4/stelladb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-29 19:40:37.677632 stelladb-0.2.4/stelladb/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-03-29 19:39:44.000000 stelladb-0.2.4/stelladb/db_desc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-03-29 19:39:44.000000 stelladb-0.2.4/stelladb/db_vmec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:40:37.677632 stelladb-0.2.4/stelladb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-29 19:40:37.000000 stelladb-0.2.4/stelladb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-29 19:40:37.000000 stelladb-0.2.4/stelladb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 19:40:37.000000 stelladb-0.2.4/stelladb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-29 19:40:37.000000 stelladb-0.2.4/stelladb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-29 19:40:37.000000 stelladb-0.2.4/stelladb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:23:56.079012 stelladb-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-01 19:23:01.000000 stelladb-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-01 19:23:56.079012 stelladb-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-01 19:23:01.000000 stelladb-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-01 19:23:56.079012 stelladb-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-01 19:23:01.000000 stelladb-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:23:56.079012 stelladb-0.2.5/stelladb/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-01 19:23:01.000000 stelladb-0.2.5/stelladb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-01 19:23:56.079012 stelladb-0.2.5/stelladb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24692 2024-04-01 19:23:01.000000 stelladb-0.2.5/stelladb/db_desc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-04-01 19:23:01.000000 stelladb-0.2.5/stelladb/db_vmec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:23:56.075013 stelladb-0.2.5/stelladb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-01 19:23:56.000000 stelladb-0.2.5/stelladb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-01 19:23:56.000000 stelladb-0.2.5/stelladb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:23:56.000000 stelladb-0.2.5/stelladb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 19:23:56.000000 stelladb-0.2.5/stelladb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 19:23:56.000000 stelladb-0.2.5/stelladb.egg-info/top_level.txt
```

### Comparing `stelladb-0.2.4/LICENSE` & `stelladb-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `stelladb-0.2.4/PKG-INFO` & `stelladb-0.2.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stelladb
-Version: 0.2.4
+Version: 0.2.5
 Summary: Includes functions to upload DESC and VMEC data to the stellarator database.
 Home-page: https://github.com/PlasmaControl/Stellarator-Database/
 Author: Yigit Gunsur Elmacioglu, Rory Conlin, Dario Panici, Egemen Kolemen
 Author-email: PlasmaControl@princeton.edu
 License: MIT
 Keywords: stellarator tokamak equilibrium perturbation mhd magnetohydrodynamics stability confinement plasma physics optimization design fusion data database
 Requires-Python: >=3.9
@@ -33,21 +33,33 @@
 Once you get the files,
 ```bash
 cd Stellarator-Database
 ```
 
 ### Building conda environment
 ```bash
-conda create --name db
+conda create --name db 'python>=3.9, <=3.12'
 conda activate db
 pip install -r requirements.txt
 ```
 
 ## Sample usage
 ```python
 from desc.examples import get
-import stelladb
+from stelladb import save_to_db_desc
 
 eq = get("HELIOTRON")
+
+# if you are using DESC, you can directly upload Equilibrium or 
+# EquilibriumFamily objects. For EquilibriumFamily, only the last
+# Equilibrium will be uploaded.
+save_to_db_desc(eq, configid="HELIOTRON", user="username")
+
+# if you have an outfile, supply the name of it without extension
+# For DESC example, we need to save it first to get the .h5 file
 eq.save("test_output_HELIOTRON.h5")
 save_to_db_desc("test_output_HELIOTRON", configid="HELIOTRON", user="username")
+
+# use copy parameter, if you want the local copy of the files that are uploaded
+# default value is False
+save_to_db_desc(eq, configid="HELIOTRON", user="username", copy=True)
 ```
```

### Comparing `stelladb-0.2.4/setup.py` & `stelladb-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `stelladb-0.2.4/stelladb/db_desc.py` & `stelladb-0.2.5/stelladb/db_desc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import os
+from desc.equilibrium import Equilibrium, EquilibriaFamily
 from desc.grid import LinearGrid
 from desc.vmec_utils import ptolemy_identity_rev, zernike_to_fourier
 import zipfile
 
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 
-from desc.io.hdf5_io import hdf5Reader, hdf5Writer
+from desc.io.hdf5_io import hdf5Reader
 from desc.io.equilibrium_io import load
 import numpy as np
 import csv
 from datetime import date
 
 
 def save_to_db_desc(  # pragma: no cover
-    filename,
+    eq,
     configid,
     user,
     isDeviceNew=False,
     deviceid=None,
     description=None,
     provenance=None,
     inputfilename=None,
@@ -32,49 +33,113 @@
     device_stell_sym=False,
     copy=False,
 ):
     """Load a DESC equilibrium and upload it to the database.
 
     Parameters
     ----------
-    filename : str
+    eq : str, Equilibrium or EquilibriumFamily
         file path of the output file without .h5 extension
+        or the equilibrium to be uploaded
     configid : str
         unique identifier for the configuration
     initialization_method : str (Default: 'surface')
         method used to initialize the equilibrium
-    user :
+    user : str
         user who created the equilibrium (must have an account on the database)
+    isDeviceNew : bool (Default: False)
+        True if the device is new and should be uploaded to the database
+    deviceid : str (Default: None)
+        unique identifier for the device
+    description : str (Default: None)
+        description of the configuration
+    provenance : str (Default: None)
+        where the configuration came from
+    inputfilename : str (Default: None)
+        name of the input file corresponding to this configuration
+    config_class : str (Default: None)
+        class of configuration i.e. quasisymmetry (QA, QH, QP)
+        or omnigenity (QI, OT, OH) or axisymmetry (AS)
+    current : bool (Default: True)
+        True if the equilibrium was solved with fixed current or not if False,
+        was solved with fixed iota
+    deviceNFP : int (Default: 1)
+        number of field periods for the device
+    deviceDescription : str (Default: None)
+        description of the device
+    device_stell_sym : bool (Default: False)
+        stellarator symmetry of the device
+    copy : bool (Default: False)
+        True if the zip and csv files should be kept after uploading
 
     """
     zip_upload_button_id = "zipToUpload"
     csv_upload_button_id = "descToUpload"
     cfg_upload_button_id = "configToUpload"
     device_upload_button_id = "deviceToUpload"
     confirm_button_id = "confirmDesc"
 
+    if isinstance(eq, str):
+        if os.path.exists(eq + ".h5"):
+            filename = eq
+            eq = eq + ".h5"
+        else:
+            raise FileNotFoundError(f"{eq}.h5 does not exist.")
+    elif isinstance(eq, Equilibrium):
+        eq = eq
+        filename = configid
+    elif isinstance(eq, EquilibriaFamily):
+        eq = eq
+        filename = configid
+    else:
+        raise TypeError(
+            "Expected type str, Equilibrium or EquilibriumFamily "
+            + f"for eq, got type {type(eq)}"
+        )
+    if os.path.exists("auto_save.h5"):
+        print("Removing auto_save.h5")
+        os.remove("auto_save.h5")
+
     # Check input files, if there isn't any create automatically
     if inputfilename is None:
         if os.path.exists("auto_generated_" + filename + "_input.txt"):
             inputfilename = "auto_generated_" + filename + "_input.txt"
         elif os.path.exists(filename + "_input.txt"):
             inputfilename = filename + "_input.txt"
         else:
             inputfilename = "auto_generated_" + filename + "_input.txt"
             from desc.input_reader import InputReader
 
             print("Auto-generating input file...")
             writer = InputReader()
-            writer.desc_output_to_input(inputfilename, filename + ".h5")
+            if isinstance(eq, str):
+                writer.desc_output_to_input(inputfilename, eq)
+            elif isinstance(eq, Equilibrium):
+                eq.save("auto_save.h5")
+                writer.desc_output_to_input(inputfilename, "auto_save.h5")
+            elif isinstance(eq, EquilibriaFamily):
+                eq[-1].save("auto_save.h5")
+                writer.desc_output_to_input(inputfilename, "auto_save.h5")
 
     # Zip the files
     print("Zipping files...")
     zip_filename = filename + ".zip"
     with zipfile.ZipFile(zip_filename, "w") as zipf:
-        zipf.write(filename + ".h5")
+        if os.path.exists(filename + ".h5"):
+            zipf.write(filename + ".h5")
+        elif isinstance(eq, Equilibrium):
+            print("Saving equilibrium to .h5 file...")
+            if not os.path.exists("auto_save.h5"):
+                eq.save("auto_save.h5")
+            zipf.write("auto_save.h5")
+        elif isinstance(eq, EquilibriaFamily):
+            print("Saving equilibrium to .h5 file...")
+            if not os.path.exists("auto_save.h5"):
+                eq[-1].save("auto_save.h5")
+            zipf.write("auto_save.h5")
         if inputfilename is not None:
             if os.path.exists(inputfilename):
                 zipf.write(inputfilename)
 
     csv_filename = "desc_runs.csv"
     config_csv_filename = "configurations.csv"
     device_csv_filename = "devices_and_concepts.csv"
@@ -86,15 +151,15 @@
         print(f"Previous {config_csv_filename} has been deleted.")
     if os.path.exists(device_csv_filename):
         os.remove(device_csv_filename)
         print(f"Previous {device_csv_filename} has been deleted.")
 
     print("Creating desc_runs.csv and configurations.csv...")
     desc_to_csv(
-        filename + ".h5",  # output filename
+        eq,  # output filename
         name=configid,  # some string descriptive name, not necessarily unique
         provenance=provenance,
         description=description,
         inputfilename=inputfilename,
         current=current,
         deviceid=deviceid,
         config_class=config_class,
@@ -180,14 +245,16 @@
         message_element = driver.find_element(By.ID, "messageContainer")
         message = message_element.text
         print(message)
 
     finally:
         # Clean up resources
         driver.quit()
+        if os.path.exists("auto_save.h5"):
+            os.remove("auto_save.h5")
         if not copy:
             os.remove(zip_filename)
             os.remove(csv_filename)
             os.remove(config_csv_filename)
             os.remove(inputfilename)
             if isDeviceNew:
                 os.remove(device_csv_filename)
@@ -207,16 +274,17 @@
     output_csv_name_config="configurations.csv",
     **kwargs,
 ):
     """Save DESC output file as a csv with relevant information.
 
     Parameters
     ----------
-        eq : str
-            DESC equilibrium to save or path to .h5 of DESC equilibrium to save
+        eq : str, Equilibrium or EquilibriumFamily
+            file path of the output file without .h5 extension
+            or the equilibrium to be uploaded
         current : bool
             True if the equilibrium was solved with fixed current or not if False,
             was solved with fixed iota
         name : str
             name of configuration (and desc run)
         provenance : str
             where this configuration (and desc run) came from, e.g. DESC github repo
@@ -259,31 +327,42 @@
     configurations_csv_name = output_csv_name_config
 
     if isinstance(eq, str) and os.path.exists(eq):
         data_desc_runs["outputfile"] = os.path.basename(eq)
         reader = hdf5Reader(eq)
         version = reader.read_dict()["__version__"]
         eq = load(eq)[-1]
+    elif isinstance(eq, Equilibrium):
+        import desc
+
+        version = desc.__version__
+        data_desc_runs["outputfile"] = "auto_save.h5"
+    elif isinstance(eq, EquilibriaFamily):
+        import desc
+
+        eq = eq[-1]
+        version = desc.__version__
+        data_desc_runs["outputfile"] = "auto_save.h5"
     else:
-        raise TypeError(f"Expected type str for eq, got type {type(eq)}")
+        raise TypeError(
+            "Expected type str, Equilibrium or EquilibriumFamily "
+            + f"for eq, got type {type(eq)}"
+        )
 
     ############ DESC_runs Data Table ############
     if name is not None:
         data_desc_runs["configid"] = name
     if provenance is not None:
         data_desc_runs["provenance"] = provenance
     if description is not None:
         data_desc_runs["description"] = description
 
     data_desc_runs["version"] = (
         version  # this is basically redundant with git commit I think
     )
-    data_desc_runs["git_commit"] = (
-        version  # this is basically redundant with git commit I think
-    )
     if inputfilename is not None:
         data_desc_runs["inputfilename"] = inputfilename
 
     data_desc_runs["initialization_method"] = initialization_method
 
     data_desc_runs["l_rad"] = eq.L
     data_desc_runs["l_grid"] = eq.L_grid
@@ -550,39 +629,42 @@
         print("I/O error")
 
     return None
 
 
 def get_driver():  # pragma: no cover
     """Initialize a webdriver for use in uploading to the database."""
+
+    try:
+        options = webdriver.ChromeOptions()
+        options.headless = True
+        return webdriver.Chrome(options=options)
+    except:  # noqa: E722
+        pass
+
     try:
         options = webdriver.FirefoxOptions()
         options.headless = True
         return webdriver.Firefox(options=options)
     except:  # noqa: E722
         pass
 
     try:
-        options = webdriver.ChromeOptions()
-        options.headless = True
-        return webdriver.Chrome(options=options)
+        return webdriver.Safari()
     except:  # noqa: E722
         pass
 
     try:
         options = webdriver.EdgeOptions()
         options.use_chromium = True
         options.add_argument("headless")
         return webdriver.Edge(options=options)
     except:  # noqa: E722
-        pass
+        import warnings
 
-    try:
-        return webdriver.Safari()
-    except:  # noqa: E722
-        print(
+        warnings.warn(
             "Failed to initialize any webdriver! Consider installing "
             + "Chrome, Safari, Firefox, or Edge."
         )
 
     # If no browser was successfully initialized, return None
     return None
```

### Comparing `stelladb-0.2.4/stelladb/db_vmec.py` & `stelladb-0.2.5/stelladb/db_vmec.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,14 @@
     data_vmec_runs["configid"] = name
     if provenance is not None:
         data_vmec_runs["provenance"] = provenance
     if description is not None:
         data_vmec_runs["description"] = description
 
     data_vmec_runs["version"] = version  # version property in wout
-    data_vmec_runs["git_commit"] = version  # not sure how this is standarised for vmec
     if inputfilename is not None:
         data_vmec_runs["inputfilename"] = inputfilename
 
     data_vmec_runs["initialization_method"] = (
         initialization_method  # Not sure what this is
     )
```

### Comparing `stelladb-0.2.4/stelladb.egg-info/PKG-INFO` & `stelladb-0.2.5/stelladb.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stelladb
-Version: 0.2.4
+Version: 0.2.5
 Summary: Includes functions to upload DESC and VMEC data to the stellarator database.
 Home-page: https://github.com/PlasmaControl/Stellarator-Database/
 Author: Yigit Gunsur Elmacioglu, Rory Conlin, Dario Panici, Egemen Kolemen
 Author-email: PlasmaControl@princeton.edu
 License: MIT
 Keywords: stellarator tokamak equilibrium perturbation mhd magnetohydrodynamics stability confinement plasma physics optimization design fusion data database
 Requires-Python: >=3.9
@@ -33,21 +33,33 @@
 Once you get the files,
 ```bash
 cd Stellarator-Database
 ```
 
 ### Building conda environment
 ```bash
-conda create --name db
+conda create --name db 'python>=3.9, <=3.12'
 conda activate db
 pip install -r requirements.txt
 ```
 
 ## Sample usage
 ```python
 from desc.examples import get
-import stelladb
+from stelladb import save_to_db_desc
 
 eq = get("HELIOTRON")
+
+# if you are using DESC, you can directly upload Equilibrium or 
+# EquilibriumFamily objects. For EquilibriumFamily, only the last
+# Equilibrium will be uploaded.
+save_to_db_desc(eq, configid="HELIOTRON", user="username")
+
+# if you have an outfile, supply the name of it without extension
+# For DESC example, we need to save it first to get the .h5 file
 eq.save("test_output_HELIOTRON.h5")
 save_to_db_desc("test_output_HELIOTRON", configid="HELIOTRON", user="username")
+
+# use copy parameter, if you want the local copy of the files that are uploaded
+# default value is False
+save_to_db_desc(eq, configid="HELIOTRON", user="username", copy=True)
 ```
```

