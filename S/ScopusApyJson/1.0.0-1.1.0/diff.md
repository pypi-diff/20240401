# Comparing `tmp/ScopusApyJson-1.0.0.tar.gz` & `tmp/ScopusApyJson-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScopusApyJson-1.0.0.tar", last modified: Mon Jan 15 16:47:37 2024, max compression
+gzip compressed data, was "ScopusApyJson-1.1.0.tar", last modified: Mon Apr  1 17:25:54 2024, max compression
```

## Comparing `ScopusApyJson-1.0.0.tar` & `ScopusApyJson-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-01-15 16:47:37.098528 ScopusApyJson-1.0.0/
--rw-rw-rw-   0        0        0     1084 2023-12-30 15:43:10.000000 ScopusApyJson-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       49 2024-01-11 12:58:47.000000 ScopusApyJson-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1533 2024-01-15 16:47:37.098528 ScopusApyJson-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-01-15 11:14:19.000000 ScopusApyJson-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-01-15 16:47:37.047467 ScopusApyJson-1.0.0/ScopusApyJson/
-drwxrwxrwx   0        0        0        0 2024-01-15 16:47:37.080769 ScopusApyJson-1.0.0/ScopusApyJson/CLI/
--rw-rw-rw-   0        0        0       58 2024-01-10 14:11:42.000000 ScopusApyJson-1.0.0/ScopusApyJson/CLI/__init__.py
--rw-rw-rw-   0        0        0     1928 2024-01-14 09:27:22.000000 ScopusApyJson-1.0.0/ScopusApyJson/CLI/cli.py
-drwxrwxrwx   0        0        0        0 2024-01-15 16:47:37.080769 ScopusApyJson-1.0.0/ScopusApyJson/CONFIG/
--rw-rw-rw-   0        0        0      746 2024-01-11 17:46:06.000000 ScopusApyJson-1.0.0/ScopusApyJson/CONFIG/api_scopus_config.json
--rw-rw-rw-   0        0        0     3619 2024-01-15 11:04:46.000000 ScopusApyJson-1.0.0/ScopusApyJson/CONFIG/scopus_col_names.json
--rw-rw-rw-   0        0        0     5280 2024-01-15 11:05:14.000000 ScopusApyJson-1.0.0/ScopusApyJson/GLOBALS.py
--rw-rw-rw-   0        0        0      245 2024-01-14 09:26:02.000000 ScopusApyJson-1.0.0/ScopusApyJson/__init__.py
--rw-rw-rw-   0        0        0     4352 2024-01-15 15:17:11.000000 ScopusApyJson-1.0.0/ScopusApyJson/api_manager.py
--rw-rw-rw-   0        0        0    20585 2024-01-14 18:13:08.000000 ScopusApyJson-1.0.0/ScopusApyJson/json_parser.py
--rw-rw-rw-   0        0        0     3082 2024-01-15 10:14:23.000000 ScopusApyJson-1.0.0/ScopusApyJson/json_utils.py
--rw-rw-rw-   0        0        0     1384 2024-01-15 09:36:30.000000 ScopusApyJson-1.0.0/ScopusApyJson/main.py
-drwxrwxrwx   0        0        0        0 2024-01-15 16:47:37.079537 ScopusApyJson-1.0.0/ScopusApyJson.egg-info/
--rw-rw-rw-   0        0        0     1533 2024-01-15 16:47:36.000000 ScopusApyJson-1.0.0/ScopusApyJson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      563 2024-01-15 16:47:36.000000 ScopusApyJson-1.0.0/ScopusApyJson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-15 16:47:36.000000 ScopusApyJson-1.0.0/ScopusApyJson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2024-01-15 16:47:36.000000 ScopusApyJson-1.0.0/ScopusApyJson.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2024-01-15 16:47:36.000000 ScopusApyJson-1.0.0/ScopusApyJson.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-01-15 16:47:36.000000 ScopusApyJson-1.0.0/ScopusApyJson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-15 16:47:37.098528 ScopusApyJson-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1781 2024-01-15 16:46:19.000000 ScopusApyJson-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:25:54.440580 ScopusApyJson-1.1.0/
+-rw-rw-rw-   0        0        0     1084 2023-12-30 15:43:10.000000 ScopusApyJson-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       49 2024-01-11 12:58:47.000000 ScopusApyJson-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1606 2024-04-01 17:25:54.440580 ScopusApyJson-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      846 2024-04-01 16:53:56.000000 ScopusApyJson-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 17:25:54.357668 ScopusApyJson-1.1.0/ScopusApyJson/
+drwxrwxrwx   0        0        0        0 2024-04-01 17:25:54.422557 ScopusApyJson-1.1.0/ScopusApyJson/CLI/
+-rw-rw-rw-   0        0        0       58 2024-01-10 14:11:42.000000 ScopusApyJson-1.1.0/ScopusApyJson/CLI/__init__.py
+-rw-rw-rw-   0        0        0     1928 2024-01-14 09:27:22.000000 ScopusApyJson-1.1.0/ScopusApyJson/CLI/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:25:54.438735 ScopusApyJson-1.1.0/ScopusApyJson/CONFIG/
+-rw-rw-rw-   0        0        0      746 2024-01-11 17:46:06.000000 ScopusApyJson-1.1.0/ScopusApyJson/CONFIG/api_scopus_config.json
+-rw-rw-rw-   0        0        0     3619 2024-01-15 11:04:46.000000 ScopusApyJson-1.1.0/ScopusApyJson/CONFIG/scopus_col_names.json
+-rw-rw-rw-   0        0        0     5300 2024-03-31 04:34:45.000000 ScopusApyJson-1.1.0/ScopusApyJson/GLOBALS.py
+-rw-rw-rw-   0        0        0      245 2024-01-14 09:26:02.000000 ScopusApyJson-1.1.0/ScopusApyJson/__init__.py
+-rw-rw-rw-   0        0        0     4521 2024-04-01 14:15:10.000000 ScopusApyJson-1.1.0/ScopusApyJson/api_manager.py
+-rw-rw-rw-   0        0        0    23840 2024-03-31 18:24:44.000000 ScopusApyJson-1.1.0/ScopusApyJson/json_parser.py
+-rw-rw-rw-   0        0        0     3082 2024-01-15 10:14:23.000000 ScopusApyJson-1.1.0/ScopusApyJson/json_utils.py
+-rw-rw-rw-   0        0        0     1986 2024-04-01 17:09:55.000000 ScopusApyJson-1.1.0/ScopusApyJson/main.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:25:54.403505 ScopusApyJson-1.1.0/ScopusApyJson.egg-info/
+-rw-rw-rw-   0        0        0     1606 2024-04-01 17:25:53.000000 ScopusApyJson-1.1.0/ScopusApyJson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      563 2024-04-01 17:25:53.000000 ScopusApyJson-1.1.0/ScopusApyJson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 17:25:53.000000 ScopusApyJson-1.1.0/ScopusApyJson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2024-04-01 17:25:53.000000 ScopusApyJson-1.1.0/ScopusApyJson.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2024-04-01 17:25:53.000000 ScopusApyJson-1.1.0/ScopusApyJson.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-01 17:25:53.000000 ScopusApyJson-1.1.0/ScopusApyJson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 17:25:54.453670 ScopusApyJson-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1781 2024-04-01 16:52:48.000000 ScopusApyJson-1.1.0/setup.py
```

### Comparing `ScopusApyJson-1.0.0/LICENSE` & `ScopusApyJson-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ScopusApyJson-1.0.0/PKG-INFO` & `ScopusApyJson-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScopusApyJson
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python modules for parsing the response to a Scopus API request
 Home-page: https://github.com/TickyWill/ScopusApyJson
 Author: BiblioAnalysis team
 Author-email: francois.bertin7@wanadoo.fr, amal.chabli@orange.fr
 License: MIT
 Keywords: Metadata parsing,Scopus request,API management
 Platform: UNKNOWN
