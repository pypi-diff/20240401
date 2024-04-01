# Comparing `tmp/firebatch-1.0.1.tar.gz` & `tmp/firebatch-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firebatch-1.0.1.tar", max compression
+gzip compressed data, was "firebatch-1.1.0.tar", max compression
```

## Comparing `firebatch-1.0.1.tar` & `firebatch-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1095 2024-04-01 09:15:03.736940 firebatch-1.0.1/LICENSE
--rw-r--r--   0        0        0     4000 2024-04-01 09:15:03.736940 firebatch-1.0.1/Readme.md
--rw-r--r--   0        0        0        0 2024-04-01 09:15:03.736940 firebatch-1.0.1/firebatch/__init__.py
--rw-r--r--   0        0        0       59 2024-04-01 09:15:03.736940 firebatch-1.0.1/firebatch/__main__.py
--rw-r--r--   0        0        0     9970 2024-04-01 09:15:03.736940 firebatch-1.0.1/firebatch/cli.py
--rw-r--r--   0        0        0     3720 2024-04-01 09:15:03.736940 firebatch-1.0.1/firebatch/endcoding.py
--rw-r--r--   0        0        0      867 2024-04-01 09:15:03.736940 firebatch-1.0.1/firebatch/firestore_client.py
--rw-r--r--   0        0        0     8957 2024-04-01 09:15:03.736940 firebatch-1.0.1/firebatch/operations.py
--rw-r--r--   0        0        0     3773 2024-04-01 09:15:03.736940 firebatch-1.0.1/firebatch/utils.py
--rw-r--r--   0        0        0      557 2024-04-01 09:15:03.736940 firebatch-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4409 1970-01-01 00:00:00.000000 firebatch-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-04-01 11:24:02.215901 firebatch-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4790 2024-04-01 11:24:02.215901 firebatch-1.1.0/Readme.md
+-rw-r--r--   0        0        0        0 2024-04-01 11:24:02.215901 firebatch-1.1.0/firebatch/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-01 11:24:02.215901 firebatch-1.1.0/firebatch/__main__.py
+-rw-r--r--   0        0        0    10239 2024-04-01 11:24:02.215901 firebatch-1.1.0/firebatch/cli.py
+-rw-r--r--   0        0        0     3720 2024-04-01 11:24:02.215901 firebatch-1.1.0/firebatch/endcoding.py
+-rw-r--r--   0        0        0      867 2024-04-01 11:24:02.219901 firebatch-1.1.0/firebatch/firestore_client.py
+-rw-r--r--   0        0        0     8974 2024-04-01 11:24:02.219901 firebatch-1.1.0/firebatch/operations.py
+-rw-r--r--   0        0        0     3905 2024-04-01 11:24:02.219901 firebatch-1.1.0/firebatch/utils.py
+-rw-r--r--   0        0        0      557 2024-04-01 11:24:02.219901 firebatch-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5184 1970-01-01 00:00:00.000000 firebatch-1.1.0/PKG-INFO
```

### Comparing `firebatch-1.0.1/LICENSE` & `firebatch-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `firebatch-1.0.1/firebatch/cli.py` & `firebatch-1.1.0/firebatch/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,24 +77,26 @@
 
 Usage:
 firebatch [OPTIONS] COMMAND [ARGS]...
 """
     pass
 
 @cli.command(cls=StdCommand)
+@click.option('--collection-group', '-cg', is_flag=True, default=False, help='Treat the collection name as a collection group name for a collection group query.')
 @click.option('--format', '-f', type=click.Choice(['json', 'jsonl']), default='jsonl', help='Output format for reading documents.')
 @click.option('--timestamp-convert', '-t', is_flag=True, help='convert firestore timestamps to simple datetime string in isoformat, otherwise the value will be wrapped with the key __timestamp__ for converting it back when writing.')
 @click.option('--geopoint-convert', '-g', is_flag=True, help='convert geopoints to simple map with longitude and latitude, otherwise the values will be wrapped with the key __geopoint__ for converting it back when writing.')
 @click.option('--raw', is_flag=True, default=False, help='disable the document ids in the output json and only output the data.')
 @click.option('--where', '-w', multiple=True, callback=validate_queries, help='Query conditions (can specify multiple), formatted as "field operator value".')
 @click.option('--order-by', help='Field to order the results by.')
 @click.option('--limit', type=int, help='Limit the number of results.')
-def read(collection, format, timestamp_convert, geopoint_convert, where, order_by, limit, verbose, raw, dry_run):
+def read(collection, collection_group, format, timestamp_convert, geopoint_convert, where, order_by, limit, verbose, raw, dry_run):
     """read documents from firestore and print them. By default it wraps every document with its id (needed by other commands). If the --raw flag is used then the documents are not wrapped."""
     read_documents = download_collection_documents(collection_path=collection, 
+                                                   collection_group=collection_group,
                                                    output_format=format,
                                                    timestamp_convert=timestamp_convert,
                                                    geopoint_convert=geopoint_convert,
                                                    conditions=where,
                                                    order_by=order_by,
                                                    limit=limit, 
                                                    raw=raw,
```

### Comparing `firebatch-1.0.1/firebatch/endcoding.py` & `firebatch-1.1.0/firebatch/endcoding.py`

 * *Files identical despite different names*

### Comparing `firebatch-1.0.1/firebatch/firestore_client.py` & `firebatch-1.1.0/firebatch/firestore_client.py`

 * *Files identical despite different names*

