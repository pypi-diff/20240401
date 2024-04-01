# Comparing `tmp/RipeDB-0.3.3.tar.gz` & `tmp/RipeDB-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RipeDB-0.3.3.tar", last modified: Tue Mar 26 10:52:05 2024, max compression
+gzip compressed data, was "RipeDB-0.3.4.tar", last modified: Mon Apr  1 16:45:09 2024, max compression
```

## Comparing `RipeDB-0.3.3.tar` & `RipeDB-0.3.4.tar`

### file list

```diff
@@ -1,19 +1,31 @@
-drwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-03-26 10:52:05.736138 RipeDB-0.3.3/
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)     1081 2024-02-03 18:25:10.000000 RipeDB-0.3.3/LICENSE
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)     1740 2024-03-26 10:52:05.731621 RipeDB-0.3.3/PKG-INFO
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)     1413 2024-03-26 08:24:11.000000 RipeDB-0.3.3/README.md
-drwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-03-26 10:52:05.726623 RipeDB-0.3.3/RipeDB.egg-info/
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)     1740 2024-03-26 10:52:05.000000 RipeDB-0.3.3/RipeDB.egg-info/PKG-INFO
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)      289 2024-03-26 10:52:05.000000 RipeDB-0.3.3/RipeDB.egg-info/SOURCES.txt
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)        1 2024-03-26 10:52:05.000000 RipeDB-0.3.3/RipeDB.egg-info/dependency_links.txt
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)       44 2024-03-26 10:52:05.000000 RipeDB-0.3.3/RipeDB.egg-info/entry_points.txt
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)       25 2024-03-26 10:52:05.000000 RipeDB-0.3.3/RipeDB.egg-info/requires.txt
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)        7 2024-03-26 10:52:05.000000 RipeDB-0.3.3/RipeDB.egg-info/top_level.txt
-drwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-03-26 10:52:05.693544 RipeDB-0.3.3/ripedb/
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)       13 2024-03-26 09:43:47.000000 RipeDB-0.3.3/ripedb/__init__.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)     7065 2024-03-26 10:51:37.000000 RipeDB-0.3.3/ripedb/main.py
-drwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-03-26 10:52:05.715108 RipeDB-0.3.3/ripedb/utils/
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)       13 2024-03-21 08:03:46.000000 RipeDB-0.3.3/ripedb/utils/__init__.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)     5379 2024-03-21 10:02:07.000000 RipeDB-0.3.3/ripedb/utils/utils.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)       38 2024-03-26 10:52:05.737140 RipeDB-0.3.3/setup.cfg
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)      725 2024-03-26 10:51:30.000000 RipeDB-0.3.3/setup.py
+drwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-04-01 16:45:09.023691 RipeDB-0.3.4/
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)     1081 2024-02-03 18:25:10.000000 RipeDB-0.3.4/LICENSE
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)     2087 2024-04-01 16:45:09.017670 RipeDB-0.3.4/PKG-INFO
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)     1794 2024-03-29 17:52:53.000000 RipeDB-0.3.4/README.md
+drwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-04-01 16:45:09.001467 RipeDB-0.3.4/RipeDB.egg-info/
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)     2087 2024-04-01 16:45:07.000000 RipeDB-0.3.4/RipeDB.egg-info/PKG-INFO
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      687 2024-04-01 16:45:08.000000 RipeDB-0.3.4/RipeDB.egg-info/SOURCES.txt
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)        1 2024-04-01 16:45:07.000000 RipeDB-0.3.4/RipeDB.egg-info/dependency_links.txt
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)       44 2024-04-01 16:45:07.000000 RipeDB-0.3.4/RipeDB.egg-info/entry_points.txt
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)       25 2024-04-01 16:45:07.000000 RipeDB-0.3.4/RipeDB.egg-info/requires.txt
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)        7 2024-04-01 16:45:07.000000 RipeDB-0.3.4/RipeDB.egg-info/top_level.txt
+drwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-04-01 16:45:08.703035 RipeDB-0.3.4/ripedb/
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)       13 2024-03-26 09:43:47.000000 RipeDB-0.3.4/ripedb/__init__.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)     7755 2024-03-29 22:08:51.000000 RipeDB-0.3.4/ripedb/main.py
+drwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-04-01 16:45:08.985324 RipeDB-0.3.4/ripedb/utils/
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)       13 2024-03-29 14:12:13.000000 RipeDB-0.3.4/ripedb/utils/__init__.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      425 2024-03-29 21:11:31.000000 RipeDB-0.3.4/ripedb/utils/expand_ip_range.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      445 2024-04-01 16:42:48.000000 RipeDB-0.3.4/ripedb/utils/export_xlsx.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)     1292 2024-03-29 21:11:31.000000 RipeDB-0.3.4/ripedb/utils/export_xlsx_new_sheet.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      566 2024-03-29 21:11:31.000000 RipeDB-0.3.4/ripedb/utils/get_export_path.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      608 2024-03-29 21:11:31.000000 RipeDB-0.3.4/ripedb/utils/get_ripe_reverse_dns.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      413 2024-03-29 14:37:33.000000 RipeDB-0.3.4/ripedb/utils/helper.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)     1465 2024-03-29 21:11:31.000000 RipeDB-0.3.4/ripedb/utils/process_input_indixes.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      626 2024-03-29 21:11:31.000000 RipeDB-0.3.4/ripedb/utils/range_to_cidr.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      528 2024-03-29 21:11:31.000000 RipeDB-0.3.4/ripedb/utils/remove_lines.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-03-29 21:11:31.000000 RipeDB-0.3.4/ripedb/utils/remove_rows.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      717 2024-03-29 21:11:31.000000 RipeDB-0.3.4/ripedb/utils/request_and_validate_indices.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      570 2024-03-29 21:11:31.000000 RipeDB-0.3.4/ripedb/utils/request_confirm.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      473 2024-03-29 21:11:31.000000 RipeDB-0.3.4/ripedb/utils/reverse_dns.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)       38 2024-04-01 16:45:09.023691 RipeDB-0.3.4/setup.cfg
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      701 2024-04-01 16:43:08.000000 RipeDB-0.3.4/setup.py
```

### Comparing `RipeDB-0.3.3/LICENSE` & `RipeDB-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `RipeDB-0.3.3/PKG-INFO` & `RipeDB-0.3.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: RipeDB
-Version: 0.3.3
-Summary: Uno strumento per effettuare query e analisi su RipeDB
+Version: 0.3.4
+Summary: A tool for making analyssis on RipeDB
 Home-page: https://github.com/apt-0/RipeDB
 Author: APT-0-Blog
 Author-email: cryptovortex@outlook.com
 Keywords: ripe ripedb
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: openpyxl
 
 [![Downloads](https://static.pepy.tech/badge/ripedb)](https://pepy.tech/project/ripedb)
 
 # RipeDB
 <p align="center">
-  <img src="https://github.com/apt-0/RipeDB/blob/main/RipeDB_Image.jpg" width="300" height="300">
+  <img src="https://github.com/apt-0/RipeDB/blob/main/assets/RipeDB_Image.jpg" width="300" height="300">
 </p>
 
 RipeDB is a Python tool designed to facilitate the search and analysis of internet domain data through the RIPE DATABASE. This project allows users to obtain detailed information about domains and their IP assignments.
 
 ## Features
 
 - Search for domain information using customizable parameters.
@@ -29,29 +29,48 @@
 
 ## Prerequisites
 
 Before you begin, make sure you have Python 3.x installed on your system. RipeDB depends on some external packages, which are listed in the requirements.txt file.
 
 ## Installation
 
-### PIP
+### Stable Version
 RipeDB can be easily installed via pip. This method is recommended for most users as it automatically manages all project dependencies.
 
 To install RipeDB, run the following command:
 
 ```bash
 pip install ripedb
 ```
+
+### Latest Version
+If you want the latest Features use this methods:
+
+#### PIP
+```bash
+git clone https://github.com/apt-0/RipeDB
+cd RipeDB
+pip install .
+```
+
+#### Python
+```bash
+git clone https://github.com/apt-0/RipeDB
+cd RipeDB
+python -m ripedb.main
+```
+
 ## Usage
 To start RipeDB, run the following command:
 ```bash
 ripedb
 ```
 Follow the on-screen instructions to enter search parameters and view the results.
 
 ## License
 Distributed under the MIT License. See LICENSE for more information.
 
 ## Contacts
 APT-0  - cryptovortex@outlook.com
 
-Project Link: https://github.com/apt-0/RipeDB
+## Contributors
+[![Contributors](https://contrib.rocks/image?repo=apt-0/RipeDB)](https://github.com/apt-0/RipeDB/graphs/contributors)
```

