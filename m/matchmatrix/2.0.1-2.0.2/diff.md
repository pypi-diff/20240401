# Comparing `tmp/matchmatrix-2.0.1.tar.gz` & `tmp/matchmatrix-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matchmatrix-2.0.1.tar", last modified: Mon Apr  1 07:57:44 2024, max compression
+gzip compressed data, was "matchmatrix-2.0.2.tar", last modified: Mon Apr  1 20:43:22 2024, max compression
```

## Comparing `matchmatrix-2.0.1.tar` & `matchmatrix-2.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 07:57:44.472164 matchmatrix-2.0.1/
--rw-rw-rw-   0        0        0     1092 2024-03-27 12:25:58.000000 matchmatrix-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     7222 2024-04-01 07:57:44.456538 matchmatrix-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6567 2024-04-01 07:49:01.000000 matchmatrix-2.0.1/README.md
--rw-rw-rw-   0        0        0      700 2024-03-31 17:10:48.000000 matchmatrix-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 07:57:44.472164 matchmatrix-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      482 2024-03-31 17:11:35.000000 matchmatrix-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:57:44.440900 matchmatrix-2.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:57:44.456538 matchmatrix-2.0.1/src/matchmatrix/
--rw-rw-rw-   0        0        0      654 2024-03-31 17:03:50.000000 matchmatrix-2.0.1/src/matchmatrix/__init__.py
--rw-rw-rw-   0        0        0    18758 2024-03-28 14:09:58.000000 matchmatrix-2.0.1/src/matchmatrix/constants.py
--rw-rw-rw-   0        0        0     8393 2024-03-28 20:21:22.000000 matchmatrix-2.0.1/src/matchmatrix/functions.py
--rw-rw-rw-   0        0        0    58637 2024-04-01 07:52:04.000000 matchmatrix-2.0.1/src/matchmatrix/manager.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:57:44.456538 matchmatrix-2.0.1/src/matchmatrix.egg-info/
--rw-rw-rw-   0        0        0     7222 2024-04-01 07:57:44.000000 matchmatrix-2.0.1/src/matchmatrix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-04-01 07:57:44.000000 matchmatrix-2.0.1/src/matchmatrix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 07:57:44.000000 matchmatrix-2.0.1/src/matchmatrix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-01 07:57:44.000000 matchmatrix-2.0.1/src/matchmatrix.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 20:43:22.686326 matchmatrix-2.0.2/
+-rw-rw-rw-   0        0        0     1092 2024-03-27 12:25:58.000000 matchmatrix-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     7257 2024-04-01 20:43:22.686326 matchmatrix-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6602 2024-04-01 19:31:14.000000 matchmatrix-2.0.2/README.md
+-rw-rw-rw-   0        0        0      700 2024-04-01 20:42:27.000000 matchmatrix-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 20:43:22.690839 matchmatrix-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      482 2024-04-01 20:42:36.000000 matchmatrix-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:43:22.592468 matchmatrix-2.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 20:43:22.639455 matchmatrix-2.0.2/src/matchmatrix/
+-rw-rw-rw-   0        0        0      654 2024-03-31 17:03:50.000000 matchmatrix-2.0.2/src/matchmatrix/__init__.py
+-rw-rw-rw-   0        0        0    13102 2024-04-01 20:37:31.000000 matchmatrix-2.0.2/src/matchmatrix/constants.py
+-rw-rw-rw-   0        0        0     8393 2024-03-28 20:21:22.000000 matchmatrix-2.0.2/src/matchmatrix/functions.py
+-rw-rw-rw-   0        0        0    58591 2024-04-01 19:13:22.000000 matchmatrix-2.0.2/src/matchmatrix/manager.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:43:22.670710 matchmatrix-2.0.2/src/matchmatrix.egg-info/
+-rw-rw-rw-   0        0        0     7257 2024-04-01 20:43:22.000000 matchmatrix-2.0.2/src/matchmatrix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-04-01 20:43:22.000000 matchmatrix-2.0.2/src/matchmatrix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 20:43:22.000000 matchmatrix-2.0.2/src/matchmatrix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-01 20:43:22.000000 matchmatrix-2.0.2/src/matchmatrix.egg-info/top_level.txt
```

### Comparing `matchmatrix-2.0.1/LICENSE` & `matchmatrix-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `matchmatrix-2.0.1/PKG-INFO` & `matchmatrix-2.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 Metadata-Version: 2.1
 Name: matchmatrix
-Version: 2.0.1
+Version: 2.0.2
 Summary: Customisable class to produce a matrix of match scores across multiple dimensions
 Home-page: https://github.com/porteverte/matchmatrix
 Author: Porte Verte
 Author-email: Port Verte <porte_verte@outlook.com>
 Project-URL: Homepage, https://github.com/porteverte/matchmatrix
 Project-URL: Issues, https://github.com/porteverte/matchmatrix/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1>About</h1>
+**multimatch | multi-dimensional match scores**
 
-**MultiMatch | Multi-Dimensional Match Scores**
+<h1>About</h1>
 
 How to use this package:
 
 1. Customise the built-in class to generate a matrix of match scores across multiple dimensions.
 2. Apply your own rules to the scores in the matrix as per your specific use-case to identify matches.
 
 Key features:
 
 1. Methods to cleanse and standardise company names.
 2. A method to dedupe data sets and add new IDs.
-3. Functionality to match in subsets to optimise performance.
+3. Functionality to match subsets to optimise performance.
 
 <h1>Dependencies</h1>
 
-**Required**
+**python 3.8 is required for this package**
+
+**Required Packages**
 
 | Package	| Version	| License						|
 |---------------|---------------|-------------------------------------------------------|
 | pandas	| 1.3.5		| BSD License (BSD 3-Clause License			|
 | numpy		| 1.20.3	| BSD License						|
 | rapidfuzz	| 1.9.1		| MIT License (MIT)					|
 | unidecode	| 1.2.0		| GNU General Public License v2 or later (GPLv2+)	|
 
-**Optional**
+**Optional Packages**
 
 | Package	| Version	| License						|
 |---------------|---------------|-------------------------------------------------------|
 | networkx	| TBC		| BSD License						|
 
 <h1>Data Preparation</h1>
 
@@ -82,23 +84,23 @@
     * fuzz.token_set_ratio: set intersection match score
     * set_intersection_match_score: alternative to the above
 3. remove_spaces: True or False (useful for postcodes)
 4. log_path: self explanatory
 
 Example code below.
 
-	# import objects
+	# import match manager class
     from matchmatrix import MatchManager
 
     # optional: create a company suffixes dictionary to integrate with default one
     csd = {'ltd': ['ltd', 'ltd.', 'limited', 'l.i.m.i.t.e.d.', 'limmyted']
           , 'plc': ['plc', 'plc.', 'public limited company', 'pee ell see']
           , 'gmbh': ['gmbh', 'gmbh.']}
     
-    # create class
+    # initialise class
     MyMatch = MatchManager()
     
     # build class
     MyMatch.build_class(
                         # positional arguments
                         lookup_frame, lookup_key, lookup_name
                         , match_frame, match_key, match_name
@@ -108,22 +110,19 @@
                         # , match_function = 'fuzz.ratio'
                         # , remove_spaces = False
                         , log_path=log_path
                         )
 
     # optional: integrate company suffixes dictionary with default one (if defined above)
     # set replace=True to replace the default one completely
-    MyMatch.integrate_company_suffixes_dictionary(csd)    
-    
-    # if necessary re-instate the default dictionary
-    # MyMatch.reset_company_dictionary()
+    MyMatch.integrate_company_suffixes_dictionary(csd)
 
 <h2>Optional (but recommended): define subsetting fields.</h2>
 
-This will do the matching in subsets e.g. county e.g. Yorkshire to Yorkshire to SIGNIFICANTLY speed up processing time.\
+This will do the matching in subsets e.g. county (Yorkshire to Yorkshire etc.) to SIGNIFICANTLY speed up processing time.
 
     MyMatch.subset_fields = ('county_name', 'county_name')
 
 <h2>Optional (but recommended): cleanse the primary matching fields</h2>
 
     MyMatch.cleanse_primary_fields()
     
@@ -135,48 +134,48 @@
     
     initial_results = MyMatch.initial_results
     
 <h2>Optional (but recommended): add secondary matches to the class</h2>
     
 **Positional argugments:**
 
-* lookup_name: name of column to match from in lookup frame.
-* match_name: name of column to match to in match frame.
+* lookup_column: name of column to match from in lookup frame.
+* match_column: name of column to match to in match frame.
 
 **Optional argugments:**
 
 * field_type: same options as primary_field_type above.
 * remove_spaces: as defined above.
 * match_function: as defined above.
 * duplicate_suffix: text to add to a duplicate column e.g. '_stripped'.
 * cleanse_data: True or False.
 * secondary_match_name: a name to refer to later e.g. if doing additional join matches.
 
 Example code below.
     
     MyMatch.clear_secondary_matches()
-    MyMatch.add_secondary_match('address', 'address', field_type='address', cleanse_data=True, secondary_match_name='address')
-    MyMatch.add_secondary_match('postcode', 'postcode', field_type='address', remove_spaces=True, cleanse_data=True, secondary_match_name='postcode')
+    MyMatch.add_secondary_match('first_line_of_address', 'first_line_of_address', field_type='address', cleanse_data=True, secondary_match_name='first_line_of_address')
+    MyMatch.add_secondary_match('post_code', 'post_code', field_type='address', remove_spaces=True, cleanse_data=True, secondary_match_name='post_code')
     
 <h2>Optional: get additional primary matches by joining a pair of secondary match fields</h2>
 
 **Positional arguments:**
 
 * secondary_match_name: the name defined above
     
 **Optional arguments:**
 
 * explode_column: True or False (if a column contains multiple values separated by a comma).
 
 Example code below.
 	
 	# get additional join matches
-    MyMatch.get_additional_join_matches('postcode')
+    MyMatch.get_additional_join_matches('post_code')
 
-<h2>Optional: create and integrate a separate class e.g. a primary match on address.</h2>
+<h2>Optional: create and integrate a separate class e.g. a primary match on first_line_of_address.</h2>
 
 	# to be developed
     
 <h2>Optional: Get secondary matches (if defined above)</h2>
 
     MyMatch.get_secondary_matches()  
 
@@ -184,17 +183,17 @@
     
     initial_results = MyMatch.initial_results
     
 <h2>Identify matches</h2>
 
 Instructions:
 
-1. Apply a series of rules across the different scores in **MyMatch.initial_results** to identify matches.\
+1. Apply a series of rules across the different scores in **MyMatch.initial_results** to identify matches.
 
-2. Create the frame **MyMatch.matched_results** in the class comprising matches ONLY.\
+2. Create the frame **MyMatch.matched_results** in the class comprising matches ONLY.
 
 <h2>Dedupe matched results and add match ids</h2>
 
     # add deduped ids to original keys
     MyMatch.create_deduped_match_ids()
 
     # get xref frame that maps original keys to deduped ids
```

