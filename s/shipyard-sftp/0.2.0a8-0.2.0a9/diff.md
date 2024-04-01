# Comparing `tmp/shipyard_sftp-0.2.0a8.tar.gz` & `tmp/shipyard_sftp-0.2.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_sftp-0.2.0a8.tar", max compression
+gzip compressed data, was "shipyard_sftp-0.2.0a9.tar", max compression
```

## Comparing `shipyard_sftp-0.2.0a8.tar` & `shipyard_sftp-0.2.0a9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-05-12 18:48:21.840614 shipyard_sftp-0.2.0a8/README.md
--rw-r--r--   0        0        0      553 2024-03-29 16:11:15.459903 shipyard_sftp-0.2.0a8/pyproject.toml
--rw-r--r--   0        0        0        1 2024-03-06 14:22:56.719708 shipyard_sftp-0.2.0a8/shipyard_sftp/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 03:34:57.761954 shipyard_sftp-0.2.0a8/shipyard_sftp/cli/__init__.py
--rw-r--r--   0        0        0      474 2024-03-06 14:22:56.720339 shipyard_sftp-0.2.0a8/shipyard_sftp/cli/authtest.py
--rw-r--r--   0        0        0     3190 2024-03-29 15:30:29.281833 shipyard_sftp-0.2.0a8/shipyard_sftp/cli/delete_file.py
--rw-r--r--   0        0        0     3385 2024-03-29 15:30:29.282700 shipyard_sftp-0.2.0a8/shipyard_sftp/cli/download_file.py
--rw-r--r--   0        0        0     3851 2024-03-29 16:03:14.516306 shipyard_sftp-0.2.0a8/shipyard_sftp/cli/move_file.py
--rw-r--r--   0        0        0     3211 2024-03-29 15:30:29.284338 shipyard_sftp-0.2.0a8/shipyard_sftp/cli/upload_file.py
--rw-r--r--   0        0        0     3387 2024-03-29 15:30:29.284848 shipyard_sftp-0.2.0a8/shipyard_sftp/exceptions.py
--rw-r--r--   0        0        0    13970 2024-03-29 16:02:38.520093 shipyard_sftp-0.2.0a8/shipyard_sftp/sftp.py
--rw-r--r--   0        0        0     1681 2024-03-29 15:30:29.285682 shipyard_sftp-0.2.0a8/shipyard_sftp/utils.py
--rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 shipyard_sftp-0.2.0a8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:21.840614 shipyard_sftp-0.2.0a9/README.md
+-rw-r--r--   0        0        0      553 2024-04-01 20:31:48.503564 shipyard_sftp-0.2.0a9/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-03-06 14:22:56.719708 shipyard_sftp-0.2.0a9/shipyard_sftp/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.761954 shipyard_sftp-0.2.0a9/shipyard_sftp/cli/__init__.py
+-rw-r--r--   0        0        0      474 2024-03-06 14:22:56.720339 shipyard_sftp-0.2.0a9/shipyard_sftp/cli/authtest.py
+-rw-r--r--   0        0        0     3345 2024-04-01 20:25:50.307269 shipyard_sftp-0.2.0a9/shipyard_sftp/cli/delete_file.py
+-rw-r--r--   0        0        0     3777 2024-04-01 20:25:50.315904 shipyard_sftp-0.2.0a9/shipyard_sftp/cli/download_file.py
+-rw-r--r--   0        0        0     3728 2024-04-01 20:25:50.324994 shipyard_sftp-0.2.0a9/shipyard_sftp/cli/move_file.py
+-rw-r--r--   0        0        0     3395 2024-04-01 20:25:50.320567 shipyard_sftp-0.2.0a9/shipyard_sftp/cli/upload_file.py
+-rw-r--r--   0        0        0     3387 2024-03-29 15:30:29.284848 shipyard_sftp-0.2.0a9/shipyard_sftp/exceptions.py
+-rw-r--r--   0        0        0    13970 2024-04-01 15:54:40.972677 shipyard_sftp-0.2.0a9/shipyard_sftp/sftp.py
+-rw-r--r--   0        0        0     1638 2024-04-01 19:49:20.622350 shipyard_sftp-0.2.0a9/shipyard_sftp/utils.py
+-rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 shipyard_sftp-0.2.0a9/PKG-INFO
```

### Comparing `shipyard_sftp-0.2.0a8/pyproject.toml` & `shipyard_sftp-0.2.0a9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-sftp"
-version = "0.2.0a8"
+version = "0.2.0a9"
 description = "A local client for connecting and working with SFTP servers"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "shipyard_sftp" }]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_sftp-0.2.0a8/shipyard_sftp/cli/delete_file.py` & `shipyard_sftp-0.2.0a9/shipyard_sftp/cli/delete_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,19 @@
         source_file_name = args.source_file_name
         source_folder_name = shipyard.clean_folder_name(args.source_folder_name)
         source_full_path = shipyard.combine_folder_and_file_name(
             source_folder_name, source_file_name
         )
         source_file_name_match_type = args.source_file_name_match_type or "exact_match"
 
