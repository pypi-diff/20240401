# Comparing `tmp/DataComparerLibrary-0.838.tar.gz` & `tmp/DataComparerLibrary-0.839.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataComparerLibrary-0.838.tar", last modified: Thu Mar 28 13:37:29 2024, max compression
+gzip compressed data, was "DataComparerLibrary-0.839.tar", last modified: Mon Apr  1 20:17:00 2024, max compression
```

## Comparing `DataComparerLibrary-0.838.tar` & `DataComparerLibrary-0.839.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 13:37:29.967607 DataComparerLibrary-0.838/
--rw-rw-rw-   0        0        0    11559 2023-09-04 19:00:59.000000 DataComparerLibrary-0.838/LICENSE.txt
--rw-rw-rw-   0        0        0    11681 2024-03-28 13:37:29.966606 DataComparerLibrary-0.838/PKG-INFO
--rw-rw-rw-   0        0        0    10856 2024-01-12 18:20:20.000000 DataComparerLibrary-0.838/README.rst
--rw-rw-rw-   0        0        0      105 2023-08-26 10:55:42.000000 DataComparerLibrary-0.838/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-28 13:37:29.967607 DataComparerLibrary-0.838/setup.cfg
--rw-rw-rw-   0        0        0     1759 2023-12-30 20:21:07.000000 DataComparerLibrary-0.838/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-28 13:37:29.937599 DataComparerLibrary-0.838/src/
-drwxrwxrwx   0        0        0        0 2024-03-28 13:37:29.957606 DataComparerLibrary-0.838/src/DataComparerLibrary/
--rw-rw-rw-   0        0        0      258 2023-11-18 19:50:29.000000 DataComparerLibrary-0.838/src/DataComparerLibrary/__init__.py
--rw-rw-rw-   0        0        0    25023 2024-03-28 13:36:26.000000 DataComparerLibrary-0.838/src/DataComparerLibrary/datacomparer.py
--rw-rw-rw-   0        0        0     8612 2024-02-11 20:57:49.000000 DataComparerLibrary-0.838/src/DataComparerLibrary/datasorter.py
--rw-rw-rw-   0        0        0      336 2023-11-18 19:57:19.000000 DataComparerLibrary-0.838/src/DataComparerLibrary/delimitertranslator.py
--rw-rw-rw-   0        0        0     2684 2024-01-25 19:44:27.000000 DataComparerLibrary-0.838/src/DataComparerLibrary/fileconverter.py
--rw-rw-rw-   0        0        0       36 2024-03-28 13:35:37.000000 DataComparerLibrary-0.838/src/DataComparerLibrary/version.py
-drwxrwxrwx   0        0        0        0 2024-03-28 13:37:29.965607 DataComparerLibrary-0.838/src/DataComparerLibrary.egg-info/
--rw-rw-rw-   0        0        0    11681 2024-03-28 13:37:29.000000 DataComparerLibrary-0.838/src/DataComparerLibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      485 2024-03-28 13:37:29.000000 DataComparerLibrary-0.838/src/DataComparerLibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 13:37:29.000000 DataComparerLibrary-0.838/src/DataComparerLibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-03-28 13:37:29.000000 DataComparerLibrary-0.838/src/DataComparerLibrary.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-28 13:37:29.963610 DataComparerLibrary-0.838/test/
--rw-rw-rw-   0        0        0     1161 2023-09-19 19:08:19.000000 DataComparerLibrary-0.838/test/test1.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:17:00.469106 DataComparerLibrary-0.839/
+-rw-rw-rw-   0        0        0    11559 2023-09-04 19:00:59.000000 DataComparerLibrary-0.839/LICENSE.txt
+-rw-rw-rw-   0        0        0    11681 2024-04-01 20:17:00.469106 DataComparerLibrary-0.839/PKG-INFO
+-rw-rw-rw-   0        0        0    10856 2024-01-12 18:20:20.000000 DataComparerLibrary-0.839/README.rst
+-rw-rw-rw-   0        0        0      105 2023-08-26 10:55:42.000000 DataComparerLibrary-0.839/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 20:17:00.469106 DataComparerLibrary-0.839/setup.cfg
+-rw-rw-rw-   0        0        0     1759 2023-12-30 20:21:07.000000 DataComparerLibrary-0.839/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:17:00.453481 DataComparerLibrary-0.839/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 20:17:00.453481 DataComparerLibrary-0.839/src/DataComparerLibrary/
+-rw-rw-rw-   0        0        0      258 2023-11-18 19:50:29.000000 DataComparerLibrary-0.839/src/DataComparerLibrary/__init__.py
+-rw-rw-rw-   0        0        0    24860 2024-04-01 20:15:58.000000 DataComparerLibrary-0.839/src/DataComparerLibrary/datacomparer.py
+-rw-rw-rw-   0        0        0     8612 2024-02-11 20:57:49.000000 DataComparerLibrary-0.839/src/DataComparerLibrary/datasorter.py
+-rw-rw-rw-   0        0        0      336 2023-11-18 19:57:19.000000 DataComparerLibrary-0.839/src/DataComparerLibrary/delimitertranslator.py
+-rw-rw-rw-   0        0        0     2684 2024-01-25 19:44:27.000000 DataComparerLibrary-0.839/src/DataComparerLibrary/fileconverter.py
+-rw-rw-rw-   0        0        0      208 2024-04-01 11:47:09.000000 DataComparerLibrary-0.839/src/DataComparerLibrary/tools.py
+-rw-rw-rw-   0        0        0       36 2024-03-28 18:18:33.000000 DataComparerLibrary-0.839/src/DataComparerLibrary/version.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:17:00.469106 DataComparerLibrary-0.839/src/DataComparerLibrary.egg-info/
+-rw-rw-rw-   0        0        0    11681 2024-04-01 20:17:00.000000 DataComparerLibrary-0.839/src/DataComparerLibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2024-04-01 20:17:00.000000 DataComparerLibrary-0.839/src/DataComparerLibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 20:17:00.000000 DataComparerLibrary-0.839/src/DataComparerLibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-01 20:17:00.000000 DataComparerLibrary-0.839/src/DataComparerLibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 20:17:00.469106 DataComparerLibrary-0.839/test/
+-rw-rw-rw-   0        0        0     1161 2023-09-19 19:08:19.000000 DataComparerLibrary-0.839/test/test1.py
```

### Comparing `DataComparerLibrary-0.838/LICENSE.txt` & `DataComparerLibrary-0.839/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DataComparerLibrary-0.838/PKG-INFO` & `DataComparerLibrary-0.839/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataComparerLibrary
-Version: 0.838
+Version: 0.839
 Summary: For comparing csv-files or 2d-array with csv-file.
 Home-page: 
 Author: René Philip Zuijderduijn
 Author-email: datacomparerlibrary@outlook.com
 License: Apache
 Keywords: robotframework testing test-automation datacompare
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `DataComparerLibrary-0.838/README.rst` & `DataComparerLibrary-0.839/README.rst`

 * *Files identical despite different names*

