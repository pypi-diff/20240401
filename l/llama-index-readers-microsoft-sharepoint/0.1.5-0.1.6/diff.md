# Comparing `tmp/llama_index_readers_microsoft_sharepoint-0.1.5.tar.gz` & `tmp/llama_index_readers_microsoft_sharepoint-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_microsoft_sharepoint-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_readers_microsoft_sharepoint-0.1.6.tar", max compression
```

## Comparing `llama_index_readers_microsoft_sharepoint-0.1.5.tar` & `llama_index_readers_microsoft_sharepoint-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1782 2024-03-31 17:05:15.790447 llama_index_readers_microsoft_sharepoint-0.1.5/README.md
--rw-r--r--   0        0        0      107 2024-03-31 17:05:15.790447 llama_index_readers_microsoft_sharepoint-0.1.5/llama_index/readers/microsoft_sharepoint/__init__.py
--rw-r--r--   0        0        0    13444 2024-03-31 17:05:15.790447 llama_index_readers_microsoft_sharepoint-0.1.5/llama_index/readers/microsoft_sharepoint/base.py
--rw-r--r--   0        0        0    41139 2024-03-31 17:05:15.790447 llama_index_readers_microsoft_sharepoint-0.1.5/llama_index/readers/microsoft_sharepoint/file_path_info.png
--rw-r--r--   0        0        0     1594 2024-03-31 17:05:15.790447 llama_index_readers_microsoft_sharepoint-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 llama_index_readers_microsoft_sharepoint-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1782 2024-04-01 21:33:17.112191 llama_index_readers_microsoft_sharepoint-0.1.6/README.md
+-rw-r--r--   0        0        0      107 2024-04-01 21:33:17.112191 llama_index_readers_microsoft_sharepoint-0.1.6/llama_index/readers/microsoft_sharepoint/__init__.py
+-rw-r--r--   0        0        0    15522 2024-04-01 21:33:17.112191 llama_index_readers_microsoft_sharepoint-0.1.6/llama_index/readers/microsoft_sharepoint/base.py
+-rw-r--r--   0        0        0    41139 2024-04-01 21:33:17.112191 llama_index_readers_microsoft_sharepoint-0.1.6/llama_index/readers/microsoft_sharepoint/file_path_info.png
+-rw-r--r--   0        0        0     1594 2024-04-01 21:33:17.112191 llama_index_readers_microsoft_sharepoint-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 llama_index_readers_microsoft_sharepoint-0.1.6/PKG-INFO
```

### Comparing `llama_index_readers_microsoft_sharepoint-0.1.5/README.md` & `llama_index_readers_microsoft_sharepoint-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_microsoft_sharepoint-0.1.5/llama_index/readers/microsoft_sharepoint/base.py` & `llama_index_readers_microsoft_sharepoint-0.1.6/llama_index/readers/microsoft_sharepoint/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """SharePoint files reader."""
 
 import logging
 import os
 import tempfile
 from typing import Any, Dict, List, Union, Optional
+from typing import Any, Dict, List, Optional
 
 import requests
 from llama_index.core.readers import SimpleDirectoryReader
 from llama_index.core.readers.base import BaseReader, BasePydanticReader
 from llama_index.core.schema import Document
 from llama_index.core.bridge.pydantic import PrivateAttr, Field
 
@@ -21,39 +22,54 @@
     Reads folders from the SharePoint site from a folder under documents.
 
     Args:
         client_id (str): The Application ID for the app registered in Microsoft Azure Portal.
             The application must also be configured with MS Graph permissions "Files.ReadAll", "Sites.ReadAll" and BrowserSiteLists.Read.All.
         client_secret (str): The application secret for the app registered in Azure.
         tenant_id (str): Unique identifier of the Azure Active Directory Instance.
+        sharepoint_site_name (Optional[str]): The name of the SharePoint site to download from.
+        sharepoint_folder_path (Optional[str]): The path of the SharePoint folder to download from.
+        sharepoint_folder_id (Optional[str]): The ID of the SharePoint folder to download from. Overrides sharepoint_folder_path.
         file_extractor (Optional[Dict[str, BaseReader]]): A mapping of file extension to a BaseReader class that specifies how to convert that
                                                           file to text. See `SimpleDirectoryReader` for more details.
     """
 
     client_id: str = None
     client_secret: str = None
     tenant_id: str = None
+    sharepoint_site_name: Optional[str] = None
+    sharepoint_folder_path: Optional[str] = None
+    sharepoint_folder_id: Optional[str] = None
     file_extractor: Optional[Dict[str, Union[str, BaseReader]]] = Field(
         default=None, exclude=True
     )
 
     _authorization_headers = PrivateAttr()
+    _site_id_with_host_name = PrivateAttr()
+    _drive_id_endpoint = PrivateAttr()
+    _drive_id = PrivateAttr()
 
     def __init__(
         self,
         client_id: str,
         client_secret: str,
         tenant_id: str,
+        sharepoint_site_name: Optional[str] = None,
+        sharepoint_folder_path: Optional[str] = None,
+        sharepoint_folder_id: Optional[str] = None,
         file_extractor: Optional[Dict[str, Union[str, BaseReader]]] = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(
             client_id=client_id,
             client_secret=client_secret,
             tenant_id=tenant_id,
+            sharepoint_site_name=sharepoint_site_name,
+            sharepoint_folder_path=sharepoint_folder_path,
+            sharepoint_folder_id=sharepoint_folder_id,
             file_extractor=file_extractor,
             **kwargs,
         )
 
     @classmethod
     def class_name(cls) -> str:
         return "SharePointReader"
@@ -290,15 +306,16 @@
         metadata[file_path] = self._extract_metadata_for_file(item)
         return metadata
 
     def _download_files_from_sharepoint(
         self,
         download_dir: str,
         sharepoint_site_name: str,
-        sharepoint_folder_path: str,
+        sharepoint_folder_path: Optional[str],
+        sharepoint_folder_id: Optional[str],
         recursive: bool,
     ) -> Dict[str, str]:
         """
         Downloads files from the specified folder and returns the metadata for the downloaded files.
 
         Args:
             download_dir (str): The directory where the files should be downloaded.