-        if source_file_name_match_type == "regex_match":
+        if source_file_name_match_type == "exact_match":
+            logger.info(f"Attempting to delete file {source_full_path}...")
+            sftp.remove(source_full_path)
+            logger.info(f"File {source_full_path} deleted successfully")
+        elif source_file_name_match_type == "regex_match":
             file_names = sftp.list_files_recursive(source_folder_name or ".")
             matching_file_names = shipyard.find_all_file_matches(
                 file_names, re.compile(source_file_name)
             )
             if len(matching_file_names) == 0:
                 raise ExitCodeException(
                     "No matches found", sftp.EXIT_CODE_FILE_NOT_FOUND
@@ -67,17 +71,15 @@
             for index, file_name in enumerate(matching_file_names, 1):
                 delete_file_path = file_name
 
                 logger.info(f"Deleting file {index} of {len(matching_file_names)}")
                 try:
                     sftp.remove(delete_file_path)
                 except Exception as e:
-                    print(f"Failed to delete {file_name} due to {e}... Skipping")
-        elif source_file_name_match_type == "exact_match":
-            sftp.remove(source_full_path)
+                    logger.info(f"Failed to delete {file_name} due to {e}... Skipping")
     except ExitCodeException as e:
         logger.error(e)
         exit_code = e.exit_code
     except Exception as e:
         logger.error(e)
         exit_code = CloudStorage.EXIT_CODE_UNKNOWN_ERROR
     finally:
```

### Comparing `shipyard_sftp-0.2.0a8/shipyard_sftp/cli/download_file.py` & `shipyard_sftp-0.2.0a9/shipyard_sftp/cli/download_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,19 @@
         source_file_name_match_type = args.source_file_name_match_type or "exact_match"
 
         destination_folder_name = shipyard.clean_folder_name(
             args.destination_folder_name
         )
         shipyard.create_folder_if_dne(destination_folder_name)
         sftp_files_full_paths = sftp.list_files_recursive(source_folder_name or ".")
+        if not sftp_files_full_paths:
+            raise ExitCodeException(
+                f"No files found in source folder {source_folder_name}",
+                CloudStorage.EXIT_CODE_FILE_NOT_FOUND,
+            )
 
         # Get the relative path of the files which is the format that shipyard.file_match expects
         sftp_files = [
             os.path.relpath(path, start=source_folder_name)
             for path in sftp_files_full_paths
         ]
 
@@ -76,15 +81,17 @@
             destination_filename=args.destination_file_name,
             match_type=source_file_name_match_type,
         )
 
         for file in files:
             source_file = file["source_path"]
             destination_full_path = file["destination_filename"]
+            logger.info(f"Attempting to download {source_file} to {destination_full_path}...")
             sftp.download(source_file, destination_full_path)
+            logger.info(f"Downloaded {source_file} to {destination_full_path}")
 
     except ExitCodeException as e:
         logger.error(e)
         exit_code = e.exit_code
     except FileNotFoundError as e:
         logger.error(e)
         exit_code = CloudStorage.EXIT_CODE_FILE_NOT_FOUND
```

### Comparing `shipyard_sftp-0.2.0a8/shipyard_sftp/cli/move_file.py` & `shipyard_sftp-0.2.0a9/shipyard_sftp/cli/move_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argparse
-import re
+import os.path
 import sys
 
 from shipyard_bp_utils import files as shipyard
 from shipyard_templates import CloudStorage, ExitCodeException
 from shipyard_templates.shipyard_logger import ShipyardLogger
 
 from shipyard_sftp.sftp import SftpClient
@@ -50,52 +50,54 @@
     sftp = None
     exit_code = 0
     try:
         args = get_args()
         connection_args, key_path = setup_connection(args)
         sftp = SftpClient(**connection_args)
 
-        source_file_name = args.source_file_name
-        source_folder_name = args.source_folder_name
-        source_full_path = shipyard.combine_folder_and_file_name(
-            source_folder_name, source_file_name
-        )
+        source_folder_name = args.source_folder_name or "."
+
         destination_folder_name = shipyard.clean_folder_name(
             args.destination_folder_name
         )
-        source_file_name_match_type = args.source_file_name_match_type or "exact_match"
-
-        if source_file_name_match_type == "exact_match":
-            destination_full_path = shipyard.determine_destination_full_path(
-                destination_folder_name=destination_folder_name,
-                destination_file_name=args.destination_file_name,
-                source_full_path=source_full_path,
-            )
-            sftp.move(source_full_path, destination_full_path)
+        logger.debug(f"Source folder name: {source_folder_name}")
 