### Comparing `RipeDB-0.3.3/README.md` & `RipeDB-0.3.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![Downloads](https://static.pepy.tech/badge/ripedb)](https://pepy.tech/project/ripedb)
 
 # RipeDB
 <p align="center">
-  <img src="https://github.com/apt-0/RipeDB/blob/main/RipeDB_Image.jpg" width="300" height="300">
+  <img src="https://github.com/apt-0/RipeDB/blob/main/assets/RipeDB_Image.jpg" width="300" height="300">
 </p>
 
 RipeDB is a Python tool designed to facilitate the search and analysis of internet domain data through the RIPE DATABASE. This project allows users to obtain detailed information about domains and their IP assignments.
 
 ## Features
 
 - Search for domain information using customizable parameters.
@@ -15,29 +15,48 @@
 
 ## Prerequisites
 
 Before you begin, make sure you have Python 3.x installed on your system. RipeDB depends on some external packages, which are listed in the requirements.txt file.
 
 ## Installation
 
-### PIP
+### Stable Version
 RipeDB can be easily installed via pip. This method is recommended for most users as it automatically manages all project dependencies.
 
 To install RipeDB, run the following command:
 
 ```bash
 pip install ripedb
 ```
+
+### Latest Version
+If you want the latest Features use this methods:
+
+#### PIP
+```bash
+git clone https://github.com/apt-0/RipeDB
+cd RipeDB
+pip install .
+```
+
+#### Python
+```bash
+git clone https://github.com/apt-0/RipeDB
+cd RipeDB
+python -m ripedb.main
+```
+
 ## Usage
 To start RipeDB, run the following command:
 ```bash
 ripedb
 ```
 Follow the on-screen instructions to enter search parameters and view the results.
 
 ## License
 Distributed under the MIT License. See LICENSE for more information.
 
 ## Contacts
 APT-0  - cryptovortex@outlook.com
 