@@ -35,16 +35,17 @@
 scopus_df = saj.build_scopus_df_from_api(doi_list)
 scopus_df.to_excel(<your_fullpath_file.xlsx), index = False)
 ```
 **for more exemples refer to** [ScopusApyJson-exemples](https://github.com/TickyWill/ScopusApyJson/Demo_ScopusApyJson.ipynb).
 
 
 # Release History
-1.0.0 first release
+- 1.0.0 first release
+- 1.1.0 check of fields availability when parsing the request response
 
 
 # Meta
-	- authors : BiblioAbnalysis team
+	- authors : BiblioAnalysis team
 
 Distributed under the [MIT license](https://mit-license.org/)
```

### Comparing `ScopusApyJson-1.0.0/README.md` & `ScopusApyJson-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 scopus_df = saj.build_scopus_df_from_api(doi_list)
 scopus_df.to_excel(<your_fullpath_file.xlsx), index = False)
 ```
 **for more exemples refer to** [ScopusApyJson-exemples](https://github.com/TickyWill/ScopusApyJson/Demo_ScopusApyJson.ipynb).
 
 
 # Release History
-1.0.0 first release
+- 1.0.0 first release
+- 1.1.0 check of fields availability when parsing the request response
 
 
 # Meta
-	- authors : BiblioAbnalysis team
+	- authors : BiblioAnalysis team
 
 Distributed under the [MIT license](https://mit-license.org/)
```

### Comparing `ScopusApyJson-1.0.0/ScopusApyJson/CLI/cli.py` & `ScopusApyJson-1.1.0/ScopusApyJson/CLI/cli.py`

 * *Files identical despite different names*

### Comparing `ScopusApyJson-1.0.0/ScopusApyJson/CONFIG/api_scopus_config.json` & `ScopusApyJson-1.1.0/ScopusApyJson/CONFIG/api_scopus_config.json`

 * *Files identical despite different names*

### Comparing `ScopusApyJson-1.0.0/ScopusApyJson/CONFIG/scopus_col_names.json` & `ScopusApyJson-1.1.0/ScopusApyJson/CONFIG/scopus_col_names.json`

 * *Files identical despite different names*

### Comparing `ScopusApyJson-1.0.0/ScopusApyJson/GLOBALS.py` & `ScopusApyJson-1.1.0/ScopusApyJson/GLOBALS.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     
 def _check_api_keys(API_CONFIG_DICT):
     # Standard library imports
     import warnings
       
     dict_apikey    = API_CONFIG_DICT["apikey"]
     dict_insttoken = API_CONFIG_DICT["insttoken"]
-    if (dict_apikey ==  "PAST_APIKEY_HERE") or (dict_insttoken == "PAST_INSTTOKEN_HERE"):
+    if (dict_apikey in  ["PAST_APIKEY_HERE", ""]) or (dict_insttoken in ["PAST_INSTTOKEN_HERE", ""]):
         message  = "Authentication keys are not yet defined (required).\n"
         warnings.warn(message)
         API_CONFIG_DICT["apikey"]    = input("Enter your authentication key (obtained from http://dev.elsevier.com):")
         API_CONFIG_DICT["insttoken"] = input("your institution token provided by Elsevier support staff:")
         _dump_json(API_CONFIG_PATH, API_CONFIG_DICT)     
 
 def _config_ScopusApyJson_dict(json_file_name):
@@ -106,10 +106,10 @@
 # stored in the folder ".ScopusApyJson/CONFIG"
 API_CONFIG_DICT, API_CONFIG_PATH = _config_ScopusApyJson_dict('api_scopus_config.json')
 _check_api_keys(API_CONFIG_DICT)
 
 # Getting the names of the selected scopus columns by the user through the json file "scopus_col_names.json" 
 # stored in the folder ""~/AppData/Roaming/ScopusApyJson" of vthe user
 scopus_column_names_dict, _   = _config_ScopusApyJson_dict('scopus_col_names.json')
-PARSED_SCOPUS_COLUMNS_NAMES   = list(scopus_column_names_dict.keys())
-SELECTED_SCOPUS_COLUMNS_NAMES = [k for k,v in scopus_column_names_dict.items() if v] 
+PARSED_SCOPUS_COLUMNS_NAMES   = list(scopus_column_names_dict.keys())[1:]
+SELECTED_SCOPUS_COLUMNS_NAMES = [k for k,v in scopus_column_names_dict.items() if v][1:]
```

### Comparing `ScopusApyJson-1.0.0/ScopusApyJson/api_manager.py` & `ScopusApyJson-1.1.0/ScopusApyJson/api_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,40 +54,42 @@
     import requests
     from requests.exceptions import Timeout
     
     # Setting client authentication keys
     MyScopusKey = api_config_dict["apikey"]
     MyInstKey   = api_config_dict["insttoken"]
     api_uses_nb = api_config_dict['api_uses_nb']