-        elif source_file_name_match_type == "regex_match":
-            file_names = sftp.list_files_recursive(source_folder_name or ".")
-            matching_file_names = shipyard.find_all_file_matches(
-                file_names, re.compile(source_file_name)
+        sftp_files_full_paths = sftp.list_files_recursive(source_folder_name or ".")
+        if not sftp_files_full_paths:
+            raise ExitCodeException(
+                f"No files found in the folder {source_folder_name}",
+                CloudStorage.EXIT_CODE_FILE_NOT_FOUND,
             )
-            logger.info(f"{len(matching_file_names)} files found. Preparing to move...")
+        # Get the relative path of the files which is the format that shipyard.file_match expects
+        sftp_files = [
+            os.path.relpath(path, start=source_folder_name)
+            for path in sftp_files_full_paths
+        ]
+        files = shipyard.file_match(
+            search_term=args.source_file_name,
+            files=sftp_files,
+            source_directory=source_folder_name,
+            destination_directory=destination_folder_name,
+            destination_filename=args.destination_file_name,
+            match_type=args.source_file_name_match_type or "exact_match",
+        )
 
-            for index, key_name in enumerate(matching_file_names, 1):
-                destination_full_path = shipyard.determine_destination_full_path(
-                    destination_folder_name=destination_folder_name,
-                    destination_file_name=args.destination_file_name,
-                    source_full_path=key_name,
-                    file_number=None if len(matching_file_names) == 1 else index,
-                )
+        for file in files:
+            source_file = file["source_path"]
+            destination_full_path = file["destination_filename"]
+            logger.info(f"Attempting to move {source_file} to {destination_full_path}...")
+            sftp.move(source_file, destination_full_path)
+            logger.info(f"Successfully moved {source_file} to {destination_full_path}")
 
-                logger.info(f"Moving file {index} of {len(matching_file_names)}")
-                sftp.move(key_name, destination_full_path)
     except ExitCodeException as e:
         logger.error(e)
         exit_code = e.exit_code
+    except FileNotFoundError as e:
+        logger.error(e)
+        exit_code = CloudStorage.EXIT_CODE_FILE_MATCH_ERROR
     except Exception as e:
         logger.error(e)
         exit_code = CloudStorage.EXIT_CODE_UNKNOWN_ERROR
     finally:
         tear_down(key_path, sftp)
         sys.exit(exit_code)
```

### Comparing `shipyard_sftp-0.2.0a8/shipyard_sftp/cli/upload_file.py` & `shipyard_sftp-0.2.0a9/shipyard_sftp/cli/upload_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,17 @@
         for file in files:
             source_file = file["source_path"]
             destination_full_path = file["destination_filename"]
             if not os.path.isfile(source_file):
                 raise ExitCodeException(
                     f"{source_file} is not a file", sftp.EXIT_CODE_FILE_MATCH_ERROR
                 )
+            logger.info(f"Attempting to upload {source_file} to {destination_full_path}...")
             sftp.upload(source_file, destination_full_path)
+            logger.info(f"Successfully uploaded {source_file} to {destination_full_path}")
 
     except ExitCodeException as e:
         logger.error(e)
         exit_code = e.exit_code
     except FileNotFoundError as e:
         logger.error(e)
         exit_code = CloudStorage.EXIT_CODE_FILE_NOT_FOUND
```

### Comparing `shipyard_sftp-0.2.0a8/shipyard_sftp/exceptions.py` & `shipyard_sftp-0.2.0a9/shipyard_sftp/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_sftp-0.2.0a8/shipyard_sftp/sftp.py` & `shipyard_sftp-0.2.0a9/shipyard_sftp/sftp.py`

 * *Files identical despite different names*

### Comparing `shipyard_sftp-0.2.0a8/shipyard_sftp/utils.py` & `shipyard_sftp-0.2.0a9/shipyard_sftp/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import argparse
 import contextlib
 import os
 import tempfile
 
 from shipyard_templates import CloudStorage, ExitCodeException, ShipyardLogger
 
-from shipyard_sftp.sftp import SftpClient
-
 logger = ShipyardLogger().get_logger()
 
 
 def setup_connection(args: argparse.Namespace) -> tuple:
     """
     Return connection arguments and the path to the private key file if it was created
```

### Comparing `shipyard_sftp-0.2.0a8/PKG-INFO` & `shipyard_sftp-0.2.0a9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-sftp
-Version: 0.2.0a8
+Version: 0.2.0a9
 Summary: A local client for connecting and working with SFTP servers
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

