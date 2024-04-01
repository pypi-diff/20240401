# Comparing `tmp/shipyard_ftp-0.2.0a6.tar.gz` & `tmp/shipyard_ftp-0.2.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_ftp-0.2.0a6.tar", max compression
+gzip compressed data, was "shipyard_ftp-0.2.0a7.tar", max compression
```

## Comparing `shipyard_ftp-0.2.0a6.tar` & `shipyard_ftp-0.2.0a7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-07-24 19:47:59.858792 shipyard_ftp-0.2.0a6/README.md
--rw-r--r--   0        0        0      538 2024-03-07 16:15:08.782006 shipyard_ftp-0.2.0a6/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-12 18:48:21.830827 shipyard_ftp-0.2.0a6/shipyard_ftp/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.435846 shipyard_ftp-0.2.0a6/shipyard_ftp/cli/__init__.py
--rw-r--r--   0        0        0      736 2024-02-05 20:53:35.436164 shipyard_ftp-0.2.0a6/shipyard_ftp/cli/authtest.py
--rw-r--r--   0        0        0     3378 2024-03-07 16:02:50.146518 shipyard_ftp-0.2.0a6/shipyard_ftp/cli/delete.py
--rw-r--r--   0        0        0     5117 2024-03-07 16:02:50.166560 shipyard_ftp-0.2.0a6/shipyard_ftp/cli/download.py
--rw-r--r--   0        0        0     4225 2024-03-07 16:14:59.219400 shipyard_ftp-0.2.0a6/shipyard_ftp/cli/move.py
--rw-r--r--   0        0        0     4342 2024-03-06 21:15:55.091110 shipyard_ftp-0.2.0a6/shipyard_ftp/cli/upload.py
--rw-r--r--   0        0        0     1266 2024-03-06 20:40:57.854097 shipyard_ftp-0.2.0a6/shipyard_ftp/exceptions.py
--rw-r--r--   0        0        0     7286 2024-03-07 16:08:22.298019 shipyard_ftp-0.2.0a6/shipyard_ftp/ftp.py
--rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 shipyard_ftp-0.2.0a6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-24 19:47:59.858792 shipyard_ftp-0.2.0a7/README.md
+-rw-r--r--   0        0        0      531 2024-03-26 13:29:31.061351 shipyard_ftp-0.2.0a7/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-12 18:48:21.830827 shipyard_ftp-0.2.0a7/shipyard_ftp/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.435846 shipyard_ftp-0.2.0a7/shipyard_ftp/cli/__init__.py
+-rw-r--r--   0        0        0      539 2024-03-14 04:10:23.523728 shipyard_ftp-0.2.0a7/shipyard_ftp/cli/authtest.py
+-rw-r--r--   0        0        0     3526 2024-03-14 04:10:23.524393 shipyard_ftp-0.2.0a7/shipyard_ftp/cli/delete.py
+-rw-r--r--   0        0        0     5838 2024-03-14 04:10:23.524953 shipyard_ftp-0.2.0a7/shipyard_ftp/cli/download.py
+-rw-r--r--   0        0        0     4616 2024-03-26 13:26:23.262083 shipyard_ftp-0.2.0a7/shipyard_ftp/cli/move.py
+-rw-r--r--   0        0        0     3037 2024-03-26 13:24:43.869714 shipyard_ftp-0.2.0a7/shipyard_ftp/cli/upload.py
+-rw-r--r--   0        0        0     1270 2024-03-14 04:10:23.526823 shipyard_ftp-0.2.0a7/shipyard_ftp/exceptions.py
+-rw-r--r--   0        0        0    10073 2024-03-14 04:10:23.527921 shipyard_ftp-0.2.0a7/shipyard_ftp/ftp.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 shipyard_ftp-0.2.0a7/PKG-INFO
```

### Comparing `shipyard_ftp-0.2.0a6/pyproject.toml` & `shipyard_ftp-0.2.0a7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "shipyard-ftp"
-version = "0.2.0a6"
+version = "0.2.0a7"
 description = "A local client for connecting and working with FTP servers"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "shipyard_ftp" }]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.10"