### Comparing `firebatch-1.0.1/firebatch/operations.py` & `firebatch-1.1.0/firebatch/operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import json
 import sys
 from typing import Any, Dict, List, Optional, TextIO, Tuple
 from tqdm import tqdm
 
 from firebatch.endcoding import convert_to_firestore_types, to_json
-from firebatch.utils import get_nested_collection_reference, read_documents
+from firebatch.utils import get_query_reference, read_documents
 from firebatch.firestore_client import initialize_firestore_client
 from google.api_core.exceptions import NotFound
 from google.cloud.firestore import SERVER_TIMESTAMP
 import logging
 logger = logging.getLogger(__name__)
 
 def print_verbose(message: str, verbose: bool):
     """Prints message if verbose mode is enabled."""
     if verbose:
         logger.info(message)
 
 def download_collection_documents(collection_path: str, 
+                                  collection_group: bool,
                                   output_format: str = 'jsonl', 
                                   timestamp_convert: bool = False, 
                                   geopoint_convert: bool = False,
                                   raw : bool = False, 
                                   conditions: List[Tuple[str, str, Any]] = [], 
                                   order_by: Optional[str] = None, 
                                   limit: Optional[int] = None, 
                                   verbose: bool = False):
 
     db = initialize_firestore_client()
-    query_ref = get_nested_collection_reference(db, collection_path)
+    query_ref = get_query_reference(db, collection_path, collection_group)
     
     for field, operator, value in conditions:
         logger.debug(f"apply conditions: {conditions}")
         if value.lower() == "null" or value.lower() == "none":
             value = None
         query_ref = query_ref.where(field, operator, value)
 
@@ -57,15 +58,15 @@
                     timestamp_field: str = None, 
                     timestamp_convert: bool = False, 
                     geopoint_convert: bool = False,
                     format: str="auto",
                     verbose: bool = False, 
                     dry_run: bool = False):
     db = initialize_firestore_client()
-    collection_ref = get_nested_collection_reference(db, collection_path)
+    collection_ref = get_query_reference(db, collection_path)
     batch = db.batch()
 
     documents = read_documents(file)
     total_documents = len(documents)
 
     with tqdm(total=total_documents, desc=f"Uploading documents to {collection_path}", disable=not verbose) as pbar:
         for data in documents:
@@ -108,15 +109,15 @@
             deleted += 1
 
         if deleted == 0:
             break  # All documents have been deleted
 
 def delete_documents_in_firestore(collection_path: str, doc_ids: List[str], verbose: bool = False, dry_run: bool = False):
     db = initialize_firestore_client()
-    collection_ref = get_nested_collection_reference(db, collection_path)
+    collection_ref = get_query_reference(db, collection_path)
 
     with tqdm(total=len(doc_ids), disable=not verbose, desc="Deleting documents") as pbar:
         for doc_id in doc_ids:
             doc_ref = collection_ref.document(doc_id)
 
             # First, delete subcollections recursively
             if not dry_run:
@@ -146,15 +147,15 @@
                                   timestamp_convert: bool = False, 
                                   geopoint_convert: bool = False,
                                   upsert: bool = False,
                                   verbose: bool = False, 
                                   dry_run: bool = False):
     db = initialize_firestore_client()
     batch = db.batch()
-    collection_ref = get_nested_collection_reference(db, collection_path)
+    collection_ref = get_query_reference(db, collection_path)
 
     # First, check for duplicate keys in the updates
     seen_doc_ids = set()
     duplicates = set()
     for update in updates:
         doc_id = update.get("__doc_id__")
         if doc_id:
```

### Comparing `firebatch-1.0.1/firebatch/utils.py` & `firebatch-1.1.0/firebatch/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,24 +35,27 @@
             except json.JSONDecodeError:
                 raise Exception("Unknown file format, could not detect either JSON or JSONL.")
     elif format == "json":
         return read_json(file)
     elif format == "jsonl":
         return read_jsonl(file)
     
-def get_nested_collection_reference(db: Client, collection_path: str):
-    # Splits the collection path and returns the final reference
-    ref = db
-    parts = collection_path.split('/')
-    for i, part in enumerate(parts):
-        if i % 2 == 0:
-            ref = ref.collection(part)
-        else:
-            ref = ref.document(part)
-    return ref
+def get_query_reference(db: Client, collection_path: str, collection_group=False):
+    if collection_group:
+        return db.collection_group(collection_path)
+    else:
+        # Existing logic for navigating collection/document paths
+        ref = db
+        parts = collection_path.split('/')
+        for i, part in enumerate(parts):
+            if i % 2 == 0:
+                ref = ref.collection(part)
+            else:
+                ref = ref.document(part)
+        return ref
 
 def parse_query_condition(condition: str) -> Tuple[str, str, Any]:
     """Parses a query condition, allowing spaces around operators and handling quoted strings as values."""
     logger.debug(f"Evaluating condition: {condition}")
     # List of Firestore operators for pattern matching
     operators = [">=", "<=", "==", "!=", ">", "<", "array-contains", "in", "array-contains-any"]
```

### Comparing `firebatch-1.0.1/pyproject.toml` & `firebatch-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firebatch"
-version = "1.0.1"
+version = "1.1.0"
 description = "A CLI and library for Firestore batch operations"
 authors = ["Alexander Balasch"]
 license = "MIT"
 readme = "Readme.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