### Comparing `matchmatrix-2.0.1/README.md` & `matchmatrix-2.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-<h1>About</h1>
+**multimatch | multi-dimensional match scores**
 
-**MultiMatch | Multi-Dimensional Match Scores**
+<h1>About</h1>
 
 How to use this package:
 
 1. Customise the built-in class to generate a matrix of match scores across multiple dimensions.
 2. Apply your own rules to the scores in the matrix as per your specific use-case to identify matches.
 
 Key features:
 
 1. Methods to cleanse and standardise company names.
 2. A method to dedupe data sets and add new IDs.
-3. Functionality to match in subsets to optimise performance.
+3. Functionality to match subsets to optimise performance.
 
 <h1>Dependencies</h1>
 
-**Required**
+**python 3.8 is required for this package**
+
+**Required Packages**
 
 | Package	| Version	| License						|
 |---------------|---------------|-------------------------------------------------------|
 | pandas	| 1.3.5		| BSD License (BSD 3-Clause License			|
 | numpy		| 1.20.3	| BSD License						|
 | rapidfuzz	| 1.9.1		| MIT License (MIT)					|
 | unidecode	| 1.2.0		| GNU General Public License v2 or later (GPLv2+)	|
 
-**Optional**
+**Optional Packages**
 
 | Package	| Version	| License						|
 |---------------|---------------|-------------------------------------------------------|
 | networkx	| TBC		| BSD License						|
 
 <h1>Data Preparation</h1>
 
@@ -66,23 +68,23 @@
     * fuzz.token_set_ratio: set intersection match score
     * set_intersection_match_score: alternative to the above
 3. remove_spaces: True or False (useful for postcodes)
 4. log_path: self explanatory
 
 Example code below.
 
-	# import objects
+	# import match manager class
     from matchmatrix import MatchManager
 
     # optional: create a company suffixes dictionary to integrate with default one
     csd = {'ltd': ['ltd', 'ltd.', 'limited', 'l.i.m.i.t.e.d.', 'limmyted']
           , 'plc': ['plc', 'plc.', 'public limited company', 'pee ell see']
           , 'gmbh': ['gmbh', 'gmbh.']}
     
-    # create class
+    # initialise class
     MyMatch = MatchManager()
     
     # build class
     MyMatch.build_class(
                         # positional arguments
                         lookup_frame, lookup_key, lookup_name
                         , match_frame, match_key, match_name
@@ -92,22 +94,19 @@
                         # , match_function = 'fuzz.ratio'
                         # , remove_spaces = False
                         , log_path=log_path
                         )
 
     # optional: integrate company suffixes dictionary with default one (if defined above)
     # set replace=True to replace the default one completely
-    MyMatch.integrate_company_suffixes_dictionary(csd)    
-    
-    # if necessary re-instate the default dictionary
-    # MyMatch.reset_company_dictionary()
+    MyMatch.integrate_company_suffixes_dictionary(csd)
 
 <h2>Optional (but recommended): define subsetting fields.</h2>
 
-This will do the matching in subsets e.g. county e.g. Yorkshire to Yorkshire to SIGNIFICANTLY speed up processing time.\
+This will do the matching in subsets e.g. county (Yorkshire to Yorkshire etc.) to SIGNIFICANTLY speed up processing time.
 
     MyMatch.subset_fields = ('county_name', 'county_name')
 
 <h2>Optional (but recommended): cleanse the primary matching fields</h2>
 
     MyMatch.cleanse_primary_fields()
     
@@ -119,48 +118,48 @@
     
     initial_results = MyMatch.initial_results
     
 <h2>Optional (but recommended): add secondary matches to the class</h2>
     
 **Positional argugments:**
 
-* lookup_name: name of column to match from in lookup frame.
-* match_name: name of column to match to in match frame.
+* lookup_column: name of column to match from in lookup frame.
+* match_column: name of column to match to in match frame.
 
 **Optional argugments:**
 
 * field_type: same options as primary_field_type above.
 * remove_spaces: as defined above.
 * match_function: as defined above.
 * duplicate_suffix: text to add to a duplicate column e.g. '_stripped'.
 * cleanse_data: True or False.
 * secondary_match_name: a name to refer to later e.g. if doing additional join matches.
 
 Example code below.
     
     MyMatch.clear_secondary_matches()
-    MyMatch.add_secondary_match('address', 'address', field_type='address', cleanse_data=True, secondary_match_name='address')
-    MyMatch.add_secondary_match('postcode', 'postcode', field_type='address', remove_spaces=True, cleanse_data=True, secondary_match_name='postcode')
+    MyMatch.add_secondary_match('first_line_of_address', 'first_line_of_address', field_type='address', cleanse_data=True, secondary_match_name='first_line_of_address')
+    MyMatch.add_secondary_match('post_code', 'post_code', field_type='address', remove_spaces=True, cleanse_data=True, secondary_match_name='post_code')
     
 <h2>Optional: get additional primary matches by joining a pair of secondary match fields</h2>
 
 **Positional arguments:**
 
 * secondary_match_name: the name defined above
     
 **Optional arguments:**
 
 * explode_column: True or False (if a column contains multiple values separated by a comma).
 
 Example code below.
 	
 	# get additional join matches
-    MyMatch.get_additional_join_matches('postcode')
+    MyMatch.get_additional_join_matches('post_code')
 
-<h2>Optional: create and integrate a separate class e.g. a primary match on address.</h2>
+<h2>Optional: create and integrate a separate class e.g. a primary match on first_line_of_address.</h2>
 
 	# to be developed
     
 <h2>Optional: Get secondary matches (if defined above)</h2>
 
     MyMatch.get_secondary_matches()  
 
@@ -168,17 +167,17 @@
     
     initial_results = MyMatch.initial_results
     
 <h2>Identify matches</h2>
 
 Instructions:
 
-1. Apply a series of rules across the different scores in **MyMatch.initial_results** to identify matches.\
+1. Apply a series of rules across the different scores in **MyMatch.initial_results** to identify matches.
 
-2. Create the frame **MyMatch.matched_results** in the class comprising matches ONLY.\
+2. Create the frame **MyMatch.matched_results** in the class comprising matches ONLY.
 
 <h2>Dedupe matched results and add match ids</h2>
 
     # add deduped ids to original keys
     MyMatch.create_deduped_match_ids()
 
     # get xref frame that maps original keys to deduped ids
```

### Comparing `matchmatrix-2.0.1/pyproject.toml` & `matchmatrix-2.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "matchmatrix"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
   { name="Port Verte", email="porte_verte@outlook.com" },
 ]
 description = "Customisable class to produce a matrix of match scores across multiple dimensions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `matchmatrix-2.0.1/src/matchmatrix/__init__.py` & `matchmatrix-2.0.2/src/matchmatrix/__init__.py`

 * *Files identical despite different names*