-shipyard-bp-utils = "^1.0.3"
-shipyard-templates = "^0.6.2"
+python = "^3.9"
+shipyard-bp-utils = "^1.2.0"
+shipyard-templates = "^0.8.0"
 
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.1"
 pytest = "^8.0.2"
 
 [build-system]
```

### Comparing `shipyard_ftp-0.2.0a6/shipyard_ftp/cli/delete.py` & `shipyard_ftp-0.2.0a7/shipyard_ftp/cli/delete.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import argparse
 import re
 import sys
 
 from shipyard_bp_utils import files as shipyard
 from shipyard_templates import ShipyardLogger, ExitCodeException, CloudStorage
 
-from shipyard_ftp.exceptions import EXIT_CODE_NO_MATCHES_FOUND
+from shipyard_ftp.exceptions import (
+    EXIT_CODE_NO_MATCHES_FOUND,
+    EXIT_CODE_FTP_DELETE_ERROR,
+)
 from shipyard_ftp.ftp import FtpClient
 
 logger = ShipyardLogger.get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser()
@@ -38,54 +41,58 @@
         host = args.host
         port = args.port
         username = args.username
         password = args.password
         file_name_match_type = args.file_name_match_type
         file_name = args.source_file_name
         folder_name = shipyard.clean_folder_name(args.source_folder_name)
-
+        errors = []
         client = FtpClient(host=host, port=port, user=username, pwd=password)
 
         if file_name_match_type == "regex_match":
             folders = [folder_name]
             files = []
             while folders:
                 folder_filter = folders[0]
 
                 files, folders = client.find_files_in_directory(
-                    folder_filter=folder_filter, files=files, folders=folders)
+                    folder_filter=folder_filter, files=files, folders=folders
+                )
 
             matching_file_names = shipyard.find_all_file_matches(
                 files, re.compile(file_name)
             )
 
-            number_of_matches = len(matching_file_names)
-
-            if number_of_matches == 0:
+            if number_of_matches := len(matching_file_names) == 0:
                 logger.info(f'No matches were found for regex "{file_name}".')
                 sys.exit(EXIT_CODE_NO_MATCHES_FOUND)
 
-            for index, file_name in enumerate(matching_file_names):
-                logger.info(
-                    f"Deleting file {index + 1} of {len(matching_file_names)} out of {number_of_matches}"
-                )
+            for index, file_name in enumerate(matching_file_names, start=1):
+                logger.info(f"Deleting file {index} out of {number_of_matches}")
+
                 try:
                     client.remove(file_name)
                 except Exception:
                     logger.error(f"Failed to delete {file_name}... Skipping")
+                    errors.append(file_name)
+
         elif file_name_match_type == "exact_match":
             file_path = shipyard.combine_folder_and_file_name(folder_name, file_name)
             try:
                 client.remove(file_path)
             except Exception as e:
                 logger.error(
-                    "Most likely, the file name/folder name you specified has typos or the full folder name was not "
-                    "provided. Check these and try again."
+                    "Check the file/folder name for misspellings and ensure that entire folder name was "
+                    "provided"
                 )
                 raise e
+        if errors:
+            logger.error("Failed to delete the following files:\n" + "\n".join(errors))
+            sys.exit(EXIT_CODE_FTP_DELETE_ERROR)
+
     except ExitCodeException as e:
         logger.error(e.message)
         sys.exit(e.exit_code)
     except Exception as e:
         logger.error(f"An unexpected error occurred: {e}")
         sys.exit(CloudStorage.EXIT_CODE_UNKNOWN_ERROR)
```

### Comparing `shipyard_ftp-0.2.0a6/shipyard_ftp/cli/download.py` & `shipyard_ftp-0.2.0a7/shipyard_ftp/cli/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 import re
 import sys
 
 from shipyard_bp_utils import files as shipyard
 from shipyard_templates import ExitCodeException, CloudStorage
 from shipyard_templates.shipyard_logger import ShipyardLogger
 
+from shipyard_ftp.exceptions import EXIT_CODE_NO_MATCHES_FOUND, EXIT_CODE_DOWNLOAD_ERROR
 from shipyard_ftp.ftp import FtpClient
 
 logger = ShipyardLogger().get_logger()
 
