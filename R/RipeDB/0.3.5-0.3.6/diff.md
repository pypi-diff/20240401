# Comparing `tmp/RipeDB-0.3.5.tar.gz` & `tmp/RipeDB-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RipeDB-0.3.5.tar", last modified: Mon Apr  1 16:51:10 2024, max compression
+gzip compressed data, was "RipeDB-0.3.6.tar", last modified: Mon Apr  1 17:04:35 2024, max compression
```

## Comparing `RipeDB-0.3.5.tar` & `RipeDB-0.3.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-04-01 16:51:10.354908 RipeDB-0.3.5/
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)     1081 2024-02-03 18:25:10.000000 RipeDB-0.3.5/LICENSE
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)     2087 2024-04-01 16:51:10.345834 RipeDB-0.3.5/PKG-INFO
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)     1794 2024-03-29 17:52:53.000000 RipeDB-0.3.5/README.md
-drwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-04-01 16:51:10.338796 RipeDB-0.3.5/RipeDB.egg-info/
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)     2087 2024-04-01 16:51:09.000000 RipeDB-0.3.5/RipeDB.egg-info/PKG-INFO
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)      687 2024-04-01 16:51:09.000000 RipeDB-0.3.5/RipeDB.egg-info/SOURCES.txt
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)        1 2024-04-01 16:51:09.000000 RipeDB-0.3.5/RipeDB.egg-info/dependency_links.txt
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)       44 2024-04-01 16:51:09.000000 RipeDB-0.3.5/RipeDB.egg-info/entry_points.txt
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)       25 2024-04-01 16:51:09.000000 RipeDB-0.3.5/RipeDB.egg-info/requires.txt
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)        7 2024-04-01 16:51:09.000000 RipeDB-0.3.5/RipeDB.egg-info/top_level.txt
-drwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-04-01 16:51:10.068600 RipeDB-0.3.5/ripedb/
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)       13 2024-03-26 09:43:47.000000 RipeDB-0.3.5/ripedb/__init__.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)     7755 2024-03-29 22:08:51.000000 RipeDB-0.3.5/ripedb/main.py
-drwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-04-01 16:51:10.307270 RipeDB-0.3.5/ripedb/utils/
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)       13 2024-03-29 14:12:13.000000 RipeDB-0.3.5/ripedb/utils/__init__.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)      425 2024-03-29 21:11:31.000000 RipeDB-0.3.5/ripedb/utils/expand_ip_range.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)      445 2024-04-01 16:42:48.000000 RipeDB-0.3.5/ripedb/utils/export_xlsx.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)     1292 2024-03-29 21:11:31.000000 RipeDB-0.3.5/ripedb/utils/export_xlsx_new_sheet.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)      566 2024-03-29 21:11:31.000000 RipeDB-0.3.5/ripedb/utils/get_export_path.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)      608 2024-03-29 21:11:31.000000 RipeDB-0.3.5/ripedb/utils/get_ripe_reverse_dns.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)      413 2024-03-29 14:37:33.000000 RipeDB-0.3.5/ripedb/utils/helper.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)     1465 2024-03-29 21:11:31.000000 RipeDB-0.3.5/ripedb/utils/process_input_indixes.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)      626 2024-03-29 21:11:31.000000 RipeDB-0.3.5/ripedb/utils/range_to_cidr.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)      528 2024-03-29 21:11:31.000000 RipeDB-0.3.5/ripedb/utils/remove_lines.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-03-29 21:11:31.000000 RipeDB-0.3.5/ripedb/utils/remove_rows.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)      745 2024-04-01 16:49:03.000000 RipeDB-0.3.5/ripedb/utils/request_and_validate_indices.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)      570 2024-03-29 21:11:31.000000 RipeDB-0.3.5/ripedb/utils/request_confirm.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)      473 2024-03-29 21:11:31.000000 RipeDB-0.3.5/ripedb/utils/reverse_dns.py
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)       38 2024-04-01 16:51:10.354908 RipeDB-0.3.5/setup.cfg
--rwxrwxrwx   0 unknown   (1000) unknown   (1000)      701 2024-04-01 16:50:51.000000 RipeDB-0.3.5/setup.py
+drwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-04-01 17:04:35.360306 RipeDB-0.3.6/
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)     1081 2024-02-03 18:25:10.000000 RipeDB-0.3.6/LICENSE
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)     2087 2024-04-01 17:04:35.354774 RipeDB-0.3.6/PKG-INFO
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)     1794 2024-03-29 17:52:53.000000 RipeDB-0.3.6/README.md
+drwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-04-01 17:04:35.347775 RipeDB-0.3.6/RipeDB.egg-info/
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)     2087 2024-04-01 17:04:34.000000 RipeDB-0.3.6/RipeDB.egg-info/PKG-INFO
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      687 2024-04-01 17:04:34.000000 RipeDB-0.3.6/RipeDB.egg-info/SOURCES.txt
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)        1 2024-04-01 17:04:34.000000 RipeDB-0.3.6/RipeDB.egg-info/dependency_links.txt
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)       44 2024-04-01 17:04:34.000000 RipeDB-0.3.6/RipeDB.egg-info/entry_points.txt
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)       25 2024-04-01 17:04:34.000000 RipeDB-0.3.6/RipeDB.egg-info/requires.txt
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)        7 2024-04-01 17:04:34.000000 RipeDB-0.3.6/RipeDB.egg-info/top_level.txt
+drwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-04-01 17:04:35.110706 RipeDB-0.3.6/ripedb/
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)       13 2024-03-26 09:43:47.000000 RipeDB-0.3.6/ripedb/__init__.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)     7755 2024-04-01 16:58:16.000000 RipeDB-0.3.6/ripedb/main.py
+drwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-04-01 17:04:35.328184 RipeDB-0.3.6/ripedb/utils/
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)       13 2024-03-29 14:12:13.000000 RipeDB-0.3.6/ripedb/utils/__init__.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      425 2024-03-29 21:11:31.000000 RipeDB-0.3.6/ripedb/utils/expand_ip_range.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      445 2024-04-01 16:42:48.000000 RipeDB-0.3.6/ripedb/utils/export_xlsx.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)     1292 2024-03-29 21:11:31.000000 RipeDB-0.3.6/ripedb/utils/export_xlsx_new_sheet.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      566 2024-03-29 21:11:31.000000 RipeDB-0.3.6/ripedb/utils/get_export_path.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      608 2024-03-29 21:11:31.000000 RipeDB-0.3.6/ripedb/utils/get_ripe_reverse_dns.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      413 2024-03-29 14:37:33.000000 RipeDB-0.3.6/ripedb/utils/helper.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)     1465 2024-03-29 21:11:31.000000 RipeDB-0.3.6/ripedb/utils/process_input_indixes.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      626 2024-03-29 21:11:31.000000 RipeDB-0.3.6/ripedb/utils/range_to_cidr.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      528 2024-03-29 21:11:31.000000 RipeDB-0.3.6/ripedb/utils/remove_lines.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)        0 2024-03-29 21:11:31.000000 RipeDB-0.3.6/ripedb/utils/remove_rows.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      785 2024-04-01 17:02:03.000000 RipeDB-0.3.6/ripedb/utils/request_and_validate_indices.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      570 2024-03-29 21:11:31.000000 RipeDB-0.3.6/ripedb/utils/request_confirm.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      473 2024-03-29 21:11:31.000000 RipeDB-0.3.6/ripedb/utils/reverse_dns.py
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)       38 2024-04-01 17:04:35.361306 RipeDB-0.3.6/setup.cfg
+-rwxrwxrwx   0 unknown   (1000) unknown   (1000)      701 2024-04-01 17:03:37.000000 RipeDB-0.3.6/setup.py
```

### Comparing `RipeDB-0.3.5/LICENSE` & `RipeDB-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `RipeDB-0.3.5/PKG-INFO` & `RipeDB-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RipeDB
-Version: 0.3.5
+Version: 0.3.6
 Summary: A tool for making analyssis on RipeDB
 Home-page: https://github.com/apt-0/RipeDB
 Author: APT-0-Blog
 Author-email: cryptovortex@outlook.com
 Keywords: ripe ripedb
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `RipeDB-0.3.5/README.md` & `RipeDB-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `RipeDB-0.3.5/RipeDB.egg-info/PKG-INFO` & `RipeDB-0.3.6/RipeDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RipeDB
-Version: 0.3.5
+Version: 0.3.6
 Summary: A tool for making analyssis on RipeDB
 Home-page: https://github.com/apt-0/RipeDB
 Author: APT-0-Blog
 Author-email: cryptovortex@outlook.com
 Keywords: ripe ripedb
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `RipeDB-0.3.5/RipeDB.egg-info/SOURCES.txt` & `RipeDB-0.3.6/RipeDB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RipeDB-0.3.5/ripedb/main.py` & `RipeDB-0.3.6/ripedb/main.py`

 * *Files identical despite different names*

### Comparing `RipeDB-0.3.5/ripedb/utils/export_xlsx_new_sheet.py` & `RipeDB-0.3.6/ripedb/utils/export_xlsx_new_sheet.py`

 * *Files identical despite different names*

### Comparing `RipeDB-0.3.5/ripedb/utils/get_export_path.py` & `RipeDB-0.3.6/ripedb/utils/get_export_path.py`

 * *Files identical despite different names*

### Comparing `RipeDB-0.3.5/ripedb/utils/get_ripe_reverse_dns.py` & `RipeDB-0.3.6/ripedb/utils/get_ripe_reverse_dns.py`

 * *Files identical despite different names*

### Comparing `RipeDB-0.3.5/ripedb/utils/process_input_indixes.py` & `RipeDB-0.3.6/ripedb/utils/process_input_indixes.py`

 * *Files identical despite different names*

### Comparing `RipeDB-0.3.5/ripedb/utils/range_to_cidr.py` & `RipeDB-0.3.6/ripedb/utils/range_to_cidr.py`

 * *Files identical despite different names*

### Comparing `RipeDB-0.3.5/ripedb/utils/remove_lines.py` & `RipeDB-0.3.6/ripedb/utils/remove_lines.py`

 * *Files identical despite different names*

### Comparing `RipeDB-0.3.5/ripedb/utils/request_and_validate_indices.py` & `RipeDB-0.3.6/ripedb/utils/request_and_validate_indices.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import process_input_indixes
+from ripedb.utils import process_input_indixes
 def request_valid_indixes(max_indice):
     """
     Prompt the user to enter indices or ranges of indices to remove.
 
     Args:
         max_indice (int): The maximum index allowed.
 
@@ -10,12 +10,12 @@
         list: List of valid indices or ranges of indices to remove.
     """
     while True:
         input_utente = input(
             "Enter the index or range of indices to remove (e.g., '3' or '1-3,4-5'), or 'n' to finish:")
         if input_utente.lower() == 'n':
             return []
-        indici_validati = process_input_indixes(input_utente, max_indice)
+        indici_validati = process_input_indixes.process_input_indixes(input_utente, max_indice)
         if indici_validati is not None:
             return indici_validati
         else:
             print("Input not valid. Try again.")
```

### Comparing `RipeDB-0.3.5/ripedb/utils/request_confirm.py` & `RipeDB-0.3.6/ripedb/utils/request_confirm.py`

 * *Files identical despite different names*

### Comparing `RipeDB-0.3.5/setup.py` & `RipeDB-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="RipeDB",
-    version="0.3.5",
+    version="0.3.6",
     packages=find_packages(),
     install_requires=[
         'requests',
         'pandas',
         'openpyxl',
     ],
     entry_points={
```