### Comparing `matchmatrix-2.0.1/src/matchmatrix/constants.py` & `matchmatrix-2.0.2/src/matchmatrix/constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,166 +1,108 @@
 # Copyright (C) 2021-2024 Porte Verte
 
 # =================================================================================================================================
 # COMPANY SUFFIXES DICTIONARY AND LIST
 # =================================================================================================================================
 
 # dictionary to standardise names -- which will then be converted to a 2 dimensional list (with the key cascaded)
-# each country section does not necessarily comprise all terms for that country -- just dictionary addenda
 
 COMPANY_SUFFIXES_DICT = {
-    # uk
-    'group holding ltd': ['group holding ltd', 'group holdings ltd', 'group holding ltd.', 'group holdings ltd.', 'group holding l.t.d.', 'group holdings l.t.d.'
-                          , 'group holding limited', 'group holdings limited']
+    'group holding ltd': ['group holding ltd', 'group holdings ltd', 'group holding ltd.', 'group holdings ltd.', 'group holding l.t.d.', 'group holdings l.t.d.', 'group holding limited', 'group holdings limited']
     , 'group holding': ['group holding', 'group holdings', 'grp holding', 'grp holdings', 'grp. holding', 'grp. holdings']
-    , '& co ltd': ['& co ltd','& co. ltd', '& company ltd', '& co ltd.','& co ltd.','& co ltd.', '& co ltd.','& co. ltd.', '& company ltd.', '& co l.t.d.'
-                   ,'& co l.t.d.','& co l.t.d.', '& co l.t.d.','& c.o. l.t.d.', '& company l.t.d.', '& co limited','& co limited','& co limited', '& co limited'
-                   ,'& co. limited', '& company limited']
+    , '& co ltd': ['& co ltd','& co. ltd', '& company ltd', '& co ltd.','& co ltd.','& co ltd.', '& co ltd.','& co. ltd.', '& company ltd.', '& co l.t.d.','& co l.t.d.','& co l.t.d.'
+                   , '& co l.t.d.','& c.o. l.t.d.', '& company l.t.d.', '& co limited','& co limited','& co limited', '& co limited','& co. limited', '& company limited']
     , '& co': ['& co','& co.', '& c.o.', '&co', '& company', 'and co','and co.','and company', '+ co', '+ co.', '+ c.o.', '+co']
     , 'assoc': ['assoc', 'assoc.' 'association', 'assoc.']
     , 'corp': ['corp', 'corp.', 'corporated', 'corporation', 'corps']
     , 'pllc': ['pllc', 'pllc.', 'p.l.l.c.', 'public limited liability company']
     , 'lllp': ['lllp', 'lllp.', 'l.l.l.p.', 'limited liability limited partnership']
-    , 'ltd': ['ltd', 'ltd.', 'l.t.d.', 'limited', 'limited company', 'l.t.d', 'l t d ', 'l. t. d.', 'ltd. .', 'ltd. 2', 'ltd 2', 'limited.']
+    , 'ltd': ['ltd', 'ltd.', 'l.t.d.', 'limited', 'limited company', 'l.t.d', 'l t d ', 'l. t. d.', 'limited.']
     , 'plc': ['plc', 'plc.', 'p.l.c.', 'public limited company', 'p l c', ' p. l. c.', 'p.l.c']
     , 'llc': ['llc', 'llc.', 'l.l.c.', 'limitied liability company', 'l.l.c', 'l l c', 'l. l. c.']
     , 'llp': ['llp', 'llp.', 'l.l.p.', 'limited liability partnership', 'l l p', 'l. l. p.']
     , 'inc': ['inc','inc.','incorporated', 'i n c', 'i. n. c.']
-    # germany
     , 'gmbh & co kg': ['gmbh & co kg', 'gmbh & co. kg', 'gmbh & co.kg' ,'gmbh&co kg', 'gmbh and co. kg', 'gmbh and co.kg', 'gmbh and co kg', 'gmbh + co. kg'
-                       ,'gmbh + co.kg', 'gmbh + co kg', 'gmbh co. kg', 'gmbh co.kg', 'gmbh co kg', 'gmbh 6co. kg', 'gmbh 6co.kg', 'gmbh 6co kg'
-                       , 'gmbha &a co.a kg', 'gmbhcokg','gmbh kg', 'gmbh & co. k', 'gmbh und co. kg', 'gmbh und co.', 'gmbh& co.', 'gmbh & co. kgaa'
-                       , 'gmbh & co kgaa','gmbh &co', 'gmbh+co.kg', 'gmbh & co .kg', 'mbh &co. kg', 'gmbh u. co.', 'gmbh &co.', 'gmbh&co.kg', 'gmbh u co'
-                       , 'gmbh & c', 'gmbh &. co.kg', 'gmbh u. co', 'gmbh &. co', 'gmbh& co.kg', 'gmbh & co. og', 'gmbh & co.', '& co.gmbh & co.', 'mbh & co.kg'
-                       , 'gmbh & co.kg.', 'gmbh & co', 'gesmbh & co kg', 'gmbh und co.kg', 'gmbh und co. kg', 'mbh & co. kg', 'gmbh u. co kg', 'gmbh u. co. kg'
-                       , 'gmbh &. co kg', 'gmbh und co kg', 'gmbh and co k', 'gmbh&co. kg', 'gmbh u. co.kg', 'gmbh &co.kg', 'gmbh & co . kg', 'gesellschaft mbh & cokg'
-                       , 'ges.m.b.h. & co kg', 'gesellschaft m.b.h. u. co. kg', 'gmbh & cco kg', 'ges.m.b.h & co. kg', 'gmbh & co. kg kg', 'gmbh & co kg i. gr.'
-                       , 'gmbh & co. kg - 2017', 'gmbh & cokg', 'gmbh u co']
-    , 'bv & co kg': ['bv & co kg', 'bv & co. kg', 'bv & co.kg', 'bv&co kg', 'bv and co. kg', 'bv and co.kg', 'bv and co kg', 'bv + co. kg', 'bv + co.kg',
-                     'bv + co kg', 'bv co. kg', 'bv co.kg', 'bv co kg', 'bv 6co. kg', 'bv 6co.kg', 'bv 6co kg', 'bva &a co.a kg', 'bvcokg', 'b. v. & co. kg']
-    , 'se & co kg': ['se & co kg','se & co. kg', 'se & co. k.g.', 'se & co. kg.', 's.e. & co. kg', 'se & co kg.', 'se & co k.g.', 's.e. & co kg.', 'se and co kg'
-                     , 'se and co. kg', 'se and co kg.', 'se and co k.g.', 's.e. and co kg', 'se. and co kg', 'se & co. k']
-    , 'ag & co kg': ['ag & co kg','ag & co. kg', 'ag & co. k.g.', 'ag & co. kg.', 'a.g. & co. kg', 'ag & co kg.', 'ag & co k.g.', 'a.g. & co kg.', 'ag and co kg'
-                     , 'ag and co. kg', 'ag and co kg.', 'ag and co k.g.', 'a.g. and co kg', 'ag. and co kg', 'ag & co. k', 'ag&co kg', 'ag & co.kg']    
-    , 'gmbh': ['gmbh', 'gmbh.', 'g.m.b.h.', 'ggmbh', 'g.m.b.h', 'g m b h', 'g. m. b. h.', 'g bh', 'ges.m.b.h.', 'gesellschaft mit beschrankter haftung', 'ges.m.b.h'
-               , 'gesellschaft m.b.h', 'gesmbh.', 'gesellschaft m.b.h.', 'ges.m.h', 'gesellschaft m. b. h.', 'gesmb.h.', 'gesellschaft mbh', 'gmbh alt']
-    , 'ohg': ['ohg', 'ohg.', 'o.h.g.', 'o.h.g', 'o h g', 'o. h. g.', 'offene handelsgesellschaft']
-    , 'ev': ['ev', 'e.v.', 'ev.', 'e. v.', 'e.v. 2', 'e.v']
-    , 'ag': ['ag', 'a.g.', 'ag.', 'a.g', 'aktiengesellschaft', 'a. g.']
-    , 'kg': ['kg', 'k.g.', 'kg.', 'k.g', 'k g', 'k. g.', 'kommanditgesellschaft']
-    , 'ek': ['ek', 'e.k.', 'ek.', 'e.k', 'e. k.', 'e k', 'e.kfm', 'ekfm', 'e.kfr', 'ekfr', 'eingetragener kaufmann', 'e. k']         
-    # france
+                       ,'gmbh + co.kg', 'gmbh + co kg', 'gmbh co. kg', 'gmbh co.kg', 'gmbh co kg']
+    , 'bv & co kg': ['bv & co kg', 'bv & co. kg', 'bv & co.kg', 'bv&co kg', 'bv and co. kg', 'bv and co.kg', 'bv and co kg', 'bv + co. kg', 'bv + co.kg','bv + co kg', 'bv co. kg', 'bv co.kg', 'bv co kg']
+    , 'se & co kg': ['se & co kg','se & co. kg', 'se & co. k.g.', 'se & co. kg.', 's.e. & co. kg', 'se & co kg.', 'se & co k.g.', 's.e. & co kg.', 'se and co kg', 'se and co. kg', 'se and co kg.', 'se and co k.g.', 's.e. and co kg', 'se. and co kg']
+    , 'ag & co kg': ['ag & co kg','ag & co. kg', 'ag & co. k.g.', 'ag & co. kg.', 'a.g. & co. kg', 'ag & co kg.', 'ag & co k.g.', 'a.g. & co kg.', 'ag and co kg', 'ag and co. kg', 'ag and co kg.', 'ag and co k.g.', 'a.g. and co kg', 'ag. and co kg']    
+    , 'gmbh': ['gmbh', 'gmbh.', 'g.m.b.h.', 'ggmbh', 'g.m.b.h', 'g m b h', 'g. m. b. h.']
+    , 'ohg': ['ohg', 'ohg.', 'o.h.g.', 'o.h.g', 'o h g', 'o. h. g.']
+    , 'ev': ['ev', 'e.v.', 'ev.', 'e. v.', 'e.v']
+    , 'ag': ['ag', 'a.g.', 'ag.', 'a.g', 'a. g.']
+    , 'kg': ['kg', 'k.g.', 'kg.', 'k.g', 'k g', 'k. g.']
+    , 'ek': ['ek', 'e.k.', 'ek.', 'e.k', 'e. k.', 'e k', 'e.kfm', 'ekfm', 'e.kfr', 'ekfr', 'e. k']         
     , 'sarl': ['sarl', 'sarl.', 's.a.r.l.', 's.a.r.l', 's.a r.l', 's a r l', 's. a. r. l.', 's.a r.l.']