### Comparing `DataComparerLibrary-0.838/setup.py` & `DataComparerLibrary-0.839/setup.py`

 * *Files identical despite different names*

### Comparing `DataComparerLibrary-0.838/src/DataComparerLibrary/datacomparer.py` & `DataComparerLibrary-0.839/src/DataComparerLibrary/datacomparer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import datetime
 import fnmatch
 import os
 import re
 
 import dateutil.relativedelta
 
+from DataComparerLibrary.tools import Tools
+
 
 class DataComparer:
     # Situations:
     # Actual txt file versus expected txt file.
     # Actual csv file versus expected csv file.
     # Array with SQL-output expected csv file.
 
@@ -177,29 +179,23 @@
                             if "{SKIP}" in expected_data_including_templates[row_nr][column_nr].upper() or "{DATETIME_FORMAT():YYYYMMDDHHMMSSFF6}" in expected_data_including_templates[row_nr][column_nr].upper():
                                 if expected_data_including_templates[row_nr][column_nr].upper() == "{SKIP}":
                                     # Complete actual data field will be skipped for verification.
                                     pass
                                 else:
                                     # Part(s) of the actual data field will be skipped for verification.
                                     # Replace {SKIP}, ignoring cases, by wildcard *.
-                                    #compiled = re.compile(re.escape("{SKIP}"), re.IGNORECASE)
-                                    #expected_data_with_wildcard = compiled.sub("*", expected_data_including_templates[row_nr][column_nr])
+                                    # compiled = re.compile(re.escape("{SKIP}"), re.IGNORECASE)
+                                    # expected_data_with_wildcard = compiled.sub("*", expected_data_including_templates[row_nr][column_nr])
                                     compiled = re.compile(re.escape("{SKIP}"), re.IGNORECASE)
                                     compiled2 = re.compile(re.escape("{DATETIME_FORMAT():YYYYMMDDHHMMSSFF6}"), re.IGNORECASE)
                                     expected_data_with_wildcard = compiled2.sub("*", compiled.sub("*", expected_data_including_templates[row_nr][column_nr]))
                                     #
                                     if fnmatch.fnmatch(actual_data[row_nr][column_nr], expected_data_with_wildcard):
                                         skip_exception_rule_used = True
                                         continue