-Project Link: https://github.com/apt-0/RipeDB
+## Contributors
+[![Contributors](https://contrib.rocks/image?repo=apt-0/RipeDB)](https://github.com/apt-0/RipeDB/graphs/contributors)
```

### Comparing `RipeDB-0.3.3/RipeDB.egg-info/PKG-INFO` & `RipeDB-0.3.4/RipeDB.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: RipeDB
-Version: 0.3.3
-Summary: Uno strumento per effettuare query e analisi su RipeDB
+Version: 0.3.4
+Summary: A tool for making analyssis on RipeDB
 Home-page: https://github.com/apt-0/RipeDB
 Author: APT-0-Blog
 Author-email: cryptovortex@outlook.com
 Keywords: ripe ripedb
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: openpyxl
 
 [![Downloads](https://static.pepy.tech/badge/ripedb)](https://pepy.tech/project/ripedb)
 
 # RipeDB
 <p align="center">
-  <img src="https://github.com/apt-0/RipeDB/blob/main/RipeDB_Image.jpg" width="300" height="300">
+  <img src="https://github.com/apt-0/RipeDB/blob/main/assets/RipeDB_Image.jpg" width="300" height="300">
 </p>
 
 RipeDB is a Python tool designed to facilitate the search and analysis of internet domain data through the RIPE DATABASE. This project allows users to obtain detailed information about domains and their IP assignments.
 
 ## Features
 
 - Search for domain information using customizable parameters.
@@ -29,29 +29,48 @@
 
 ## Prerequisites
 
 Before you begin, make sure you have Python 3.x installed on your system. RipeDB depends on some external packages, which are listed in the requirements.txt file.
 
 ## Installation
 
-### PIP
+### Stable Version
 RipeDB can be easily installed via pip. This method is recommended for most users as it automatically manages all project dependencies.
 
 To install RipeDB, run the following command:
 
 ```bash
 pip install ripedb
 ```
+
+### Latest Version
+If you want the latest Features use this methods:
+
+#### PIP
+```bash
+git clone https://github.com/apt-0/RipeDB
+cd RipeDB
+pip install .
+```
+
+#### Python
+```bash
+git clone https://github.com/apt-0/RipeDB
+cd RipeDB
+python -m ripedb.main
+```
+
 ## Usage
 To start RipeDB, run the following command:
 ```bash
 ripedb
 ```
 Follow the on-screen instructions to enter search parameters and view the results.
 
 ## License
 Distributed under the MIT License. See LICENSE for more information.
 
 ## Contacts
 APT-0  - cryptovortex@outlook.com
 
-Project Link: https://github.com/apt-0/RipeDB
+## Contributors
+[![Contributors](https://contrib.rocks/image?repo=apt-0/RipeDB)](https://github.com/apt-0/RipeDB/graphs/contributors)
```

### Comparing `RipeDB-0.3.3/ripedb/main.py` & `RipeDB-0.3.4/ripedb/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,19 @@
-from ripedb.utils import utils
+from ripedb.utils import range_to_cidr, request_confirm, helper, request_and_validate_indices, remove_lines, reverse_dns, get_ripe_reverse_dns, expand_ip_range, get_export_path, export_xlsx, export_xlsx_new_sheet
 import sys
 import xml.etree.ElementTree as ET
 import os
-
-try:
-    import requests
-except ImportError:
-    print('[!] Module "requests" not installed. Try: python3 -m pip install requests')
-    sys.exit(-1)
-
-try:
-    import pandas as pd
-except ImportError:
-    print('[!] Module "pandas" not installed. Try: python3 -m pip install pandas')
-    sys.exit(-1)
-
-try:
-    import openpyxl
-except ImportError:
-    print('[!] Module "openpyxl" not installed. Try: python3 -m pip install openpyxl')
-    sys.exit(-1)
-
+import argparse
+import pandas as pd
+import requests
+
+pd.set_option('display.max_rows', None)
+pd.set_option('display.max_columns', None)
+pd.set_option('display.width', 1000)
+pd.set_option('display.max_colwidth', None)
 
 banner = """
 ····················································
 :                                                  :
 : 888 88e  ,e,                  888 88e   888 88b, :
 : 888 888D  "  888 88e   ,e e,  888 888b  888 88P' :
 : 888 88"  888 888 888b d88 88b 888 8888D 888 8K   :
@@ -32,154 +21,178 @@
 : 888 88b, 888 888 88"   "YeeP" 888 88"   888 88P' :
 :              888                                 :
 :              888                                 :
 :                                                  :
 ····················································
 """
 
+
 def main():
     print(banner)
+    parser = argparse.ArgumentParser(
+        description='RipeDB: A tool for performing queries and analysis on RipeDB.')
+    parser.add_argument('command', nargs='?',
+                        help='The command to execute (query, help).')
+    parser.add_argument('-q', '--query', help='Query parameter')
+    parser.add_argument('-em', '--editing-mode',
+                        help='Enable DNS resolution and editing mode', action='store_true')
+
+    args = parser.parse_args()
+
+    if args.command == 'help':
+        helper.show_general_help()
+
     base_url = 'https://apps.db.ripe.net/db-web-ui/api/rest/fulltextsearch/select'
-    dominio_param = input("Enter the search parameter:")
-   
+
+    if args.query:
+        domain_param = args.query
+    else:
+        domain_param = input("Enter the search parameter:")
+
     params = {
         'facet': 'true',
         'format': 'xml',
         'hl': 'true',
-        'q': '('+dominio_param+')',
-        'start': 0,  
+        'q': '('+domain_param+')',
+        'start': 0,
         'wt': 'json'
     }
 
-    # Lista per tenere traccia dei risultati
     results = []
 
     while True:
         response = requests.get(base_url, params=params)
         xml_data = response.text
-        
-        if not xml_data.strip(): 
+
+        if not xml_data.strip():
             print("No data found, exiting the loop.")
             break
-        
+
         root = ET.fromstring(xml_data)
         docs = root.findall('.//doc')
-        
+
         if not docs:
             print("No data found, exiting the loop.")
             break
-        
+
         for doc in docs:
             descr_element = doc.find("str[@name='description']")
             netname_element = doc.find("str[@name='netname']")
             inetnum_element = doc.find("str[@name='inetnum']")
-            
+
             descr_text = descr_element.text if descr_element is not None else "N/A"
             netname_text = netname_element.text if netname_element is not None else "N/A"
             inetnum_text = inetnum_element.text if inetnum_element is not None else "N/A"
-            
-            results.append({"Inetnum": inetnum_text, "Description": descr_text, "NetName": netname_text})
-        
+
+            results.append(
+                {"Inetnum": inetnum_text, "Description": descr_text, "NetName": netname_text})
+
         params['start'] += len(docs)
 
     df = pd.DataFrame(results)
-    pd.set_option('display.max_rows', None)  
-    pd.set_option('display.max_columns', None)  
-    pd.set_option('display.width', 1000)  
-    pd.set_option('display.max_colwidth', None)
 
-    df['CIDR'] = df['Inetnum'].apply(utils.range_to_cidr)
+    df['CIDR'] = df['Inetnum'].apply(range_to_cidr.range_to_cidr)
     inetnum_idx = df.columns.get_loc('Inetnum') + 1
 
     df.insert(inetnum_idx, 'CIDR', df.pop('CIDR'))
 
-    # Rimuozione delle righe dove tutte le colonne sono 'N/A'
-    df = df[(df['Description'] != 'N/A') | (df['NetName'] != 'N/A') | (df['Inetnum'] != 'N/A')]
-    df = df.sort_values(by=['NetName', 'Description', 'Inetnum']).reset_index(drop=True)
-    print("Below are the results found for:"+dominio_param)
+    df = df[(df['Description'] != 'N/A') |
+            (df['NetName'] != 'N/A') | (df['Inetnum'] != 'N/A')]
+    df = df.sort_values(by=['NetName', 'Description',
+                        'Inetnum']).reset_index(drop=True)
+    print("Below are the results found for:"+domain_param)
     print(" ")
     print(df.to_string(index=True))
     print(" ")
-    risposta = utils.richiedi_conferma("Do you want to delete rows? (y/n):")
-    print(" ")
 
-    if risposta:
-        while True:
-            max_indice = len(df) - 1
-            indici_da_rimuovere = utils.richiedi_e_valida_indici(max_indice)
-
-            if indici_da_rimuovere:
-                df = utils.rimuovi_righe(df, indici_da_rimuovere)
-                print(df.to_string(index=True))
-            else:
-                print("")
-                break
-    
-            print(" ")
+    if args.editing_mode:
+        reply = request_confirm.request_confirm("Do you want to delete rows? (y/n):")
+        print(" ")
 
-    # Esporta in xlsx
-    risposta = utils.richiedi_conferma("Do you want to export the results to an xslx file? (y/n):")
-    print(" ")
-    if risposta:
-        export_path = utils.get_export_path("Enter the export path for the xslx file (leave blank to use the current directory): ")
-        ds_export_path = os.path.join(export_path, f"{dominio_param}_results.xlsx")
-        reverseds_export_path = os.path.join(export_path, f"{dominio_param}_reverse_results.xlsx")
-        utils.export_xlsx(ds_export_path, dominio_param, df)
+        if reply:
+            while True:
+                max_indice = len(df) - 1
+                index_to_remove = request_and_validate_indices.request_valid_indixes(max_indice)
+
+                if index_to_remove:
+                    df = remove_lines.remove_lines(df, index_to_remove)
+                    print(df.to_string(index=True))
+                else:
+                    print("")
+                    break
 
-    risposta_reverse = utils.richiedi_conferma("Do you want to perform the reverse DNS lookup? (y/n):")
-    print(" ")
+                print(" ")
 
-    if risposta_reverse:
-        ip_colonna = 'CIDR'
+        reply_reverse = request_confirm.request_confirm(
+            "Do you want to perform the reverse DNS lookup? (y/n):")
+        print(" ")
 
-        for indice, riga in df.iterrows():
-            cidr = riga[ip_colonna] 
-            lista_ip = utils.expand_ip_range(cidr)  
-
-            print("***************************")
-            print("Results for "+cidr)
-            dati_ip_dominio = []
+        if reply_reverse:
+            ip_colonna = 'CIDR'
 
-            if not lista_ip:
-                print(f"No IP address found for the CIDR: {cidr}")
-                print(" ")
-                continue
-           
-            domini = []
-            for ip in lista_ip:
-                dominio_locale = utils.reverse_dns(ip) 
-                dominio_ripe = utils.get_ripe_reverse_dns(ip) 
-            
-                if dominio_locale == dominio_ripe or dominio_ripe != "No domain found":
-                    dominio = dominio_ripe
-                elif dominio_locale != "No domain found":
-                    dominio = dominio_locale
-                else:
-                    dominio = "No domain found"
-                
-                if dominio != "No domain found":
-                    dati_ip_dominio.append({'IP': ip, 'Domain': dominio})
-
-            df_subnet = pd.DataFrame(dati_ip_dominio)
-            if not df_subnet.empty:
-                print(df_subnet)
-                risposta = utils.richiedi_conferma("Do you want to export the results to an xslx file? (y/n):")
-                print(" ")
-                if risposta:
-                    cidr_sheet = cidr.replace("/","-")
-                    if os.path.exists(reverseds_export_path):                    
-                        utils.export_xlsx_newsheet(reverseds_export_path, cidr_sheet, df_subnet)
+            for indice, riga in df.iterrows():
+                cidr = riga[ip_colonna]
+                lista_ip = expand_ip_range.expand_ip_range(cidr)
+
+                print("***************************")
+                print("Results for "+cidr)
+                data_ip_domain = []
+
+                if not lista_ip:
+                    print(f"No IP address found for the CIDR: {cidr}")
+                    print(" ")
+                    continue
+
+                for ip in lista_ip:
+                    domain_local = reverse_dns.reverse_dns(ip)
+                    domain_ripe = get_ripe_reverse_dns.get_ripe_reverse_dns(ip)
+
+                    if domain_local == domain_ripe or domain_ripe != "No domain found":
+                        domain = domain_ripe
+                    elif domain_local != "No domain found":
+                        domain = domain_local
                     else:
-                        export_path = utils.get_export_path("Enter the export path for the xslx file (leave blank to use the current directory): ")
-                        reverseds_export_path = os.path.join(export_path, f"{dominio_param}_reverse_results.xlsx")
-                        utils.export_xlsx(reverseds_export_path, cidr_sheet, df_subnet)
-            else:
-                print("No domain found for the IP addresses in this subnet.")
+                        domain = "No domain found"
 
-        print(" ")
-    else:
-        print("Skipping the reverse DNS lookup.")
+                    if domain != "No domain found":
+                        data_ip_domain.append({'IP': ip, 'Domain': domain})
+
+                df_subnet = pd.DataFrame(data_ip_domain)
+                if not df_subnet.empty:
+                    print(df_subnet)
+                    reply = request_confirm.request_confirm(
+                        "Do you want to export the results to an xslx file? (y/n):")
+                    print(" ")
+                    if reply:
+                        cidr_sheet = cidr.replace("/", "-")
+                        if os.path.exists(reverseds_export_path):
+                            export_xlsx_new_sheet.export_xlsx_newsheet(
+                                reverseds_export_path, cidr_sheet, df_subnet)
+                        else:
+                            export_path = get_export_path.get_export_path(
+                                "Enter the export path for the xslx file (leave blank to use the current directory): ")
+                            reverseds_export_path = os.path.join(
+                                export_path, f"{domain_param}_reverse_results.xlsx")
+                            export_xlsx.export_xlsx(
+                                reverseds_export_path, cidr_sheet, df_subnet)
+                else:
+                    print("No domain found for the IP addresses in this subnet.")
+
+            print(" ")
+        else:
+            print("Skipping the reverse DNS lookup.")
 
-    #print("Termine Programma...")
+# Esporta in xlsx
+    reply = request_confirm.request_confirm(
+        "Do you want to export the results to an xslx file? (y/n):")
+    print(" ")
+    if reply:
+        export_path = get_export_path.get_export_path(
+            "Enter the export path for the xslx file (leave blank to use the current directory): ")
+        ds_export_path = os.path.join(
+            export_path, f"{domain_param}_results.xlsx")
+        reverseds_export_path = os.path.join(
+            export_path, f"{domain_param}_reverse_results.xlsx")
+        export_xlsx.export_xlsx(ds_export_path, domain_param, df)   
 
 if __name__ == "__main__":
-    main()
+    main()
```