+    if (MyScopusKey in  ["PAST_APIKEY_HERE", ""]) or (MyInstKey in ["PAST_INSTTOKEN_HERE", ""]):
+        response_status = "Wrong authentication"
 
     # Setting Elsevier API
     els_api = _set_els_doi_api(MyScopusKey, MyInstKey, doi)
     
     # Initializing parameters
     response_dict = None
 
     # Get the request response
     try:
         response = requests.get(els_api, timeout = 10)   
     except Timeout:
-        print('The request timed out')
+        response_status = "Timeout"
     else:
-        if response == False: # response.status_code <200 or > 400
-            print('Resource not found')
+        if response == False: # response.status_code <200
+            response_status = "False"
         else:
-            print(f'Resquest successful for DOI {doi}')
-            if response.status_code == 204:
-                print('No content')
-            else:            
+            if response.status_code in [204, 404]:
+                response_status = "Empty"
+            else:
+                response_status = "True"
                 response_dict = response.json()
                 
         # Updating api_uses_nb in config_dict
         api_config_dict["api_uses_nb"] = api_uses_nb + 1
     
-    return (response_dict, api_config_dict)
+    return (response_dict, api_config_dict, response_status)
 
 
 def _update_api_config_json(API_CONFIG_PATH, API_CONFIG_DICT):
     # Standard library imports
     import json
     
     with open(API_CONFIG_PATH, 'w') as f:
@@ -111,13 +113,13 @@
     """ 
     
     # Globals imports
     from ScopusApyJson.GLOBALS import API_CONFIG_DICT
     from ScopusApyJson.GLOBALS import API_CONFIG_PATH
     
     # Getting api json data
-    doi_json_data, API_CONFIG_DICT = _get_json_from_api(doi, API_CONFIG_DICT)
+    doi_json_data, API_CONFIG_DICT, request_status = _get_json_from_api(doi, API_CONFIG_DICT)
     
     # Updatting api config json with number of requests
     _update_api_config_json(API_CONFIG_PATH, API_CONFIG_DICT)
     
-    return doi_json_data
+    return (doi_json_data, request_status)
```

### Comparing `ScopusApyJson-1.0.0/ScopusApyJson/json_parser.py` & `ScopusApyJson-1.1.0/ScopusApyJson/json_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,316 +2,341 @@
 
     
 def _built_date(dic, key):
     # Standard library imports
     import calendar
     
     # Local library imports
+    from ScopusApyJson.json_utils import check_not_none
     from ScopusApyJson.json_utils import check_true_to_append
     from ScopusApyJson.json_utils import get_json_key_value
         
     dateitems = get_json_key_value(dic, key)
-    dateitems_list = []  
-    dateitems_list = check_true_to_append(dateitems, '@day', dateitems_list)
-    item_num  = 0
-    dateitems_list = check_true_to_append(dateitems, '@month', dateitems_list)
-    item_num += 1
-    month_num = int(dateitems_list[item_num])
-    dateitems_list[item_num] = calendar.month_name[month_num]
-    dateitems_list = check_true_to_append(dateitems, '@year', dateitems_list)
-    date = " ".join(dateitems_list)
-    
-    return date
+    if check_not_none(dateitems):
+        dateitems_list = []  
+        dateitems_list = check_true_to_append(dateitems, '@day', dateitems_list)
+        item_num  = 0
+        dateitems_list = check_true_to_append(dateitems, '@month', dateitems_list)
+        item_num += 1
+        month_num = int(dateitems_list[item_num])
+        dateitems_list[item_num] = calendar.month_name[month_num]
+        dateitems_list = check_true_to_append(dateitems, '@year', dateitems_list)
+        date = " ".join(dateitems_list)
+
+        return date
 
 
 def _parse_source_info(json_data, article_dic):
     '''Parse the field "source" under the top 
     "field asbtracts-retrieval-response/item/bibrecord/head".
     '''
     
     # Local library imports
     from ScopusApyJson.json_utils import check_not_none
     from ScopusApyJson.json_utils import check_true_to_append
     from ScopusApyJson.json_utils import check_true_to_set
     from ScopusApyJson.json_utils import get_json_key_value
     
-    source_dict                             = get_json_key_value(json_data, "source")
-    article_dic['Year']                     = get_json_key_value(source_dict, "year")
-    article_dic['Source title']             = get_json_key_value(source_dict, 'sourcetitle')
-    article_dic['Abbreviated Source Title'] = get_json_key_value(source_dict, 'sourcetitle-abbrev')
-    article_dic['CODEN']                    = get_json_key_value(source_dict, 'codencode')
-    
-    # Parsing issn
-    issn_info = get_json_key_value(source_dict, 'issn')
-    if check_not_none(issn_info):
-        if not isinstance(issn_info, list):
-            article_dic['ISSN'] = get_json_key_value(issn_info, '$')
-        else:    
-            for issn_dict in issn_info:
-                issn_type = get_json_key_value(issn_dict, '@type')
-                if issn_type == "print": article_dic['ISSN'] = get_json_key_value(issn_dict, '$')
-
-    #Parsing isbn if available  
-    isbn_info = get_json_key_value(source_dict, 'isbn')
-    if check_not_none(isbn_info):
-        if not isinstance(isbn_info, list):
-            article_dic['ISBN'] = get_json_key_value(isbn_info, '$')            
+    source_dict = get_json_key_value(json_data, "source")
+    if check_not_none(source_dict):
+        article_dic['Year']                     = get_json_key_value(source_dict, "year")
+        article_dic['Source title']             = get_json_key_value(source_dict, 'sourcetitle')
+        article_dic['Abbreviated Source Title'] = get_json_key_value(source_dict, 'sourcetitle-abbrev')
+        article_dic['CODEN']                    = get_json_key_value(source_dict, 'codencode')
+
+        # Parsing issn
+        issn_info = get_json_key_value(source_dict, 'issn')
+        if check_not_none(issn_info):
+            if not isinstance(issn_info, list):
+                article_dic['ISSN'] = get_json_key_value(issn_info, '$')
+            else:    
+                for issn_dict in issn_info:
+                    issn_type = get_json_key_value(issn_dict, '@type')
+                    if issn_type == "print": article_dic['ISSN'] = get_json_key_value(issn_dict, '$')
+
+        #Parsing isbn if available  
+        isbn_info = get_json_key_value(source_dict, 'isbn')
+        if check_not_none(isbn_info):
+            if not isinstance(isbn_info, list):
+                article_dic['ISBN'] = get_json_key_value(isbn_info, '$')            
+            else:
+                for isbn_dict in isbn_info:
+                    isbn_type = get_json_key_value(isbn_dict, '@type')
+                    if isbn_type == "print": article_dic['ISBN'] = get_json_key_value(isbn_dict, '$')
+
+        # Parsing conference info if available
+        conference_info = get_json_key_value(source_dict, 'additional-srcinfo')
+        if check_not_none(conference_info):
+            conferenceinfo = get_json_key_value(conference_info, 'conferenceinfo')
+            if check_not_none(conferenceinfo):
+                confevent = get_json_key_value(conferenceinfo, 'confevent')
+                if check_not_none(confevent):
+                    article_dic['Conference name'] = get_json_key_value(confevent, 'confname')                
+                    article_dic['Conference code'] = get_json_key_value(confevent, 'confcode')
+                    conflocation = get_json_key_value(confevent, 'conflocation')
+                    if check_not_none(conflocation): 
+                        article_dic['Conference location'] = get_json_key_value(conflocation, 'city')
+                    confdates = get_json_key_value(confevent, 'confdate')
+                    if check_not_none(confdates):
+                        start_date = _built_date(confdates, 'startdate')
+                        end_date   = _built_date(confdates, 'enddate')                   
+                        article_dic['Conference date'] = start_date + " through " + end_date        
+
+        # Parsing volisspag if available          
+        article_dic = check_true_to_set(source_dict, 'article-number', article_dic, 'Art. No.')
+        volisspag   = get_json_key_value(source_dict, "volisspag")
+        if check_not_none(volisspag):
+            voliss      = get_json_key_value(volisspag, "voliss")
+            article_dic = check_true_to_set(voliss, '@volume', article_dic, 'Volume')
+            article_dic = check_true_to_set(voliss, '@issue', article_dic, 'Issue')
+            pagerange   = get_json_key_value(volisspag, "pagerange")
+            if check_not_none(pagerange): 
+                article_dic['Page start'] = get_json_key_value(pagerange, '@first')
+                article_dic['Page end']   = get_json_key_value(pagerange, '@last')
+                article_dic['Page count'] = str(int(article_dic['Page end']) - int(article_dic['Page start']))
+
+        # Parsing publication stage
+        stage_info  = get_json_key_value(source_dict, 'publicationdate')
+        if "month" in stage_info.keys(): 
+            article_dic['Publication Stage'] = "Final" 
         else:
-            for isbn_dict in isbn_info:
-                isbn_type = get_json_key_value(isbn_dict, '@type')
-                if isbn_type == "print": article_dic['ISBN'] = get_json_key_value(isbn_dict, '$')
-                
-    # Parsing conference info if available
-    conference_info = get_json_key_value(source_dict, 'additional-srcinfo')
-    if check_not_none(conference_info):
-        conferenceinfo = get_json_key_value(conference_info, 'conferenceinfo')
-        if check_not_none(conferenceinfo):
-            confevent = get_json_key_value(conferenceinfo, 'confevent')
-            if check_not_none(confevent):
-                article_dic['Conference name'] = get_json_key_value(confevent, 'confname')                
-                article_dic['Conference code'] = get_json_key_value(confevent, 'confcode')
-                conflocation = get_json_key_value(confevent, 'conflocation')
-                if check_not_none(conflocation): 
-                    article_dic['Conference location'] = get_json_key_value(conflocation, 'city')
-                confdates = get_json_key_value(confevent, 'confdate')
-                if check_not_none(confdates):
-                    start_date = _built_date(confdates, 'startdate')
-                    end_date   = _built_date(confdates, 'enddate')                   
-                    article_dic['Conference date'] = start_date + " through " + end_date        
-    
-    # Parsing volisspag if available          
-    article_dic = check_true_to_set(source_dict, 'article-number', article_dic, 'Art. No.')
-    volisspag   = get_json_key_value(source_dict, "volisspag")
-    if check_not_none(volisspag):
-        voliss      = get_json_key_value(volisspag, "voliss")
-        article_dic = check_true_to_set(voliss, '@volume', article_dic, 'Volume')
-        article_dic = check_true_to_set(voliss, '@issue', article_dic, 'Issue')
-        pagerange   = get_json_key_value(volisspag, "pagerange")
-        if check_not_none(pagerange): 
-            article_dic['Page start'] = get_json_key_value(pagerange, '@first')
-            article_dic['Page end']   = get_json_key_value(pagerange, '@last')
-            article_dic['Page count'] = str(int(article_dic['Page end']) - int(article_dic['Page start']))
-    
-    # Parsing publication stage
-    stage_info  = get_json_key_value(source_dict, 'publicationdate')
-    if "month" in stage_info.keys(): 
-        article_dic['Publication Stage'] = "Final" 
-    else:
-        article_dic['Publication Stage'] = "Article in press"
+            article_dic['Publication Stage'] = "Article in press"
 
         
 def _parse_citation_info(json_data, article_dic):
     '''Parse the field "citation-info" under the top field 
     "asbtracts-retrieval-response/item/bibrecord/head".
     '''
     # Local library imports
     from ScopusApyJson.json_utils import check_not_none
     from ScopusApyJson.json_utils import get_json_key_value
     
     citation_info = get_json_key_value(json_data, 'citation-info')
-    language_dict = get_json_key_value(citation_info, 'citation-language')
-    if check_not_none(language_dict): 
-        article_dic['Language of Original Document'] = get_json_key_value(language_dict, '@language')
+    if check_not_none(citation_info):
+        language_dict = get_json_key_value(citation_info, 'citation-language')
+        if check_not_none(language_dict): 
+            article_dic['Language of Original Document'] = get_json_key_value(language_dict, '@language')
 
     
 def _parse_ordered_authors(json_data, article_dic):
     '''Parse the field "author" under the top field 
     "astracts-retrieval-response/authors".
     The field "author" is a dict if there is only 
     one author otherwise it is a list of dict.
     '''
     
     # Local library imports
+    from ScopusApyJson.json_utils import check_not_none
     from ScopusApyJson.json_utils import get_json_key_value
     
     authors            = []
     authors_ids        = []
     authors_full_names = []
     
     auths_field = get_json_key_value(json_data, "authors")
-    auths_group = get_json_key_value(auths_field, "author")
-    if not isinstance(auths_group, list) : auths_group = [auths_group]
+    if check_not_none(auths_field):
+        auths_group = get_json_key_value(auths_field, "author")
+        if check_not_none(auths_group):
+            if not isinstance(auths_group, list) : auths_group = [auths_group]
+            for auths in auths_group:                
+                auth_preferred_name = get_json_key_value(auths, 'preferred-name')
+                if check_not_none(auth_preferred_name):
+                    auth_id         = get_json_key_value(auths, '@auid')
+                    auth_name       = get_json_key_value(auth_preferred_name, 'ce:indexed-name')
+                    auth_surname    = get_json_key_value(auth_preferred_name, 'ce:surname')
+                    auth_given_name = get_json_key_value(auth_preferred_name, 'ce:given-name')
+                    
+                    authors_ids.append(auth_id)
+                    authors.append(auth_name)                
+                    authors_full_names.append(f'{auth_surname}, {auth_given_name} ({auth_id})')
+
+            article_dic['Authors']           = '; '.join(authors)
+            article_dic['Author(s) ID']      = '; '.join(authors_ids)
+            article_dic['Author full names'] = '; '.join(authors_full_names)
         
-    for auths in auths_group:
-        auth_id             = get_json_key_value(auths, '@auid')
-        auth_preferred_name = get_json_key_value(auths, 'preferred-name')
-        auth_name           = get_json_key_value(auth_preferred_name, 'ce:indexed-name')
-        auth_surname        = get_json_key_value(auth_preferred_name, 'ce:surname')
-        auth_given_name     = get_json_key_value(auth_preferred_name, 'ce:given-name')
-                
-        authors.append(auth_name)
-        authors_ids.append(auth_id)
-        authors_full_names.append(f'{auth_surname}, {auth_given_name} ({auth_id})')
-
-    article_dic['Authors']           = '; '.join(authors)
-    article_dic['Author(s) ID']      = '; '.join(authors_ids)
-    article_dic['Author full names'] = '; '.join(authors_full_names)
-    
     
 def _parse_authors_affiliations(json_data, article_dic):
     '''Parse the field "author-group" under the top field 
     "abstracts-retrieval-response/item/bibrecord/head".
     The field "author-group" is a dict if there is only one author, 
     otherwise it is a list of dict .
     '''
     
     # Standard library imports
     from collections import defaultdict
     
     # Local library imports
+    from ScopusApyJson.json_utils import check_not_none
     from ScopusApyJson.json_utils import check_true_to_append
     from ScopusApyJson.json_utils import get_json_key_value
     
-    authors_with_affiliations_dict = defaultdict(list)
-    authors_with_affiliations_list = []
-    affiliations_list              = []
-    ordered_authors                = article_dic['Authors'].split('; ')
-    
     affiliations_group = get_json_key_value(json_data, 'author-group')
-    if not isinstance(affiliations_group, list) : affiliations_group = [affiliations_group]
-        
-    for affiliation_dict in affiliations_group:
-        affiliation = get_json_key_value(affiliation_dict, 'affiliation')
+    if check_not_none(affiliations_group):
     
-        # Building affiliation full address
-        organizations_list = get_json_key_value(affiliation, 'organization')
-        if not isinstance(organizations_list, list) : organizations_list = [organizations_list]
-        address_items_list = []
-        for organization_dict in organizations_list:
-            address_items_list.append(get_json_key_value(organization_dict, '$'))        
-        address_items_list = check_true_to_append(affiliation, 'address-part', address_items_list)
-        address_items_list = check_true_to_append(affiliation, 'city', address_items_list)
-        address_items_list = check_true_to_append(affiliation, 'postal-code', address_items_list)
-        address_items_list = check_true_to_append(affiliation, 'country', address_items_list)
-        affiliation_address = ', '.join(address_items_list)
-      
-        # Appending "affiliation_address" to "affiliations_list"
-        affiliations_list.append(affiliation_address)
-        
-        # Appending "affiliation_address" to "authors_with_affiliations_dict" for each author of the "affiliation_authors_list"
-        affiliation_authors_list = get_json_key_value(affiliation_dict, 'author')
-        if not isinstance(affiliation_authors_list, list) : affiliation_authors_list = [affiliation_authors_list]
-        for author in affiliation_authors_list:
-            author_preferred_name = get_json_key_value(author, 'preferred-name')
-            author_name           = get_json_key_value(author_preferred_name, 'ce:indexed-name')
-            authors_with_affiliations_dict[author_name].append(affiliation_address)
-            
-    # Ordering the "authors_with_affiliations_list" in the order of the "ordered_authors"
-    for author in ordered_authors:
-        author_affiliations_list = authors_with_affiliations_dict[author]
-        authors_with_affiliations_list.append(f"{author}, {', '.join(author_affiliations_list)}")        
+        authors_with_affiliations_dict = defaultdict(list)
+        authors_with_affiliations_list = []
+        affiliations_list              = []
+        ordered_authors                = article_dic['Authors'].split('; ')
+        
+        if not isinstance(affiliations_group, list) : affiliations_group = [affiliations_group]
+
+        for affiliation_dict in affiliations_group:
+            affiliation = get_json_key_value(affiliation_dict, 'affiliation')
+
+            # Building affiliation full address
+            organizations_list = get_json_key_value(affiliation, 'organization')
+            if not isinstance(organizations_list, list) : organizations_list = [organizations_list]
+            address_items_list = []
+            for organization_dict in organizations_list:
+                address_items_list.append(get_json_key_value(organization_dict, '$'))        
+            address_items_list = check_true_to_append(affiliation, 'address-part', address_items_list)
+            address_items_list = check_true_to_append(affiliation, 'city', address_items_list)
+            address_items_list = check_true_to_append(affiliation, 'postal-code', address_items_list)
+            address_items_list = check_true_to_append(affiliation, 'country', address_items_list)
+            affiliation_address = ', '.join(address_items_list)
+
+            # Appending "affiliation_address" to "affiliations_list"
+            affiliations_list.append(affiliation_address)
+
+            # Appending "affiliation_address" to "authors_with_affiliations_dict" for each author of the "affiliation_authors_list"
+            affiliation_authors_list = get_json_key_value(affiliation_dict, 'author')
+            if not isinstance(affiliation_authors_list, list) : affiliation_authors_list = [affiliation_authors_list]
+            for author in affiliation_authors_list:
+                author_preferred_name = get_json_key_value(author, 'preferred-name')
+                author_name           = get_json_key_value(author_preferred_name, 'ce:indexed-name')
+                authors_with_affiliations_dict[author_name].append(affiliation_address)
+
+        # Ordering the "authors_with_affiliations_list" in the order of the "ordered_authors"
+        for author in ordered_authors:
+            author_affiliations_list = authors_with_affiliations_dict[author]
+            authors_with_affiliations_list.append(f"{author}, {', '.join(author_affiliations_list)}")        
 
-    article_dic['Authors with affiliations'] = '; '.join(authors_with_affiliations_list)
-    article_dic['Affiliations']              = '; '.join(affiliations_list)
+        article_dic['Authors with affiliations'] = '; '.join(authors_with_affiliations_list)
+        article_dic['Affiliations']              = '; '.join(affiliations_list)
 
     
 def _parse_correspondence_address(json_data, article_dic):
     '''Parse the field "correspondence" under the top field 
     "abstracts-retrieval-response/item/bibrecord/head".
     The field "correspondence" is a dict if there is only one corresponding person, 
     otherwise it is a list of dict.
     '''
     # Local library imports
+    from ScopusApyJson.json_utils import check_not_none
     from ScopusApyJson.json_utils import check_true_to_append
     from ScopusApyJson.json_utils import get_json_key_value    
-    
-    person_address_list = []
-    
-    correspondence_list = get_json_key_value(json_data, 'correspondence')   
-    if not isinstance(correspondence_list, list) : correspondence_list = [correspondence_list]
-    for correspondence_dict in correspondence_list:        
-        correspondence_person_dict = get_json_key_value(correspondence_dict, 'person')
-        correspondence_person      = get_json_key_value(correspondence_person_dict, 'ce:indexed-name')
-               
-        # Building affiliation full address
-        affiliation = get_json_key_value(correspondence_dict, 'affiliation')
-        organizations_list = get_json_key_value(affiliation, 'organization')
-        if not isinstance(organizations_list, list) : organizations_list = [organizations_list]
-        address_items_list = []
-        for organization_dict in organizations_list:
-            address_items_list.append(get_json_key_value(organization_dict, '$'))
-        address_items_list = check_true_to_append(affiliation, 'address-part', address_items_list)
-        address_items_list = check_true_to_append(affiliation, 'city', address_items_list)
-        address_items_list = check_true_to_append(affiliation, 'postal-code', address_items_list)
-        address_items_list = check_true_to_append(affiliation, 'country', address_items_list)
-        correspondence_address = ', '.join(address_items_list)
-        
-        person_address_list.append(correspondence_person + "; " + correspondence_address)
-        
-    article_dic['Correspondence Address'] = '; '.join(person_address_list)
+
+    correspondence_list = get_json_key_value(json_data, 'correspondence')
+    if check_not_none(correspondence_list):
+        person_address_list = []
+        if not isinstance(correspondence_list, list) : correspondence_list = [correspondence_list]
+        for correspondence_dict in correspondence_list:        
+            correspondence_person_dict = get_json_key_value(correspondence_dict, 'person')
+            if check_not_none(correspondence_person_dict):
+                correspondence_person = get_json_key_value(correspondence_person_dict, 'ce:indexed-name')
+
+            # Building affiliation full address
+            affiliation = get_json_key_value(correspondence_dict, 'affiliation')
+            if check_not_none(affiliation):
+                organizations_list = get_json_key_value(affiliation, 'organization')
+                if not isinstance(organizations_list, list) : organizations_list = [organizations_list]
+                address_items_list = []
+                for organization_dict in organizations_list:
+                    address_items_list.append(get_json_key_value(organization_dict, '$'))
+                address_items_list = check_true_to_append(affiliation, 'address-part', address_items_list)
+                address_items_list = check_true_to_append(affiliation, 'city', address_items_list)
+                address_items_list = check_true_to_append(affiliation, 'postal-code', address_items_list)
+                address_items_list = check_true_to_append(affiliation, 'country', address_items_list)
+                correspondence_address = ', '.join(address_items_list)
+
+            person_address_list.append(correspondence_person + "; " + correspondence_address)
+
+        article_dic['Correspondence Address'] = '; '.join(person_address_list)
 
     
 def _parse_references(json_data, article_dic):
     '''Parse the field "bibliography" under the top field 
     "abstracts-retrieval-response/item/bibrecord/tail".
     The field "bibliography" is a dict keyyed by "$" if it is not None.
     '''
     # Local library imports
     from ScopusApyJson.json_utils import check_not_none
-    from ScopusApyJson.json_utils import get_json_key_value
+    from ScopusApyJson.json_utils import get_json_key_value   
     
-    ref_text_list = []
-    tail             = get_json_key_value(json_data, 'tail')
-    bibliography     = get_json_key_value(tail, 'bibliography')
-    references_list  = get_json_key_value(bibliography, 'reference')
-    if not isinstance(references_list, list): references_list = [references_list]
-
-    for ref_dict in references_list:
-        ref_item_list = []
-        
-        ref_info    = get_json_key_value(ref_dict, 'ref-info')
-        ref_authors = get_json_key_value(ref_info, 'ref-authors')
-        author_dict = get_json_key_value(ref_authors, 'author')
-        et_al       = ""
-        if isinstance(author_dict, list): 
-            author_dict = author_dict[0]
-            et_al       = " et al."
-        author_name = get_json_key_value(author_dict, 'ce:indexed-name')
-        if check_not_none(author_name):
-            authors     = author_name + et_al                
-            ref_item_list.append(authors)
-
-        ref_title = get_json_key_value(ref_info, 'ref-title')
-        title     = get_json_key_value(ref_title, 'ref-titletext')
-        if check_not_none(title): ref_item_list.append(title)
-
-        source = get_json_key_value(ref_info, 'ref-sourcetitle')
-        if check_not_none(source): ref_item_list.append(source)
-
-        ref_volisspag = get_json_key_value(ref_info, 'ref-volisspag')
-        voliss        = get_json_key_value(ref_volisspag, 'voliss')
-        volume        = get_json_key_value(voliss, '@volume')
-        issue         = get_json_key_value(voliss, '@issue')
-        pagerange     = get_json_key_value(ref_volisspag, 'pagerange')
-        page_first    = get_json_key_value(pagerange, '@first')
-        page_last     = get_json_key_value(pagerange, '@last')
-        if check_not_none(volume): ref_item_list.append(volume)        
-        if check_not_none(issue): ref_item_list.append(issue)
-        if check_not_none(page_first) and check_not_none(page_last): 
-            ref_item_list.append('pp. ' + page_first + '-' + page_last)
-
-        ref_publicationyear = get_json_key_value(ref_info, 'ref-publicationyear')
-        year                = get_json_key_value(ref_publicationyear, '@first')
-        if check_not_none(year): ref_item_list.append("(" + year + ")")
-
-        refd_itemidlist = get_json_key_value(ref_info, 'refd-itemidlist')
-        itemid_list     = get_json_key_value(refd_itemidlist, 'itemid')
-        if not isinstance(itemid_list, list): itemid_list = [itemid_list]
-        doi = None
-        for itemid_dict in itemid_list:
-            itemid_type = get_json_key_value(itemid_dict, '@idtype')            
-            if itemid_type == "DOI": doi = get_json_key_value(itemid_dict, '$')
-        if check_not_none(doi): ref_item_list.append(doi)
-        
-        ref_text = get_json_key_value(ref_info, 'ref-text')
-        if check_not_none(ref_text): ref_item_list.append(ref_text)
-
-        full_ref = ', '.join(ref_item_list)
-        ref_text_list.append(full_ref)
-    article_dic['References'] = '; '.join(ref_text_list)            
+    tail = get_json_key_value(json_data, 'tail')
+    if check_not_none(tail):
+        bibliography     = get_json_key_value(tail, 'bibliography')
+        if check_not_none(bibliography):
+            references_list  = get_json_key_value(bibliography, 'reference')
+            if check_not_none(references_list):
+                if not isinstance(references_list, list): references_list = [references_list]
+                ref_text_list = []
+                for ref_dict in references_list:
+                    if check_not_none(ref_dict):
+                        ref_info = get_json_key_value(ref_dict, 'ref-info')                        
+                        if check_not_none(ref_info):
+                            ref_item_list = []
+                            ref_authors = get_json_key_value(ref_info, 'ref-authors')
+                            if check_not_none(ref_authors):
+                                author_dict = get_json_key_value(ref_authors, 'author')
+                                if check_not_none(author_dict):
+                                    et_al = ""
+                                    if isinstance(author_dict, list): 
+                                        author_dict = author_dict[0]
+                                        et_al = " et al."
+                                    author_name = get_json_key_value(author_dict, 'ce:indexed-name')
+                                    if check_not_none(author_name):
+                                        authors = author_name + et_al                
+                                        ref_item_list.append(authors)
+
+                            ref_title = get_json_key_value(ref_info, 'ref-title')
+                            if check_not_none(ref_title):
+                                title = get_json_key_value(ref_title, 'ref-titletext')
+                                if check_not_none(title): ref_item_list.append(title)
+
+                            source = get_json_key_value(ref_info, 'ref-sourcetitle')
+                            if check_not_none(source): ref_item_list.append(source)
+
+                            ref_volisspag = get_json_key_value(ref_info, 'ref-volisspag')
+                            if check_not_none(ref_volisspag):    
+                                voliss = get_json_key_value(ref_volisspag, 'voliss')
+                                if check_not_none(voliss):
+                                    volume = get_json_key_value(voliss, '@volume')
+                                    issue  = get_json_key_value(voliss, '@issue')
+                                    if check_not_none(volume): ref_item_list.append(volume)        
+                                    if check_not_none(issue): ref_item_list.append(issue)
+                                pagerange = get_json_key_value(ref_volisspag, 'pagerange')
+                                if check_not_none(pagerange):
+                                    page_first = get_json_key_value(pagerange, '@first')
+                                    page_last  = get_json_key_value(pagerange, '@last')
+                                    if check_not_none(page_first) and check_not_none(page_last): 
+                                        ref_item_list.append('pp. ' + page_first + '-' + page_last)
+
+                            ref_publicationyear = get_json_key_value(ref_info, 'ref-publicationyear')
+                            if check_not_none(ref_publicationyear):
+                                year = get_json_key_value(ref_publicationyear, '@first')
+                                if check_not_none(year): ref_item_list.append("(" + year + ")")
+
+                            refd_itemidlist = get_json_key_value(ref_info, 'refd-itemidlist')
+                            if check_not_none(refd_itemidlist):
+                                itemid_list = get_json_key_value(refd_itemidlist, 'itemid')
+                                if check_not_none(itemid_list):
+                                    if not isinstance(itemid_list, list): itemid_list = [itemid_list]
+                                    doi = None
+                                    for itemid_dict in itemid_list:
+                                        itemid_type = get_json_key_value(itemid_dict, '@idtype') 
+                                        if itemid_type == "DOI": doi = get_json_key_value(itemid_dict, '$')
+                                    if check_not_none(doi): ref_item_list.append(doi)
+
+                            ref_text = get_json_key_value(ref_info, 'ref-text')
+                            if check_not_none(ref_text): ref_item_list.append(ref_text)
+
+                            full_ref = ', '.join(ref_item_list)
+                            ref_text_list.append(full_ref)
+                        article_dic['References'] = '; '.join(ref_text_list)            
 
         
 def _parse_index_keywords(json_data, article_dic):
     '''Parse the field "idxterms" under the top field "abstracts-retrieval-response".
     The field "idxterms" is a dict keyyed by "$" if it is not None.
     '''
     # Local library imports
@@ -341,43 +366,46 @@
             article_dic['Author Keywords'] = '; '.join([x['$'] for x in author_keywords_list])   
 
 
 def _parse_coredata(json_data, article_dic):
     '''Parse the field "coredata" under the top field "abstracts-retrieval-response".
     '''
     # Local library imports
+    from ScopusApyJson.json_utils import check_not_none
     from ScopusApyJson.json_utils import get_json_key_value
     
-    coredata_dict                = get_json_key_value(json_data, 'coredata')
-    article_dic['Title']         = get_json_key_value(coredata_dict, 'dc:title')
-    article_dic['DOI']           = get_json_key_value(coredata_dict, 'prism:doi')
-    article_dic['EID']           = get_json_key_value(coredata_dict, 'eid')
-    article_dic['Document Type'] = get_json_key_value(coredata_dict, 'subtypeDescription')
-    article_dic['PubMed ID']     = get_json_key_value(coredata_dict, 'pubmed-id')
-    article_dic['Publisher']     = get_json_key_value(coredata_dict, 'dc:publisher')
-    article_dic['Cited by']      = get_json_key_value(coredata_dict, 'citedby-count')
-    article_dic['Abstract']      = get_json_key_value(coredata_dict, 'dc:description')
-    
-    # Parsing open access
-    openaccess = get_json_key_value(coredata_dict, 'openaccess')
-    if openaccess == "2" : 
-        article_dic['Open Access'] = "All Open Access; Green Open Access"
-    if openaccess == "1" : 
-        article_dic['Open Access'] = "All Open Access; Green Open Access; Gold Open Access (Hybrid?)"
-    
-    # Parsing link
-    link_info = get_json_key_value(coredata_dict, 'link')
-    if isinstance(link_info, list):        
-        for link_dict in link_info:
-            link_rel = get_json_key_value(link_dict, '@rel')
-            if link_rel == "scopus": article_dic['Link'] = get_json_key_value(link_dict, '@href')
-    else:
-        link_dict =  link_info
-        article_dic['Link'] = get_json_key_value(link_dict, '@href')
-    
+    coredata_dict = get_json_key_value(json_data, 'coredata')
+    if check_not_none(coredata_dict):
+        article_dic['Title']         = get_json_key_value(coredata_dict, 'dc:title')
+        article_dic['DOI']           = get_json_key_value(coredata_dict, 'prism:doi')
+        article_dic['EID']           = get_json_key_value(coredata_dict, 'eid')
+        article_dic['Document Type'] = get_json_key_value(coredata_dict, 'subtypeDescription')
+        article_dic['PubMed ID']     = get_json_key_value(coredata_dict, 'pubmed-id')
+        article_dic['Publisher']     = get_json_key_value(coredata_dict, 'dc:publisher')
+        article_dic['Cited by']      = get_json_key_value(coredata_dict, 'citedby-count')
+        article_dic['Abstract']      = get_json_key_value(coredata_dict, 'dc:description')
+
+        # Parsing open access
+        openaccess = get_json_key_value(coredata_dict, 'openaccess')
+        if openaccess == "2" : 
+            article_dic['Open Access'] = "All Open Access; Green Open Access"
+        if openaccess == "1" : 
+            article_dic['Open Access'] = "All Open Access; Green Open Access; Gold Open Access (Hybrid?)"
+
+        # Parsing link
+        link_info = get_json_key_value(coredata_dict, 'link')
+        if check_not_none(link_info):
+            if isinstance(link_info, list):        
+                for link_dict in link_info:
+                    link_rel = get_json_key_value(link_dict, '@rel')
+                    if link_rel == "scopus": article_dic['Link'] = get_json_key_value(link_dict, '@href')
+            else:
+                link_dict =  link_info
+                article_dic['Link'] = get_json_key_value(link_dict, '@href')
+
 
 def _make_json_data_dict(json_data, article_dic):
     
     # Setting default values (not in json_data)
     article_dic['Source'] = "Scopus"
     
     # Parsing json data
```

### Comparing `ScopusApyJson-1.0.0/ScopusApyJson/json_utils.py` & `ScopusApyJson-1.1.0/ScopusApyJson/json_utils.py`

 * *Files identical despite different names*

### Comparing `ScopusApyJson-1.0.0/ScopusApyJson.egg-info/PKG-INFO` & `ScopusApyJson-1.1.0/ScopusApyJson.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScopusApyJson
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python modules for parsing the response to a Scopus API request
 Home-page: https://github.com/TickyWill/ScopusApyJson
 Author: BiblioAnalysis team
 Author-email: francois.bertin7@wanadoo.fr, amal.chabli@orange.fr
 License: MIT
 Keywords: Metadata parsing,Scopus request,API management
 Platform: UNKNOWN
@@ -35,16 +35,17 @@
 scopus_df = saj.build_scopus_df_from_api(doi_list)
 scopus_df.to_excel(<your_fullpath_file.xlsx), index = False)
 ```
 **for more exemples refer to** [ScopusApyJson-exemples](https://github.com/TickyWill/ScopusApyJson/Demo_ScopusApyJson.ipynb).
 
 
 # Release History
-1.0.0 first release
+- 1.0.0 first release
+- 1.1.0 check of fields availability when parsing the request response
 
 
 # Meta
-	- authors : BiblioAbnalysis team
+	- authors : BiblioAnalysis team
 
 Distributed under the [MIT license](https://mit-license.org/)
```

### Comparing `ScopusApyJson-1.0.0/ScopusApyJson.egg-info/SOURCES.txt` & `ScopusApyJson-1.1.0/ScopusApyJson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ScopusApyJson-1.0.0/setup.py` & `ScopusApyJson-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # Reading the content of the "requirements.txt" file
 with open(path.join(this_directory, 'requirements.txt'), encoding='utf-8') as f:
     install_requires = f.read().strip().split('\n')
 
 # Setting the setup parameters
 setup(name = 'ScopusApyJson',
-      version = '1.0.0',
+      version = '1.1.0',
       description = 'Python modules for parsing the response to a Scopus API request',
       long_description = long_description,
       long_description_content_type = 'text/markdown',
       include_package_data = True,
       license = 'MIT',
       classifiers = [
         'Development Status :: 4 - Beta',
```

