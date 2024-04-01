# Comparing `tmp/llama_index_readers_gcs-0.1.5.tar.gz` & `tmp/llama_index_readers_gcs-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_gcs-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_readers_gcs-0.1.6.tar", max compression
```

## Comparing `llama_index_readers_gcs-0.1.5.tar` & `llama_index_readers_gcs-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1535 2024-03-28 00:19:29.496813 llama_index_readers_gcs-0.1.5/README.md
--rw-r--r--   0        0        0       76 2024-03-28 00:19:29.496813 llama_index_readers_gcs-0.1.5/llama_index/readers/gcs/__init__.py
--rw-r--r--   0        0        0     3849 2024-03-28 00:19:29.496813 llama_index_readers_gcs-0.1.5/llama_index/readers/gcs/base.py
--rw-r--r--   0        0        0     1562 2024-03-28 00:19:29.496813 llama_index_readers_gcs-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 llama_index_readers_gcs-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1535 2024-04-01 21:33:17.092190 llama_index_readers_gcs-0.1.6/README.md
+-rw-r--r--   0        0        0       76 2024-04-01 21:33:17.092190 llama_index_readers_gcs-0.1.6/llama_index/readers/gcs/__init__.py
+-rw-r--r--   0        0        0     4222 2024-04-01 21:33:17.092190 llama_index_readers_gcs-0.1.6/llama_index/readers/gcs/base.py
+-rw-r--r--   0        0        0     1562 2024-04-01 21:33:17.092190 llama_index_readers_gcs-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 llama_index_readers_gcs-0.1.6/PKG-INFO
```

### Comparing `llama_index_readers_gcs-0.1.5/README.md` & `llama_index_readers_gcs-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_gcs-0.1.5/llama_index/readers/gcs/base.py` & `llama_index_readers_gcs-0.1.6/llama_index/readers/gcs/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 GCS file and directory reader.
 
 A loader that fetches a file or iterates through a directory on Google Cloud Storage (GCS).
 
 """
-
+import json
 from typing import Callable, Dict, List, Optional, Union
 
 from google.oauth2 import service_account
 from llama_index.core.readers import SimpleDirectoryReader
 from llama_index.core.readers.base import BaseReader, BasePydanticReader
 from llama_index.core.schema import Document
 from llama_index.core.bridge.pydantic import Field
@@ -37,15 +37,16 @@
     required_exts (Optional[List[str]]): List of required extensions.
         Default is None.
     num_files_limit (Optional[int]): Maximum number of files to read.
         Default is None.
     file_metadata (Optional[Callable[str, Dict]]): A function that takes
         in a filename and returns a Dict of metadata for the Document.
         Default is None.
-    service_account_key_json (Optional[str]): provide GCP service account key JSON directly.
+    service_account_key (Optional[Dict[str, str]]): provide GCP service account key directly.
+    service_account_key_json (Optional[str]): provide GCP service account key as a JSON string.
     """
 
     is_remote: bool = True
 
     bucket: str
     key: Optional[str] = None
     prefix: Optional[str] = ""
@@ -53,27 +54,32 @@
     file_extractor: Optional[Dict[str, Union[str, BaseReader]]] = Field(
         default=None, exclude=True
     )
     required_exts: Optional[List[str]] = None
     filename_as_id: bool = True
     num_files_limit: Optional[int] = None
     file_metadata: Optional[Callable[[str], Dict]] = Field(default=None, exclude=True)
+    service_account_key: Optional[Dict[str, str]] = None
     service_account_key_json: Optional[str] = None
 
     @classmethod
     def class_name(cls) -> str:
         return "GCSReader"
 
     def load_gcs_files_as_docs(self) -> List[Document]:
         """Load file(s) from GCS."""
         from gcsfs import GCSFileSystem
 
-        if self.service_account_key_json is not None:
+        if self.service_account_key is not None:
             creds = service_account.Credentials.from_service_account_info(
-                self.service_account_key_json, scopes=SCOPES
+                self.service_account_key, scopes=SCOPES
+            )
+        elif self.service_account_key_json is not None:
+            creds = service_account.Credentials.from_service_account_file(
+                json.loads(self.service_account_key_json), scopes=SCOPES
             )
         else:
             # Use anonymous access if none are specified
             creds = "anon"
 
         gcsfs = GCSFileSystem(
             token=creds,
```

### Comparing `llama_index_readers_gcs-0.1.5/pyproject.toml` & `llama_index_readers_gcs-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = "llama-index readers gcs integration"
 exclude = ["**/BUILD"]
 keywords = ["bucket", "gcp", "gcs", "google cloud storage"]
 license = "MIT"
 maintainers = ["nfiacco"]
 name = "llama-index-readers-gcs"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 llama-index-readers-file = "^0.1.11"
 gcsfs = "^2024.3.1"
```

### Comparing `llama_index_readers_gcs-0.1.5/PKG-INFO` & `llama_index_readers_gcs-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-gcs
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index readers gcs integration
 License: MIT
 Keywords: bucket,gcp,gcs,google cloud storage
 Author: Your Name
 Author-email: you@example.com
 Maintainer: nfiacco
 Requires-Python: >=3.8.1,<4.0
```