-    , 'sas': ['sas', 's.a.s.', 'sas.', 's.a.s', 's a s', 's. a. s.', 'sas-2']
+    , 'sas': ['sas', 's.a.s.', 'sas.', 's.a.s', 's a s', 's. a. s.']
     , 'snc': ['snc', 'snc.', 's.n.c.', 's.n.c', 's n c', 's. n. c.']
-    , 'sa': ['sa', 's.a.', 'sa.', 's.a', 'sa .', 's a', 's.a..', 's. a', 's. a .', 's . a .', 'sa 2', 's. a.', '- sa', 's.a. 2', 'sa - 2']
-     # italy
-    , 'scarl': ['scarl', 's.c.a.r.l.', 's.c.a.r.l', 'scarl.', 's.c. a r.l.']
+    , 'sa': ['sa', 's.a.', 'sa.', 's.a', 'sa .', 's a', 's.a..', 's. a', 's. a .', 's . a .', 's. a.']
+    , 'scarl': ['scarl', 's.c.a.r.l.', 's.c.a.r.l', 'scarl.']
     , 'scpa': ['scpa', 's.c.p.a.', 's.c.p.a', 'scpa.', 's c p a', 's. c. p. a.']
-    , 'srl': ['srl', 'srl.', 's.r.l.', 's.r.l', 'srls', 'srls.', 's.r.l.s.', 's.r.l', 'sr.l.', 's.rl.', 's r l', 's. r. l.', 'srl 2', 's.r.l.u.', 's.r.l.s', 's.r l']
-    , 'spa': ['spa', 's.p.a.', 'spa.', 's.pa', 'sp.a', 's.p.a', 's..p.a.', 's p a', 's. p. a.', 's p a', 's. p. a.', 'spa - 2']
-    # netherlands
+    , 'srl': ['srl', 'srl.', 's.r.l.', 's.r.l', 'srls', 'srls.', 's.r.l.s.', 's.r.l', 'sr.l.', 's.rl.', 's r l', 's. r. l.']
+    , 'spa': ['spa', 's.p.a.', 'spa.', 's.pa', 'sp.a', 's.p.a', 's..p.a.', 's p a', 's. p. a.', 's p a', 's. p. a.']
     , 'bv': ['bv', 'b.v.', 'bv.', 'b.v', 'b v.', 'b. v', 'b. v.', 'b v', '.b.v']