@@ -314,20 +331,21 @@
 
         self._site_id_with_host_name = self._get_site_id_with_host_name(
             access_token, sharepoint_site_name
         )
 
         self._drive_id = self._get_drive_id()
 
-        self.sharepoint_folder_id = self._get_sharepoint_folder_id(
-            sharepoint_folder_path
-        )
+        if sharepoint_folder_id is None:
+            sharepoint_folder_id = self._get_sharepoint_folder_id(
+                sharepoint_folder_path
+            )
 
         return self._download_files_and_extract_metadata(
-            self.sharepoint_folder_id, download_dir, recursive
+            sharepoint_folder_id, download_dir, recursive
         )
 
     def _load_documents_with_metadata(
         self,
         files_metadata: Dict[str, Any],
         download_dir: str,
         recursive: bool,
@@ -353,36 +371,60 @@
             file_metadata=get_metadata,
             recursive=recursive,
         )
         return simple_loader.load_data()
 
     def load_data(
         self,
-        sharepoint_site_name: str,
-        sharepoint_folder_path: str,
+        sharepoint_site_name: Optional[str] = None,
+        sharepoint_folder_path: Optional[str] = None,
+        sharepoint_folder_id: Optional[str] = None,
         recursive: bool = False,
     ) -> List[Document]:
         """
         Loads the files from the specified folder in the SharePoint site.
 
         Args:
-            sharepoint_site_name (str): The name of the SharePoint site.
-            sharepoint_folder_path (str): The path of the folder in the SharePoint site.
+            sharepoint_site_name (Optional[str]): The name of the SharePoint site.
+            sharepoint_folder_path (Optional[str]): The path of the folder in the SharePoint site.
             recursive (bool): If True, files from all subfolders are downloaded.
 
         Returns:
             List[Document]: A list containing the documents with metadata.
 
         Raises:
             Exception: If an error occurs while accessing SharePoint site.
         """
+        # If no arguments are provided to load_data, default to the object attributes
+        if sharepoint_site_name is None:
+            sharepoint_site_name = self.sharepoint_site_name
+
+        if sharepoint_folder_path is None:
+            sharepoint_folder_path = self.sharepoint_folder_path
+
+        if sharepoint_folder_id is None:
+            sharepoint_folder_id = self.sharepoint_folder_id
+
+        # TODO: make both of these values optional — and just default to the client ID defaults
+        if sharepoint_site_name is None:
+            raise ValueError("sharepoint_site_name must be provided.")
+
+        if sharepoint_folder_path is None and sharepoint_folder_id is None:
+            raise ValueError(
+                "sharepoint_folder_path or sharepoint_folder_id must be provided."
+            )
+
         try:
             with tempfile.TemporaryDirectory() as temp_dir:
                 files_metadata = self._download_files_from_sharepoint(
-                    temp_dir, sharepoint_site_name, sharepoint_folder_path, recursive
+                    temp_dir,
+                    sharepoint_site_name,
+                    sharepoint_folder_path,
+                    sharepoint_folder_id,
+                    recursive,
                 )
                 # return self.files_metadata
                 return self._load_documents_with_metadata(
                     files_metadata, temp_dir, recursive
                 )
 
         except Exception as exp:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `llama_index_readers_microsoft_sharepoint-0.1.5/llama_index/readers/microsoft_sharepoint/file_path_info.png` & `llama_index_readers_microsoft_sharepoint-0.1.6/llama_index/readers/microsoft_sharepoint/file_path_info.png`

 * *Files identical despite different names*

### Comparing `llama_index_readers_microsoft_sharepoint-0.1.5/pyproject.toml` & `llama_index_readers_microsoft_sharepoint-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = "llama-index readers microsoft_sharepoint integration"
 exclude = ["**/BUILD"]
 keywords = ["microsoft 365", "microsoft365", "sharepoint"]
 license = "MIT"
 maintainers = ["arun-soliton"]
 name = "llama-index-readers-microsoft-sharepoint"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_readers_microsoft_sharepoint-0.1.5/PKG-INFO` & `llama_index_readers_microsoft_sharepoint-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-microsoft-sharepoint
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index readers microsoft_sharepoint integration
 License: MIT
 Keywords: microsoft 365,microsoft365,sharepoint
 Author: Your Name
 Author-email: you@example.com
 Maintainer: arun-soliton
 Requires-Python: >=3.8.1,<4.0
```