-                                    # This can probably be removed. It is verified further in the code
-#                                    else:
-#                                        # No match despite using of wildcard(s).
-#                                        if "{NOW()" not in expected_data_including_templates[row_nr][column_nr].upper():
-#                                            difference_found = True
-#                                            DataComparer.__print_comparation_result(self, row_nr, column_nr, actual_data[row_nr][column_nr], expected_data_including_templates[row_nr][column_nr], "Actual data field has not been SKIPped.")
                             #
                             if expected_data_with_wildcard is None:
                                 # Wildcards not used.
                                 expected_data_including_date_template = expected_data_including_templates[row_nr][column_nr]
                             else:
                                 expected_data_including_date_template = expected_data_with_wildcard
                             #
@@ -219,24 +215,25 @@
                                     if not fnmatch.fnmatch(actual_data[row_nr][column_nr], expected_data):
                                         # No match despite using of wildcard(s).
                                         difference_found = True
                                         DataComparer.__print_comparation_result(self, row_nr, column_nr, actual_data[row_nr][column_nr], expected_data_including_templates[row_nr][column_nr], "Date template format displayed. See also next message line.")
                                         DataComparer.__print_comparation_result(self, row_nr, column_nr, actual_data[row_nr][column_nr], expected_data, "There is a difference between actual and expected data.")
                                 continue
                                 #
-                            if "{NOT(" in expected_data_including_templates[row_nr][column_nr].upper():
+                            elif "{NOT(" in expected_data_including_templates[row_nr][column_nr].upper():
                                 try:
                                     unwanted_expected_data = DataComparer.__get_unwanted_expected_data(self, expected_data_including_date_template)
                                     #
-                                    if fnmatch.fnmatch(actual_data[row_nr][column_nr], unwanted_expected_data):
+                                    if actual_data[row_nr][column_nr] == unwanted_expected_data:
                                         # Unwanted match.
                                         difference_found = True
                                         DataComparer.__print_comparation_result(self, row_nr, column_nr, actual_data[row_nr][column_nr], expected_data_including_templates[row_nr][column_nr], "NOT() template format displayed. See also next message line.")
                                         DataComparer.__print_comparation_result(self, row_nr, column_nr, actual_data[row_nr][column_nr], unwanted_expected_data, "Actual and expected data are equal. However actual data should NOT be equal to the expected data!!!")
-                                except:
+                                except Exception as exception_message:
+                                    # print(f"An exception occurred: {exception_message}")
                                     difference_found = True
                                     DataComparer.__print_comparation_result(self, row_nr, column_nr, actual_data[row_nr][column_nr], expected_data_including_templates[row_nr][column_nr], "NOT() has been found in expected data field, but format is incorrect.")
                                 #
                             else:
                                 if not skip_exception_rule_used:
                                     # No exceptions.
                                     difference_found = True
@@ -379,10 +376,21 @@
             raise Exception()
         #
         if position_close_brace == -1:
             #print("position_close_brace:", position_close_brace)
             raise Exception()
         #
         unwanted_expected_data = expected_data_field_including_date_template[position_open_brace+5:position_close_brace]
+        #
+        if DataComparer.is_integer(self, unwanted_expected_data):
+            unwanted_expected_data = int(unwanted_expected_data)
         return unwanted_expected_data
 
 
+
+    def is_integer(self, string):
+        if string[0] == '-':
+            # if a negative number
+            return string[1:].isdigit()
+        else:
+            return string.isdigit()
+
```

### Comparing `DataComparerLibrary-0.838/src/DataComparerLibrary/datasorter.py` & `DataComparerLibrary-0.839/src/DataComparerLibrary/datasorter.py`

 * *Files identical despite different names*

### Comparing `DataComparerLibrary-0.838/src/DataComparerLibrary/fileconverter.py` & `DataComparerLibrary-0.839/src/DataComparerLibrary/fileconverter.py`

 * *Files identical despite different names*

### Comparing `DataComparerLibrary-0.838/src/DataComparerLibrary.egg-info/PKG-INFO` & `DataComparerLibrary-0.839/src/DataComparerLibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataComparerLibrary
-Version: 0.838
+Version: 0.839
 Summary: For comparing csv-files or 2d-array with csv-file.
 Home-page: 
 Author: René Philip Zuijderduijn
 Author-email: datacomparerlibrary@outlook.com
 License: Apache
 Keywords: robotframework testing test-automation datacompare
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `DataComparerLibrary-0.838/test/test1.py` & `DataComparerLibrary-0.839/test/test1.py`

 * *Files identical despite different names*