-    # belgium
     , 'commv': ['commv', 'c.o.m.m.v.', 'c.o.m.m.v', 'commv.', 'comm.v.']
     , 'cvba': ['cvba', 'c.v.b.a.', 'c.v.b.a', 'cvba.']
     , 'bvba': ['bvba', 'b.v.b.a.', 'b.v.b.a', 'bvba.']
     , 'asbl': ['asbl', 'a.s.b.l.', 'a.s.b.l', 'asbl.']
     , 'scrl': ['scrl', 's.c.r.l.', 's.c.r.l', 'scrl.']
     , 'sprl': ['sprl', 's.p.r.l.', 's.p.r.l', 'sprl.']
     , 'ivzw': ['ivzw', 'i.v.z.w.', 'i.v.z.w', 'ivzw.']
     , 'vof': ['vof', 'v.o.f.', 'v.o.f', 'vof.']
     , 'vzw': ['vzw', 'v.z.w.', 'v.z.w', 'vzw.']
     , 'cv': ['cv', 'c.v.', 'cv.', 'c.v', 'c. v.']
     , 'nv': ['nv', 'n.v.', 'nv.', 'n.v', 'n. v.']
-    # spain
     , 'coop v': ['coop v', 'coop. v.', 'coop. v', 'coop v.']
     , 'sccl': ['sccl', 's.c.c.l.', 's.c.c.l', 'sccl.', 's c c l ', 's. c. c. l.']
     , 'slu': ['slu', 's.l.u.', 'slu.', 's.l.u', 's l u', 's. l. u.']
     , 'slp': ['slp', 's.l.p.', 'slp.', 's. l. p.', 's.l.p', 's l p']
     , 'sau': ['sau', 's.a.u.', 'sau.', 's.a.u', 's a u', 's. a. u.']
     , 'sl': ['sl', 's.l.', 'sl.', 's l', 's.l', 's. l.']          
-    # portugal
     , 'lda': ['lda', 'l.d.a.', 'lda.', 'l.d.a', 'limitada', 'l d a', 'l. d. a.']            
-    , 'sc': ['sc', 's.c.', 'sc.', 's.c', 'sc .', 's c', 's.c..', 's. c', 's. c .', 's . c .', 's.c. 2']
-    # denmark
+    , 'sc': ['sc', 's.c.', 'sc.', 's.c', 'sc .', 's c', 's. c', 's. c .', 's . c .']
     , 'aps': ['aps', 'a.p.s.', 'a.p.s', 'aps.', 'aps .', ' a p s', 'a. p. s.']
-    # swdeden
-    , 'ab': ['ab', 'a.b.', 'a.b', 'a b', 'a. b.', 'aktiebolag', 'a/b']
-    # czech republic            
-    , 'spol sro': ['spol sro', 'spol. sro', 'spol.s r.o.', 'spol. s r. o._2', 'spol. s r.o.,_2', 'spol. s r. o._2', 'spol. s r', 'spol. s r.o.', 'spol. s.r.o.'
-                   , 'spol. s r. o.', 'spol. s r.o', 'spol. s r.o', 'spol. s r..o.', 'spol. s r. o.', 'spol. s .r.o.', 'spol. s r.o.', 'spol. s. r. o'
-                   , 'spol. s. r. o.', 'spol. s.r.o', 'spol.s r.o', 'spol.r.o.', 'spol. s r. o']
-    , 'sro': ['sro', 'sro.', 's.r.o.', 's r.o.', 's r.o', 's. r. o.','s r. o.', 's.r.o', 's .r.o.', 's.r.o.,', 's r..o.', 's.r.o.,,', 's. r. o', 's r o', 's r o.'
-              , 's.r. o', 's r.o', 's r. o.,', 's.r.o', 's .r.o.', 's.r.o', 's.r.o.,', 's.r.o..', 's.r.o,', 's. r. o._2', 's r.o_2', 's r.o._2', 's.ro.'
-              , 's.r.o._2', 's.r.o. 2', 's.r.o..', 's..r.o.', 's.r.o.2', 's.r.o .']     
+    , 'ab': ['ab', 'a.b.', 'a.b', 'a b', 'a. b.']        
+    , 'spol sro': ['spol sro', 'spol. sro', 'spol.s r.o.', 'spol. s r', 'spol. s r.o.', 'spol. s.r.o.', 'spol. s r. o.', 'spol. s r.o', 'spol. s r.o'
+                   , 'spol. s r. o.', 'spol. s .r.o.', 'spol. s r.o.', 'spol. s. r. o', 'spol. s. r. o.', 'spol. s.r.o', 'spol.s r.o', 'spol.r.o.', 'spol. s r. o']
+    , 'sro': ['sro', 'sro.', 's.r.o.', 's r.o.', 's r.o', 's. r. o.','s r. o.', 's.r.o', 's. r. o', 's r o', 's r o.', 's.r. o', 's r.o', 's r. o.,', 's.r.o', 's .r.o.', 's.r.o']     
     , 'o.p.s.': ['o.p.s.', 'o.p.s', 'o. p. s.']
     , 'vos':['vos', 'vos.', 'v.o.s.', 'v.o.s']
-    , 'as': ['as', 'a.s.','a. s.', 'a s.', 'a. s', 'a s', 'a.s.,', 'a.s. ,', 'a .s.', 'a.s', 'a.s..', 'a.s.,.', 'a.s.,,', 'a.s._2', 'a.s._', 'a..s.', 'a.s...'
-             , 'a..s.', 'as.', 'a/s', 'a/s.', 'a.s. 2', 'a / s', '.a.s', 'a.s. . .']
+    , 'as': ['as', 'a.s.','a. s.', 'a s.', 'a. s', 'a s', 'a.s.,', 'a.s. ,', 'a .s.', 'a.s', 'a..s.', 'as.', '.a.s']
     , 'ks':['ks', 'ks.', 'k.s.', 'k.s', 'k s', 'k. s.']
     , 'zs':['zs', 'zs.', 'z.s.', 'z.s', 'z s', 'z. s.']            
