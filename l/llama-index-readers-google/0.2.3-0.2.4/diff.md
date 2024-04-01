# Comparing `tmp/llama_index_readers_google-0.2.3.tar.gz` & `tmp/llama_index_readers_google-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_google-0.2.3.tar", max compression
+gzip compressed data, was "llama_index_readers_google-0.2.4.tar", max compression
```

## Comparing `llama_index_readers_google-0.2.3.tar` & `llama_index_readers_google-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1366 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/README.md
--rw-r--r--   0        0        0      567 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/__init__.py
--rw-r--r--   0        0        0     1246 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/calendar/README.md
--rw-r--r--   0        0        0        0 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/calendar/__init__.py
--rw-r--r--   0        0        0     4756 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/calendar/base.py
--rw-r--r--   0        0        0     1442 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/docs/README.md
--rw-r--r--   0        0        0        0 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/docs/__init__.py
--rw-r--r--   0        0        0     8589 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/docs/base.py
--rw-r--r--   0        0        0     1983 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/drive/README.md
--rw-r--r--   0        0        0        0 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/drive/__init__.py
--rw-r--r--   0        0        0    20139 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/drive/base.py
--rw-r--r--   0        0        0      863 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/gmail/README.md
--rw-r--r--   0        0        0        0 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/gmail/__init__.py
--rw-r--r--   0        0        0     6475 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/gmail/base.py
--rw-r--r--   0        0        0     2256 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/keep/README.md
--rw-r--r--   0        0        0        0 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/keep/__init__.py
--rw-r--r--   0        0        0     2265 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/keep/base.py
--rw-r--r--   0        0        0     1053 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/sheets/README.md
--rw-r--r--   0        0        0        0 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/sheets/__init__.py
--rw-r--r--   0        0        0     7127 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/llama_index/readers/google/sheets/base.py
--rw-r--r--   0        0        0     1989 2024-03-31 17:05:15.774447 llama_index_readers_google-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2194 1970-01-01 00:00:00.000000 llama_index_readers_google-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1366 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/README.md
+-rw-r--r--   0        0        0      567 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/__init__.py
+-rw-r--r--   0        0        0     1246 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/calendar/README.md
+-rw-r--r--   0        0        0        0 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/calendar/__init__.py
+-rw-r--r--   0        0        0     4756 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/calendar/base.py
+-rw-r--r--   0        0        0     1442 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/docs/README.md
+-rw-r--r--   0        0        0        0 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/docs/__init__.py
+-rw-r--r--   0        0        0     8589 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/docs/base.py
+-rw-r--r--   0        0        0     1983 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/drive/README.md
+-rw-r--r--   0        0        0        0 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/drive/__init__.py
+-rw-r--r--   0        0        0    21424 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/drive/base.py
+-rw-r--r--   0        0        0      863 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/gmail/README.md
+-rw-r--r--   0        0        0        0 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/gmail/__init__.py
+-rw-r--r--   0        0        0     6475 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/gmail/base.py
+-rw-r--r--   0        0        0     2256 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/keep/README.md
+-rw-r--r--   0        0        0        0 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/keep/__init__.py
+-rw-r--r--   0        0        0     2265 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/keep/base.py
+-rw-r--r--   0        0        0     1053 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/sheets/README.md
+-rw-r--r--   0        0        0        0 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/sheets/__init__.py
+-rw-r--r--   0        0        0     7127 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/sheets/base.py
+-rw-r--r--   0        0        0     1989 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2194 1970-01-01 00:00:00.000000 llama_index_readers_google-0.2.4/PKG-INFO
```

### Comparing `llama_index_readers_google-0.2.3/README.md` & `llama_index_readers_google-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.3/llama_index/readers/google/__init__.py` & `llama_index_readers_google-0.2.4/llama_index/readers/google/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.3/llama_index/readers/google/calendar/README.md` & `llama_index_readers_google-0.2.4/llama_index/readers/google/calendar/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.3/llama_index/readers/google/calendar/base.py` & `llama_index_readers_google-0.2.4/llama_index/readers/google/calendar/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.3/llama_index/readers/google/docs/README.md` & `llama_index_readers_google-0.2.4/llama_index/readers/google/docs/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.3/llama_index/readers/google/docs/base.py` & `llama_index_readers_google-0.2.4/llama_index/readers/google/docs/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.3/llama_index/readers/google/drive/README.md` & `llama_index_readers_google-0.2.4/llama_index/readers/google/drive/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.3/llama_index/readers/google/drive/base.py` & `llama_index_readers_google-0.2.4/llama_index/readers/google/drive/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 class GoogleDriveReader(BasePydanticReader):
     """Google Drive Reader.
 
     Reads files from Google Drive. Credentials passed directly to the constructor
     will take precedence over those passed as file paths.
 
     Args:
+        drive_id (Optional[str]): Drive id of the shared drive in google drive.
+        folder_id (Optional[str]): Folder id of the folder in google drive.
+        file_ids (Optional[str]): File ids of the files in google drive.
+        query_string: A more generic query string to filter the documents, e.g. "name contains 'test'".
+            It gives more flexibility to filter the documents. More info: https://developers.google.com/drive/api/v3/search-files
         is_cloud (Optional[bool]): Whether the reader is being used in
             a cloud environment. Will not save credentials to disk if so.
             Defaults to False.
         credentials_path (Optional[str]): Path to client config file.
             Defaults to None.
         token_path (Optional[str]): Path to authorized user info file. Defaults
             to None.
@@ -45,28 +50,36 @@
         service_account_key (Optional[dict]): Dictionary containing service
             account key. Defaults to None.
         file_extractor (Optional[Dict[str, BaseReader]]): A mapping of file
             extension to a BaseReader class that specifies how to convert that
             file to text. See `SimpleDirectoryReader` for more details.
     """
 