-EXIT_CODE_INCORRECT_CREDENTIALS = 3
-EXIT_CODE_NO_MATCHES_FOUND = 200
-
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--source-file-name-match-type",
         dest="source_file_name_match_type",
         choices={"exact_match", "regex_match"},
@@ -67,66 +65,84 @@
         password = args.password
         source_file_name = args.source_file_name
         source_folder_name = shipyard.clean_folder_name(args.source_folder_name)
         source_full_path = shipyard.combine_folder_and_file_name(
             folder_name=source_folder_name, file_name=source_file_name
         )
         source_file_name_match_type = args.source_file_name_match_type
-
-        destination_folder_name = shipyard.clean_folder_name(args.destination_folder_name)
+        destination_folder_name = shipyard.clean_folder_name(
+            args.destination_folder_name
+        )
+        errors = []
         if destination_folder_name:
             shipyard.create_folder_if_dne(destination_folder_name)
         client = FtpClient(host=host, port=port, user=username, pwd=password)
 
         logger.info("Beginning the download process...")
         if source_file_name_match_type == "exact_match":
             try:
                 destination_name = shipyard.determine_destination_full_path(
                     destination_folder_name=destination_folder_name,
                     destination_file_name=args.destination_file_name,
-                    source_full_path=source_full_path)
+                    source_full_path=source_full_path,
+                )
                 client.download(source_full_path, destination_name)
 
             except Exception as e:
-                logger.error(f"Failed to download {source_full_path} due to {e}\n"
-                             f"Most likely, the file name/folder name you specified has typos or the full folder name was "
-                             f"not provided. Check these and try again.")
+                logger.error(
+                    f"Failed to download {source_full_path} due to {e}\n"
+                    f"Most likely, the file name/folder name you specified has typos or the full folder name was "
+                    f"not provided. Check these and try again."
+                )
                 raise e
         elif source_file_name_match_type == "regex_match":
             folders = [source_folder_name]
             files = []
             while folders:
                 folder_filter = folders[0]
                 files, folders = client.find_files_in_directory(
                     folder_filter=folder_filter, files=files, folders=folders
                 )
 
-            matching_file_names = shipyard.find_all_file_matches(files, re.compile(source_file_name))
+            matching_file_names = shipyard.find_all_file_matches(
+                files, re.compile(source_file_name)
+            )
 
-            number_of_matches = len(matching_file_names)
-
-            if number_of_matches == 0:
+            if number_of_matches := len(matching_file_names) == 0:
                 logger.info(f'No matches were found for regex "{source_file_name}".')
                 sys.exit(EXIT_CODE_NO_MATCHES_FOUND)
 
-            logger.info(f"{len(matching_file_names)} files found. Preparing to download...")
-
-            for index, file_name in enumerate(matching_file_names):
+            logger.info(f"{number_of_matches} files found. Preparing to download...")
+            for index, file_name in enumerate(matching_file_names, start=1):
                 destination_name = shipyard.determine_destination_full_path(
                     destination_folder_name=destination_folder_name,
                     destination_file_name=args.destination_file_name,
                     source_full_path=file_name,
-                    file_number=index + 1,
+                    file_number=index if number_of_matches > 1 else None,
                 )
 
-                logger.info(f"Downloading file {index + 1} of {len(matching_file_names)}")
-
-                client.download(file_name, destination_name)
+                logger.info(
+                    f"Attempting to download file {index} of {number_of_matches}: {file_name} to {destination_name}..."
+                )
+                try:
+                    client.download(file_name, destination_name)
+                    logger.info(
+                        f"Successfully downloaded {file_name} to {destination_name}."
+                    )
+                except Exception as e:
+                    logger.error(f"Failed to download {file_name} due to {e}")
+                    errors.append(file_name)
 
         logger.info("Download process complete.")
+
+        if errors:
+            logger.error(
+                "Failed to download the following files:\n" + "\n".join(errors)
+            )
+            sys.exit(EXIT_CODE_DOWNLOAD_ERROR)
     except ExitCodeException as e:
         logger.error(e.message)
         sys.exit(e.exit_code)
     except Exception as e:
         logger.error(f"An error occurred during the download process: {e}")
         sys.exit(CloudStorage.EXIT_CODE_UNKNOWN_ERROR)