-    # poland
     , 'sp zoo spk': ['sp zoo spk', 'sp zoo sp k', 'sp. z.o.o. s.p. k.', 'sp. z.o.o. s.p.k.', 'sp. z o.o. sp. k','sp. z o.o sp.k.','sp. z o.o. sk',  'sp z o.o. sp.k.'
                      , 'sp. z o. o. sp. k.', 'sp. z o.o. sp.k.', 'sp. z o.o. sp. k.', 'sp z o.o. sp.k', 'sp. z.o.o. sp.k.', 'sp. z o.o. sp.k', 'sp. z o. o. sp. k'
-                     , 'sp. z o.o. sp. kom.', 'sp. z.o. sp. k', 'sp. z o.o. spk', 'sp.z o.o. sp.k', 'sp z o.o. sp. k.', 'sp. z o.o. sp. k.a', 'spolka z o. o. sp. k'
-                     , 'sp. z o. o. sp. kom.', 'sp.z o.o. sp. k.', 'sp. z o.o. spolka komandytowa', 'sp z o.o. spolka komandytowa', 'sp z o o spolka komandytowa'
-                     , 'spolka z o.o. spolka komandytowa', 'sp. z o. o. spolka komandytowa', 'sp. z o.o. spolka komandytowa', 'sp. z.o.o. sp. k.', 'sp. z o.o. sp.'
-                     , 'sp.zo.o. sp.k.', 'sp. zo.o. sp.k', 'sp. z.o.o. sp.k', 'spolka z ograniczona odpowiedzialnoscia sp.k', 'spolka z ograniczona odpowiedzialnoscia sp. k'
-                     , 'spolka z ograniczona odpowiedzialnoscia sp k', 'spolka z ograniczona odpowiedzialnoscia spk', 'sp.z o.o. sp.k.', 'sp z.o.o sp. k', 'spolka zoo - sp.k.'
-                     , 'spolka z ograniczona odpowiedzialnoscia sp.k. 1', 'sp zo.o sp. k.', 'spolka z ogran iczona odpowiedzialnoscia sp.k.'
-                     , 'spolka z ograniczona odpowiedzialnoscia sp.k.', 'spolka z ograniczona odpowiedzialnoscia sp. k.', 'spolka z ograniczona odpowiedzialnoscia - sp.k.'
-                     , 'spolka z o o. sp. k.', 'sp. z o.o sp.k', 'sp.zo.o sp.k', 'sp. z o. o. sp.k.', 'sp. zo.o. sp.k.', 'sp. zo.o. sp. komandytowa', 'spolka z o.o. sp.k.'
-                     , 'sp z o.o. s.k.', 'sp z o o spolka k', 'sp.z o. o. sp. k.', 'sp. o. o. sp. k.', 'sp. z.o.o sp. kom.', 'sp.zo.o. s p. k.', 'sp.z o.o.sp.k'
-                     , 'spolka z o.o. sp. k.', 'sp. z o.o. sp. komandytowa']
-    , 'sp zoo spj': ['sp zoo spj', 'sp. z o.o. sp. jawna', 'sp. z o.o. spolka jawna', 'sp. z.o.o. sp.j', 'sp. z.o.o. sp. j', 'sp. z.o.o. sp. j.', 'sp. z o.o. sp.j.'
-                     , 'sp. z o.o. - sp.j', 'sp. z o.o. sp. j.', 'sp. z o. o. sp. j.']
-    , 'sp zoo ska': ['sp zoo ska', 'sp. z.o.o. s.k.a.', 'sp. z o.o. s. k.a', 'sp. z o.o. s.k.a.',  'sp. z oo s.k.a.', 'sp. z o.o. s.k.', 'sp. z o. o. s. k.'
-                     , 'sp. z o.o. s.k.a', 'sp. z o. o. ska', 'sp. z o.o. 4f s.k.a.', 'spolka z ograniczona odpowiedzialnoscia s.k.a.'
-                     , 'spolka z ograniczona odpowiedzialnoscia ska', 'spolka z ograniczona odpowiedzialnoscia ska.', 'spolka z o.o. s.k.a.', 'sp. z o.o. ska'
-                     , 'sp. z o.o.s.k.a', 'sp. z o. o. s. k. a.', 'sp. z o.o.s.k.a.', 'sp. z o.o. s.kom']
-    , 'sp zoo': ['sp zoo', 'sp. z.o.o.', 'sp z o o',  'sp z o.o',  'sp z o.o.',  'sp. z o o',  'sp. z o. o.', 'sp. z o.o',  'sp. z o.o.',  'sp. z. o. o.', 'sp.z o.o'
-                 , 'sp.z o.o.', 's.p. z.o.o.', 's.p. zoo', 'sp zoo.', 'sp. zoo', 'sp. zoo.', 'sp z oo', 'sp zo.o.', 'sp.z.o.o.', 'sp. z o. o', 'spo. z o.o.', 'sp. z o .o.'
-                 , 'sp z o. o', 'sp z.o.o.', 'spolka z o.o.', 'sp. zo.o.', 'sp. z .o.o.', 'sp. z o .o', 'sp. z o . o.', 'sp . sp zoo', 'sp. z.o.o', 'sp. z o', 'sp. z. o.o.'
-                 , 'spolka z ograniczona odpowiedzialnoscia', 'sp. z o.o. 2', 'sp z o. o.', 'sp. z o.o. ul.', 'sp. z o.o. 3', 'sp. z o.o 1', 'sp. z .o.o', 'spolka z o. o.'
-                 , 'spolka z o.o', 'sp.zo.o.', 'sp.zo.o', 'sp. zo. o.', 'sp.z o.', 'sp.z o', 'sp.z.o.o', 'spz o.o.', 'sp.z o. o.', 'sp. z o.o. 4', 'sp. z o.o 2'
-                 , 'sp. z o.o._4', 'sp. z o.o._3', 'sp. z o.o._2', 'sp. z oo']
-    , 'spj': ['spj', 'sp j', 'sp. j', 'sp j.', 'sp.j', 'sp.j.', 'spolka jawna', 'sp. j.', 'sp. jawna']
-    , 'spk': ['spk', 'sp k', 'sp. k', 'sp k.', 'sp.k', 'sp.k.', 'spolka komandytowa', 'sp. k.']
-    # Turkey
-    , 'ltd sti': ['ltd sti', 'ltd. sti.', 'l.t.d. s.t.i.', 'l t g s t i', 'l. t. d. s. t. i.', 'ltdsti', 'ltdsti.', 'l.t.d.s.t.i.', 'ltd. sti', 'ltd sti.'
-                  , 'ltd. sti..', 'ltd.. sti.', 'ltd.sti.', 'ltd.sti']
-    , 'ao': ['ao', 'a.o.','a. o.', 'a o.', 'a. o', 'a o', 'a.o.,', 'a.o. ,', 'a .o.', 'a.o', 'a.o..', 'a.o.,.', 'a.o.,,', 'a.o._2', 'a.o._', 'a..o.', 'a/o'
-             , 'a.o...', 'a..o.', 'ao.']
-    # russia
+                     , 'sp. z.o. sp. k', 'sp. z o.o. spk', 'sp.z o.o. sp.k', 'sp z o.o. sp. k.', 'sp. z o.o. sp. k.a', 'sp.z o.o. sp. k.']
+    , 'sp zoo spj': ['sp zoo spj', 'sp. z.o.o. sp.j', 'sp. z.o.o. sp. j', 'sp. z.o.o. sp. j.', 'sp. z o.o. sp.j.', 'sp. z o.o. sp. j.', 'sp. z o. o. sp. j.']
+    , 'sp zoo ska': ['sp zoo ska', 'sp. z.o.o. s.k.a.', 'sp. z o.o. s. k.a', 'sp. z o.o. s.k.a.',  'sp. z oo s.k.a.', 'sp. z o.o. s.k.', 'sp. z o.o. s.k.a', 'sp. z o. o. ska']
+    , 'sp zoo': ['sp zoo', 'sp. z.o.o.', 'sp z o o',  'sp z o.o',  'sp z o.o.',  'sp. z o o',  'sp. z o. o.', 'sp. z o.o',  'sp. z o.o.',  'sp. z. o. o.', 'sp.z o.o', 'sp.z o.o.'
+                 , 's.p. z.o.o.', 's.p. zoo', 'sp zoo.', 'sp. zoo', 'sp. zoo.', 'sp z oo', 'sp zo.o.', 'sp.z.o.o.', 'sp. z o. o', 'spo. z o.o.', 'sp. z o .o.', 'sp z o. o', 'sp z.o.o.']
+    , 'spj': ['spj', 'sp j', 'sp. j', 'sp j.', 'sp.j', 'sp.j.', 'sp. j.']
+    , 'spk': ['spk', 'sp k', 'sp. k', 'sp k.', 'sp.k', 'sp.k.', 'sp. k.']
+    , 'ltd sti': ['ltd sti', 'ltd. sti.', 'l.t.d. s.t.i.', 'l t g s t i', 'l. t. d. s. t. i.', 'ltdsti', 'ltdsti.', 'l.t.d.s.t.i.', 'ltd. sti', 'ltd sti.', 'ltd.sti.', 'ltd.sti']
     , 'pjsc': ['pjsc', 'p.j.s.c.', 'pjsc.', 'p.j.s.c', 'public joint stock company', 'public joint-stock company']
     , 'ojsc': ['ojsc', 'o.j.s.c.', 'ojsc.', 'o.j.s.c']
     , 'cjsc': ['cjsc', 'c.j.s.c.', 'cjsc.', 'c.j.s.c']
     , 'jsc': ['jsc', 'j.s.c.', 'jsc.', 'j.s.c', 'joint stock company', 'joint-stock company']
     , 'ooo': ['ooo', 'o.o.o.', 'ooo.', 'o.o.o']
     , 'oao': ['oao', 'o.a.o.', 'oao.', 'o.a.o']
     , 'rao': ['rao', 'r.a.o.', 'rao.', 'r.a.o']
     , 'pao': ['pao', 'p.a.o.', 'pao.', 'p.a.o']            