+    drive_id: Optional[str] = None
+    folder_id: Optional[str] = None
+    file_ids: Optional[List[str]] = None
+    query_string: Optional[str] = None
     client_config: Optional[dict] = None
     authorized_user_info: Optional[dict] = None
     service_account_key: Optional[dict] = None
     token_path: Optional[str] = None
     file_extractor: Optional[Dict[str, Union[str, BaseReader]]] = Field(
         default=None, exclude=True
     )
 
     _is_cloud: bool = PrivateAttr(default=False)
     _creds: Credentials = PrivateAttr()
     _mimetypes: dict = PrivateAttr()
 
     def __init__(
         self,
+        drive_id: Optional[str] = None,
+        folder_id: Optional[str] = None,
+        file_ids: Optional[List[str]] = None,
+        query_string: Optional[str] = None,
         is_cloud: Optional[bool] = False,
         credentials_path: str = "credentials.json",
         token_path: str = "token.json",
         service_account_key_path: str = "service_account_key.json",
         client_config: Optional[dict] = None,
         authorized_user_info: Optional[dict] = None,
         service_account_key: Optional[dict] = None,
@@ -108,14 +121,18 @@
             with open(service_account_key_path, encoding="utf-8") as json_file:
                 service_account_key = json.load(json_file)
 
         if client_config is None and service_account_key is None:
             raise ValueError("Must specify `client_config` or `service_account_key`.")
 
         super().__init__(
+            drive_id=drive_id,
+            folder_id=folder_id,
+            file_ids=file_ids,
+            query_string=query_string,
             client_config=client_config,
             authorized_user_info=authorized_user_info,
             service_account_key=service_account_key,
             token_path=token_path,
             file_extractor=file_extractor,
             **kwargs,
         )
@@ -489,14 +506,24 @@
                 It gives more flexibility to filter the documents. More info: https://developers.google.com/drive/api/v3/search-files
 
         Returns:
             List[Document]: A list of documents.
         """
         self._creds = self._get_credentials()
 
+        # If no arguments are provided to load_data, default to the object attributes
+        if drive_id is None:
+            drive_id = self.drive_id
+        if folder_id is None:
+            folder_id = self.folder_id
+        if file_ids is None:
+            file_ids = self.file_ids
+        if query_string is None:
+            query_string = self.query_string
+
         if folder_id:
             return self._load_from_folder(drive_id, folder_id, mime_types, query_string)
         elif file_ids:
             return self._load_from_file_ids(
                 drive_id, file_ids, mime_types, query_string
             )
         else:
```

### Comparing `llama_index_readers_google-0.2.3/llama_index/readers/google/gmail/README.md` & `llama_index_readers_google-0.2.4/llama_index/readers/google/gmail/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.3/llama_index/readers/google/gmail/base.py` & `llama_index_readers_google-0.2.4/llama_index/readers/google/gmail/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.3/llama_index/readers/google/keep/README.md` & `llama_index_readers_google-0.2.4/llama_index/readers/google/keep/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.3/llama_index/readers/google/keep/base.py` & `llama_index_readers_google-0.2.4/llama_index/readers/google/keep/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.3/llama_index/readers/google/sheets/README.md` & `llama_index_readers_google-0.2.4/llama_index/readers/google/sheets/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.3/llama_index/readers/google/sheets/base.py` & `llama_index_readers_google-0.2.4/llama_index/readers/google/sheets/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.3/pyproject.toml` & `llama_index_readers_google-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     "ong",
     "piroz",
     "pycui",
     "ravi03071991",
 ]
 name = "llama-index-readers-google"
 readme = "README.md"
-version = "0.2.3"
+version = "0.2.4"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 llama-index-core = "^0.10.11.post1"
 google-api-python-client = "^2.115.0"
 google-auth-httplib2 = "^0.2.0"
 google-auth-oauthlib = "^1.2.0"
```

### Comparing `llama_index_readers_google-0.2.3/PKG-INFO` & `llama_index_readers_google-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-google
-Version: 0.2.3
+Version: 0.2.4
 Summary: llama-index readers google integration
 License: MIT
 Keywords: email,gmail,google keep,google notes
 Author: Your Name
 Author-email: you@example.com
 Maintainer: bbornsztein
 Requires-Python: >=3.10,<4.0
```