```

### Comparing `shipyard_ftp-0.2.0a6/shipyard_ftp/cli/move.py` & `shipyard_ftp-0.2.0a7/shipyard_ftp/cli/move.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import re
 import sys
 
 from shipyard_bp_utils import files as shipyard
-from shipyard_templates import ShipyardLogger
+from shipyard_templates import ShipyardLogger, ExitCodeException, CloudStorage
 
 from shipyard_ftp.ftp import FtpClient
 
 logger = ShipyardLogger.get_logger()
 
 
 def get_args():
@@ -39,75 +39,77 @@
     parser.add_argument("--port", dest="port", default=21, required=True)
     parser.add_argument("--username", dest="username", default=None, required=False)
     parser.add_argument("--password", dest="password", default=None, required=False)
     return parser.parse_args()
 
 
 def main():
-    args = get_args()
-    host = args.host
-    port = args.port
-    username = args.username
-    password = args.password
-    source_file_name = args.source_file_name
-    source_folder_name = args.source_folder_name
-
-    destination_folder_name = shipyard.clean_folder_name(
-        args.destination_folder_name
-    )
-    source_file_name_match_type = args.source_file_name_match_type
-    ftp_client = FtpClient(host=host, port=port, user=username, pwd=password)
-    # if the source folder name is omitted, then use the current working directory
-    source_folder_name = source_folder_name or ftp_client.client.pwd()
-    if source_file_name_match_type == "exact_match":
-        source_full_path = shipyard.combine_folder_and_file_name(
-            source_folder_name, source_file_name
-        )
-        destination_file = shipyard.determine_destination_file_name(
-            source_full_path=source_full_path,
-            destination_file_name=args.destination_file_name,
-        )
-        destination_full_path = shipyard.combine_folder_and_file_name(
-            destination_folder_name,
-            destination_file,
-        )
-        if len(destination_full_path.split("/")) > 1:
-            path, file_name = destination_full_path.rsplit("/", 1)
-            ftp_client.create_new_folders(destination_path=path)
-        ftp_client.move(
-            source_full_path=source_full_path,
-            destination_full_path=destination_full_path,
-        )
-
-
-    elif source_file_name_match_type == "regex_match":
-        file_names = ftp_client.get_all_nested_items(source_folder_name)
-        matching_file_names = shipyard.find_all_file_matches(
-            file_names, re.compile(source_file_name)
-        )
-
-        number_of_matches = len(matching_file_names)
-
-        if number_of_matches == 0:
-            logger.info(f'No matches were found for regex "{source_file_name}".')
-            sys.exit(ftp_client.EXIT_CODE_FILE_MATCH_ERROR)
-
-        logger.info(f"{len(matching_file_names)} files found. Preparing to move...")
-
-        for index, key_name in enumerate(matching_file_names, 1):
-            destination_full_path = shipyard.determine_destination_full_path(
-                destination_folder_name=destination_folder_name,
+    try:
+        args = get_args()
+        host = args.host
+        port = args.port
+        username = args.username
+        password = args.password
+        source_file_name = args.source_file_name
+        source_folder_name = args.source_folder_name
+
+        destination_folder_name = shipyard.clean_folder_name(args.destination_folder_name)
+        source_file_name_match_type = args.source_file_name_match_type
+        ftp_client = FtpClient(host=host, port=port, user=username, pwd=password)
+        # if the source folder name is omitted, then use the current working directory
+        source_folder_name = source_folder_name or ftp_client.client.pwd()
+        if source_file_name_match_type == "exact_match":
+            source_full_path = shipyard.combine_folder_and_file_name(
+                source_folder_name, source_file_name
+            )
+            destination_file = shipyard.determine_destination_file_name(
+                source_full_path=source_full_path,
                 destination_file_name=args.destination_file_name,
-                source_full_path=key_name,
-                file_number=None if len(matching_file_names) == 1 else index,
+            )
+            destination_full_path = shipyard.combine_folder_and_file_name(
+                destination_folder_name, destination_file
             )
             if len(destination_full_path.split("/")) > 1:
                 path, file_name = destination_full_path.rsplit("/", 1)
-                ftp_client.create_new_folders(path)
-            logger.info(f"Moving file {index} of {len(matching_file_names)}")
+                ftp_client.create_new_folders(destination_path=path)
             ftp_client.move(
-                source_full_path=key_name, destination_full_path=destination_full_path
+                source_full_path=source_full_path,
+                destination_full_path=destination_full_path,
             )
 
+        elif source_file_name_match_type == "regex_match":
+            file_names = ftp_client.get_all_nested_items(source_folder_name)
+            matching_file_names = shipyard.find_all_file_matches(
+                file_names, re.compile(source_file_name)
+            )
+
+            if (number_of_matches := len(matching_file_names)) == 0:
+                logger.error(f'No matches were found for regex "{source_file_name}".')
+                sys.exit(ftp_client.EXIT_CODE_FILE_MATCH_ERROR)
+
+            logger.info(f"{number_of_matches} files found. Preparing to move...")
+
+            for index, key_name in enumerate(matching_file_names, start=1):
+                destination_full_path = shipyard.determine_destination_full_path(
+                    destination_folder_name=destination_folder_name,
+                    destination_file_name=args.destination_file_name,
+                    source_full_path=key_name,
+                    file_number=index if number_of_matches > 1 else None,
+                )
+                if len(destination_full_path.split("/")) > 1:
+                    path, file_name = destination_full_path.rsplit("/", 1)
+                    ftp_client.create_new_folders(path)
+
+                logger.info(f"Moving file {index} of {number_of_matches}")
+                ftp_client.move(
+                    source_full_path=key_name, destination_full_path=destination_full_path
+                )
+    except ExitCodeException as e:
+        logger.error(e.message)
+        sys.exit(e.exit_code)
+    except Exception as e:
+        logger.error(e)
+        sys.exit(CloudStorage.EXIT_CODE_UNKNOWN_ERROR)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_ftp-0.2.0a6/shipyard_ftp/cli/upload.py` & `shipyard_ftp-0.2.0a7/shipyard_ftp/cli/upload.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import argparse
-import os
-import re
 import sys
 
 from shipyard_bp_utils import files as shipyard
 from shipyard_templates import ShipyardLogger, ExitCodeException, CloudStorage
 
 from shipyard_ftp.ftp import FtpClient
 
@@ -41,68 +39,42 @@
     parser.add_argument("--password", dest="password", default=None, required=False)
     return parser.parse_args()
 
 
 def main():
     try:
         args = get_args()
-        host = args.host
-        port = args.port
-        username = args.username
-        password = args.password
+
         source_file_name = args.source_file_name
         source_folder_name = args.source_folder_name
         destination_filename = args.destination_file_name or source_file_name
         destination_folder_name = shipyard.clean_folder_name(args.destination_folder_name)
-        source_file_name_match_type = args.source_file_name_match_type
-        ftp_client = FtpClient(host=host, port=port, user=username, pwd=password)
-        if source_file_name_match_type == "exact_match":
-            source_full_path = shipyard.combine_folder_and_file_name(
-                folder_name=f"{os.getcwd()}/{source_folder_name}", file_name=source_file_name
-            )
-            destination_full_path = shipyard.determine_destination_full_path(
-                destination_folder_name=destination_folder_name,
-                destination_file_name=destination_filename,
-                source_full_path=source_full_path,
-            )
+
+        ftp_client = FtpClient(host=args.host, port=args.port, user=args.username, pwd=args.password)
+        files = shipyard.file_match(search_term=source_file_name,
+                                    files=shipyard.fetch_file_paths_from_directory(source_folder_name),
+                                    source_directory=source_folder_name,
+                                    destination_directory=destination_folder_name,
+                                    destination_filename=destination_filename,
+                                    match_type=args.source_file_name_match_type)
+
+        for file in files:
+            source_file = file['source_path']
+            destination_full_path = file['destination_filename']
             if len(destination_full_path.split("/")) > 1:
                 path, file_name = destination_full_path.rsplit("/", 1)
                 ftp_client.create_new_folders(path)
+            ftp_client.upload(source_file, destination_full_path)
 
-            ftp_client.upload(source_full_path, destination_full_path)
-
-        elif source_file_name_match_type == "regex_match":
-            file_names = shipyard.find_all_local_file_names(source_folder_name)
-            matching_file_names = shipyard.find_all_file_matches(
-                file_names, re.compile(source_file_name)
-            )
-
-            number_of_matches = len(matching_file_names)
-
-            if number_of_matches == 0:
-                logger.error(f'No matches were found for regex "{source_file_name}".')
-                sys.exit(ftp_client.EXIT_CODE_FILE_MATCH_ERROR)
-
-            logger.info(f"{len(matching_file_names)} files found. Preparing to upload...")
-
-            for index, key_name in enumerate(matching_file_names):
-                destination_full_path = shipyard.determine_destination_full_path(
-                    destination_folder_name=destination_folder_name,
-                    destination_file_name=destination_filename,
-                    source_full_path=key_name,
-                    file_number=index + 1,
-                )
-                if len(destination_full_path.split("/")) > 1:
-                    path, file_name = destination_full_path.rsplit("/", 1)
-                    ftp_client.create_new_folders(destination_path=path)
-                logger.info(f"Uploading file {index + 1} of {len(matching_file_names)}")
-                ftp_client.upload(key_name, destination_full_path)
     except ExitCodeException as e:
         logger.error(e.message)
         sys.exit(e.exit_code)
+    except FileNotFoundError as e:
+        logger.error(f"File not found: {e}")
+        sys.exit(CloudStorage.EXIT_CODE_FILE_MATCH_ERROR)
     except Exception as e:
         logger.error(f"An error occurred: {e}")
         sys.exit(CloudStorage.EXIT_CODE_UNKNOWN_ERROR)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_ftp-0.2.0a6/shipyard_ftp/exceptions.py` & `shipyard_ftp-0.2.0a7/shipyard_ftp/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 logger = ShipyardLogger().get_logger()
 EXIT_CODE_FTP_MOVE_ERROR = 100
 EXIT_CODE_FTP_DELETE_ERROR = 101
 EXIT_CODE_UPLOAD_ERROR = CloudStorage.EXIT_CODE_UPLOAD_ERROR
 EXIT_CODE_NO_MATCHES_FOUND = CloudStorage.EXIT_CODE_FILE_MATCH_ERROR
 EXIT_CODE_INCORRECT_CREDENTIALS = CloudStorage.EXIT_CODE_INVALID_CREDENTIALS
-EXIT_CODE_DOWNLOAD_ERROR= CloudStorage.EXIT_CODE_DOWNLOAD_ERROR
+EXIT_CODE_DOWNLOAD_ERROR = CloudStorage.EXIT_CODE_DOWNLOAD_ERROR
 
 
 class MoveError(ExitCodeException):
     def __init__(self, message):
         super().__init__(message, EXIT_CODE_FTP_MOVE_ERROR)
 
 
@@ -19,19 +19,21 @@
         super().__init__(message, EXIT_CODE_UPLOAD_ERROR)
 
 
 class NoMatchFound(ExitCodeException):
     def __init__(self, message):
         super().__init__(message, EXIT_CODE_NO_MATCHES_FOUND)
 
+
 class InvalidCredentials(ExitCodeException):
     def __init__(self, message):
         super().__init__(message, EXIT_CODE_INCORRECT_CREDENTIALS)
 
+
 class DownloadError(ExitCodeException):
     def __init__(self, message):
         super().__init__(message, EXIT_CODE_DOWNLOAD_ERROR)
 
 
 class DeleteError(ExitCodeException):
     def __init__(self, message):
-        super().__init__(message, EXIT_CODE_FTP_DELETE_ERROR)
+        super().__init__(message, EXIT_CODE_FTP_DELETE_ERROR)
```

### Comparing `shipyard_ftp-0.2.0a6/PKG-INFO` & `shipyard_ftp-0.2.0a7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: shipyard-ftp
-Version: 0.2.0a6
+Version: 0.2.0a7
 Summary: A local client for connecting and working with FTP servers
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
-Requires-Python: >=3.9,<3.10
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: shipyard-bp-utils (>=1.0.3,<2.0.0)
-Requires-Dist: shipyard-templates (>=0.6.2,<0.7.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: shipyard-bp-utils (>=1.2.0,<2.0.0)
+Requires-Dist: shipyard-templates (>=0.8.0,<0.9.0)
 Description-Content-Type: text/markdown
```