-    # serbia
-    , 'doo': ['doo', 'd.o.o.', 'd.o.o', 'doo.', 'd.o.o. s.k.', 'd o o', 'd. o. o.', 'd.o.o. 6','d.o.o. 1']
-    # qatar
+    , 'doo': ['doo', 'd.o.o.', 'd.o.o', 'doo.', 'd.o.o. s.k.', 'd o o', 'd. o. o.']
     , 'wll': ['wll', 'w.l.l.', 'wll.', 'w.l.l', 'w. l. l.', 'w l l']
-    # hungary
-    , 'nyrt': ['nyrt', 'n.y.r.t.', 'n.y.r.t', 'nyrt.', 'n. y. r. t. ', 'n y r t', 'nyilvanosan mukodo reszvenytarsasag']
-    , 'kft': ['kft', 'kft.', 'k.f.t.', 'k.f.t', 'k. f. t.', 'k f t', 'korlatolt felelossegu tarsasag']
-    , 'zrt': ['zrt', 'zrt.', 'z.r.t.', 'z.r.t', 'z. r. t.', 'z r t', 'zartkoruen mukodo reszvenytarsasag', 'zrt. 2']
-    , 'kkt': ['kkt', 'kkt.', 'k.k.t.', 'k.k.t', 'k. k. t.', 'k k t', 'kozkereseti tarsasag']
-    # greece
+    , 'nyrt': ['nyrt', 'n.y.r.t.', 'n.y.r.t', 'nyrt.', 'n. y. r. t. ', 'n y r t']
+    , 'kft': ['kft', 'kft.', 'k.f.t.', 'k.f.t', 'k. f. t.', 'k f t']
+    , 'zrt': ['zrt', 'zrt.', 'z.r.t.', 'z.r.t', 'z. r. t.', 'z r t']
+    , 'kkt': ['kkt', 'kkt.', 'k.k.t.', 'k.k.t', 'k. k. t.', 'k k t']
     , 'epe': ['epe', 'e.p.e.', 'e.p.e', 'epe.', 'e. p. e.', 'e p e ']
     , 'ae':['ae', 'ae.', 'a.e.', 'a.e', 'a e', 'a. e.']
     , 'oe':['oe', 'oe.', 'o.e.', 'o.e', 'o e', 'o. e.']
     , 'ee':['ee', 'ee.', 'e.e.', 'e.e', 'e e', 'e. e.']
-    # europe
     , 'se': ['se', 's.e.', 'se.', 's.e'] 
-    # others
     , 'vvi': ['vvi', 'v.v.i.', 'v. v. i.', 'v.v.i.,,', 'v.vi.'] 
     , 'z.u.': ['zu', 'z.u.', 'z. u.', 'z u.', 'z. u', 'z u']
 }
 
 # =================================================================================================================================
 # =================================================================================================================================
 # =================================================================================================================================
```

### Comparing `matchmatrix-2.0.1/src/matchmatrix/functions.py` & `matchmatrix-2.0.2/src/matchmatrix/functions.py`

 * *Files identical despite different names*

### Comparing `matchmatrix-2.0.1/src/matchmatrix/manager.py` & `matchmatrix-2.0.2/src/matchmatrix/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -940,15 +940,15 @@
     
         # get the names of the respective join fields as defined in the class's secondary matches (the list of tuples)
         for i, sm in enumerate(self.secondary_matches):
             if sm[6] == secondary_match_name:
                 lookup_join = sm[0] + sm[3]
                 match_join = sm[1] + sm[3] 
         
-        # set frames to merge -- filter for only necessary columns -- means column name changes won't affect originals
+        # create frames to merge -- use copies so column name changes won't affect originals -- and filter for only necessary columns
         left_frame = self.lookup_frame.copy()[[lookup_name, lookup_join, lookup_subset]]
         right_frame = self.match_frame.copy()[[match_name, match_join, match_subset]]
         
         # explode the join field if applicable
         if explode_column == True: 
             left_frame = explode_frame_list_column(left_frame, lookup_join)
             right_frame = explode_frame_list_column(right_frame, match_join)
@@ -991,15 +991,14 @@
     
         # if there are no results then get out since the subsequent code will fail
         if join_matches.shape[0] == 0:
             write_to_log(log_path, 'no additional primary match records identified')
             return pd.DataFrame()
     
         # remove unwanted columns
-        # join_matches = join_matches[['lookup_key', 'match_key', temp_lookup_name, temp_match_name, temp_lookup_name + '_stripped', temp_match_name + '_stripped']]
         join_matches = join_matches[['lookup_key', 'match_key', temp_lookup_name, temp_match_name]]
     
         # remove duplicates
         join_matches = join_matches.drop_duplicates(keep='first')
     
         # add fuzz ratio match score
         vec_fun = np.vectorize(fuzz.ratio)
@@ -1056,15 +1055,17 @@
         
     def integrate_company_suffixes_dictionary(self, d, *, replace=False):
         
         if replace == True:
             self.company_suffixes_dict = d            
         else:
             self.company_suffixes_dict = merge_dictionaries(self.company_suffixes_dict, d)
-    
+        
+        self.company_suffixes_list = convert_dict_to_list(self.company_suffixes_dict)
+            
     def reset_company_suffixes_dictionary(self):
         
         self.company_suffixes_dict = COMPANY_SUFFIXES_DICT
         self.company_suffixes_list = convert_dict_to_list(self.company_suffixes_dict)             
     
     # =============================================================================================================================
     # =============================================================================================================================
```

### Comparing `matchmatrix-2.0.1/src/matchmatrix.egg-info/PKG-INFO` & `matchmatrix-2.0.2/src/matchmatrix.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 Metadata-Version: 2.1
 Name: matchmatrix
-Version: 2.0.1
+Version: 2.0.2
 Summary: Customisable class to produce a matrix of match scores across multiple dimensions
 Home-page: https://github.com/porteverte/matchmatrix
 Author: Porte Verte
 Author-email: Port Verte <porte_verte@outlook.com>
 Project-URL: Homepage, https://github.com/porteverte/matchmatrix
 Project-URL: Issues, https://github.com/porteverte/matchmatrix/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1>About</h1>
+**multimatch | multi-dimensional match scores**
 
-**MultiMatch | Multi-Dimensional Match Scores**
+<h1>About</h1>
 
 How to use this package:
 
 1. Customise the built-in class to generate a matrix of match scores across multiple dimensions.
 2. Apply your own rules to the scores in the matrix as per your specific use-case to identify matches.
 
 Key features:
 
 1. Methods to cleanse and standardise company names.
 2. A method to dedupe data sets and add new IDs.
-3. Functionality to match in subsets to optimise performance.
+3. Functionality to match subsets to optimise performance.
 
 <h1>Dependencies</h1>
 
-**Required**
+**python 3.8 is required for this package**
+
+**Required Packages**
 
 | Package	| Version	| License						|
 |---------------|---------------|-------------------------------------------------------|
 | pandas	| 1.3.5		| BSD License (BSD 3-Clause License			|
 | numpy		| 1.20.3	| BSD License						|
 | rapidfuzz	| 1.9.1		| MIT License (MIT)					|
 | unidecode	| 1.2.0		| GNU General Public License v2 or later (GPLv2+)	|
 
-**Optional**
+**Optional Packages**
 
 | Package	| Version	| License						|
 |---------------|---------------|-------------------------------------------------------|
 | networkx	| TBC		| BSD License						|
 
 <h1>Data Preparation</h1>
 
@@ -82,23 +84,23 @@
     * fuzz.token_set_ratio: set intersection match score
     * set_intersection_match_score: alternative to the above
 3. remove_spaces: True or False (useful for postcodes)
 4. log_path: self explanatory
 
 Example code below.
 
-	# import objects
+	# import match manager class
     from matchmatrix import MatchManager
 
     # optional: create a company suffixes dictionary to integrate with default one
     csd = {'ltd': ['ltd', 'ltd.', 'limited', 'l.i.m.i.t.e.d.', 'limmyted']
           , 'plc': ['plc', 'plc.', 'public limited company', 'pee ell see']
           , 'gmbh': ['gmbh', 'gmbh.']}
     
-    # create class
+    # initialise class
     MyMatch = MatchManager()
     
     # build class
     MyMatch.build_class(
                         # positional arguments
                         lookup_frame, lookup_key, lookup_name
                         , match_frame, match_key, match_name
@@ -108,22 +110,19 @@
                         # , match_function = 'fuzz.ratio'
                         # , remove_spaces = False
                         , log_path=log_path
                         )
 
     # optional: integrate company suffixes dictionary with default one (if defined above)
     # set replace=True to replace the default one completely
-    MyMatch.integrate_company_suffixes_dictionary(csd)    
-    
-    # if necessary re-instate the default dictionary
-    # MyMatch.reset_company_dictionary()
+    MyMatch.integrate_company_suffixes_dictionary(csd)
 
 <h2>Optional (but recommended): define subsetting fields.</h2>
 
-This will do the matching in subsets e.g. county e.g. Yorkshire to Yorkshire to SIGNIFICANTLY speed up processing time.\
+This will do the matching in subsets e.g. county (Yorkshire to Yorkshire etc.) to SIGNIFICANTLY speed up processing time.
 
     MyMatch.subset_fields = ('county_name', 'county_name')
 
 <h2>Optional (but recommended): cleanse the primary matching fields</h2>
 
     MyMatch.cleanse_primary_fields()
     
@@ -135,48 +134,48 @@
     
     initial_results = MyMatch.initial_results
     
 <h2>Optional (but recommended): add secondary matches to the class</h2>
     
 **Positional argugments:**
 
-* lookup_name: name of column to match from in lookup frame.
-* match_name: name of column to match to in match frame.
+* lookup_column: name of column to match from in lookup frame.
+* match_column: name of column to match to in match frame.
 
 **Optional argugments:**
 
 * field_type: same options as primary_field_type above.
 * remove_spaces: as defined above.
 * match_function: as defined above.
 * duplicate_suffix: text to add to a duplicate column e.g. '_stripped'.
 * cleanse_data: True or False.
 * secondary_match_name: a name to refer to later e.g. if doing additional join matches.
 
 Example code below.
     
     MyMatch.clear_secondary_matches()
-    MyMatch.add_secondary_match('address', 'address', field_type='address', cleanse_data=True, secondary_match_name='address')
-    MyMatch.add_secondary_match('postcode', 'postcode', field_type='address', remove_spaces=True, cleanse_data=True, secondary_match_name='postcode')
+    MyMatch.add_secondary_match('first_line_of_address', 'first_line_of_address', field_type='address', cleanse_data=True, secondary_match_name='first_line_of_address')
+    MyMatch.add_secondary_match('post_code', 'post_code', field_type='address', remove_spaces=True, cleanse_data=True, secondary_match_name='post_code')
     
 <h2>Optional: get additional primary matches by joining a pair of secondary match fields</h2>
 
 **Positional arguments:**
 
 * secondary_match_name: the name defined above
     
 **Optional arguments:**
 
 * explode_column: True or False (if a column contains multiple values separated by a comma).
 
 Example code below.
 	
 	# get additional join matches
-    MyMatch.get_additional_join_matches('postcode')
+    MyMatch.get_additional_join_matches('post_code')
 
-<h2>Optional: create and integrate a separate class e.g. a primary match on address.</h2>
+<h2>Optional: create and integrate a separate class e.g. a primary match on first_line_of_address.</h2>
 
 	# to be developed
     
 <h2>Optional: Get secondary matches (if defined above)</h2>
 
     MyMatch.get_secondary_matches()  
 
@@ -184,17 +183,17 @@
     
     initial_results = MyMatch.initial_results
     
 <h2>Identify matches</h2>
 
 Instructions:
 
-1. Apply a series of rules across the different scores in **MyMatch.initial_results** to identify matches.\
+1. Apply a series of rules across the different scores in **MyMatch.initial_results** to identify matches.
 
-2. Create the frame **MyMatch.matched_results** in the class comprising matches ONLY.\
+2. Create the frame **MyMatch.matched_results** in the class comprising matches ONLY.
 
 <h2>Dedupe matched results and add match ids</h2>
 
     # add deduped ids to original keys
     MyMatch.create_deduped_match_ids()
 
     # get xref frame that maps original keys to deduped ids
```

