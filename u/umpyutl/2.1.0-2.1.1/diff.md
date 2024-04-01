# Comparing `tmp/umpyutl-2.1.0.tar.gz` & `tmp/umpyutl-2.1.1.tar.gz`

## Comparing `umpyutl-2.1.0.tar` & `umpyutl-2.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 umpyutl-2.1.0/src/umpyutl/__about__.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 umpyutl-2.1.0/src/umpyutl/__init__.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 umpyutl-2.1.0/src/umpyutl/convert.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 umpyutl-2.1.0/src/umpyutl/http.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umpyutl-2.1.0/src/umpyutl/py.typed
--rw-r--r--   0        0        0     8387 2020-02-02 00:00:00.000000 umpyutl-2.1.0/src/umpyutl/read.py
--rw-r--r--   0        0        0    10838 2020-02-02 00:00:00.000000 umpyutl-2.1.0/src/umpyutl/write.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 umpyutl-2.1.0/.gitignore
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 umpyutl-2.1.0/LICENSE
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 umpyutl-2.1.0/README.md
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 umpyutl-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 umpyutl-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 umpyutl-2.1.1/src/umpyutl/__about__.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 umpyutl-2.1.1/src/umpyutl/__init__.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 umpyutl-2.1.1/src/umpyutl/convert.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 umpyutl-2.1.1/src/umpyutl/http.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umpyutl-2.1.1/src/umpyutl/py.typed
+-rw-r--r--   0        0        0     8714 2020-02-02 00:00:00.000000 umpyutl-2.1.1/src/umpyutl/read.py
+-rw-r--r--   0        0        0    11177 2020-02-02 00:00:00.000000 umpyutl-2.1.1/src/umpyutl/write.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 umpyutl-2.1.1/.gitignore
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 umpyutl-2.1.1/LICENSE
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 umpyutl-2.1.1/README.md
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 umpyutl-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 umpyutl-2.1.1/PKG-INFO
```

### Comparing `umpyutl-2.1.0/src/umpyutl/convert.py` & `umpyutl-2.1.1/src/umpyutl/convert.py`

 * *Files identical despite different names*

### Comparing `umpyutl-2.1.0/src/umpyutl/http.py` & `umpyutl-2.1.1/src/umpyutl/http.py`

 * *Files identical despite different names*

### Comparing `umpyutl-2.1.0/src/umpyutl/read.py` & `umpyutl-2.1.1/src/umpyutl/read.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import csv
 import json
+import pathlib
 import yaml
 from typing import List, OrderedDict
 from warnings import warn
 
 
 def from_csv(
-    filepath: str,
+    filepath: pathlib.Path | str,
     encoding: str = "utf-8",
     newline: str = "",
     delimiter: str = ",",
 ) -> List[list]:
     """
     Reads a CSV file, parsing row values per the provided delimiter. Returns a list of lists,
     wherein each nested list represents a single row from the input file.
@@ -18,41 +19,41 @@
     WARN: If a byte order mark (BOM) is encountered at the beginning of the first line of decoded
     text, call < from_csv > and pass 'utf-8-sig' as the < encoding > argument.
 
     WARN: If newline='' is not specified, newlines '\n' or '\r\n' embedded inside quoted fields
     may not be interpreted correctly by the csv.reader.
 
     Parameters:
-        filepath (str): absolute or relative path to source file
+        filepath (pathlib.Path | str): absolute or relative path to source file
         encoding (str): name of encoding used to decode the file
         newline (str): specifies replacement value for newline '\n'
                        or '\r\n' (Windows) character sequences
         delimiter (str): delimiter that separates the row values
 
     Returns:
         list: a list of nested "row" lists
     """
 
     with open(filepath, "r", encoding=encoding, newline=newline) as file_obj:
         return [row for row in csv.reader(file_obj, delimiter=delimiter)]
 
 
 def from_csv_to_dicts(
-    filepath: str,
+    filepath: pathlib.Path | str,
     encoding: str = "utf-8",
     newline: str = "",
     delimiter: str = ",",
     ordered: bool = True,
 ) -> List[OrderedDict] | List[dict]:
     """Accepts a file path, creates a file object, and returns a list of dictionaries
     that represent the row values using the cvs.DictReader(). Default type returned
     in list is an OrderedDict which can be overridden.
 
     Parameters:
-        filepath (str): absolute or relative path to source file
+        filepath (pathlib.Path | str): absolute or relative path to source file
         encoding (str): name of encoding used to decode the file
         newline (str): specifies replacement value for newline '\n'
                        or '\r\n' (Windows) character sequences
         delimiter (str): delimiter that separates the row values
         ordered (bool): return either list of OrderedDict objects or dict objects
 
     Returns:
@@ -62,66 +63,68 @@
     with open(filepath, "r", newline=newline, encoding=encoding) as file_obj:
         if ordered:
             return [row for row in csv.DictReader(file_obj, delimiter=delimiter)]
         else:
             return [dict(row) for row in csv.DictReader(file_obj, delimiter=delimiter)]
 
 
-def from_json(filepath: str, encoding: str = "utf-8") -> dict | list:
+def from_json(filepath: pathlib.Path | str, encoding: str = "utf-8") -> dict | list:
     """Reads a JSON document, decodes the file content, and returns a list or dictionary if
     provided with a valid filepath.
 
     Parameters:
-        filepath (str): absolute or relative path to source file
+        filepath (pathlib.Path | str): absolute or relative path to source file
         encoding (str): name of encoding used to decode the file
 
     Returns:
         dict | list: dict or list representations of the decoded JSON document
     """
 
     with open(filepath, "r", encoding=encoding) as file_obj:
         return json.load(file_obj)
 
 
-def from_txt(filepath: str, encoding: str = "utf-8", strip: bool = True) -> List[str]:
+def from_txt(
+    filepath: pathlib.Path | str, encoding: str = "utf-8", strip: bool = True
+) -> List[str]:
     """Read text file line by line. Remove whitespace and trailing newline
     escape character.
 
     Parameters:
-        filepath (str): absolute or relative path to source file
+        filepath (pathlib.Path | str): absolute or relative path to source file
         encoding (str): name of encoding used to decode the file.
         strip (bool): remove white space, newline escape characters
 
     Returns
         list: list of lines in file
     """
 
     with open(filepath, "r", encoding=encoding) as file_obj:
         if strip:
             return [line.strip() for line in file_obj]
         else:
             return file_obj.readlines()
 
 
-def from_yaml(filepath: str) -> dict | list:
+def from_yaml(filepath: pathlib.Path | str) -> dict | list:
     """Read a YAML (Yet Another Markup Language) file given a valid filepath.
 
     Parameters:
-        filepath (str): absolute or relative path to source file
+        filepath (pathlib.Path | str): absolute or relative path to source file
 
     Returns:
         dict | list: typically a list or dictionary representation of the file object
     """
 
     with open(filepath, "r") as file_object:
         return yaml.load(file_object, Loader=yaml.FullLoader)
 
 
 def read_csv(
-    filepath: str,
+    filepath: pathlib.Path | str,
     encoding: str = "utf-8",
     newline: str = "",
     delimiter: str = ",",
 ) -> List[list]:
     """
     Reads a CSV file, parsing row values per the provided delimiter. Returns a list of lists,
     wherein each nested list represents a single row from the input file.
@@ -129,15 +132,15 @@
     WARN: If a byte order mark (BOM) is encountered at the beginning of the first line of decoded
     text, call < from_csv > and pass 'utf-8-sig' as the < encoding > argument.
 
     WARN: If newline='' is not specified, newlines '\n' or '\r\n' embedded inside quoted fields
     may not be interpreted correctly by the csv.reader.
 
     Parameters:
-        filepath (str): absolute or relative path to source file
+        filepath (pathlib.Path | str): absolute or relative path to source file
         encoding (str): name of encoding used to decode the file
         newline (str): specifies replacement value for newline '\n'
                        or '\r\n' (Windows) character sequences
         delimiter (str): delimiter that separates the row values
 
     Returns:
         list: a list of nested "row" lists
@@ -149,26 +152,26 @@
         stacklevel=2,
     )
 
     return from_csv(filepath, encoding, newline, delimiter)
 
 
 def read_csv_to_dicts(
-    filepath: str,
+    filepath: pathlib.Path | str,
     encoding: str = "utf-8",
     newline: str = "",
     delimiter: str = ",",
     ordered: bool = True,
 ) -> List[OrderedDict] | List[dict]:
     """Accepts a file path, creates a file object, and returns a list of dictionaries
     that represent the row values using the cvs.DictReader(). Default type returned
     in list is an OrderedDict which can be overridden.
 
     Parameters:
-        filepath (str): absolute or relative path to source file
+        filepath (pathlib.Path | str): absolute or relative path to source file
         encoding (str): name of encoding used to decode the file
         newline (str): specifies replacement value for newline '\n'
                        or '\r\n' (Windows) character sequences
         delimiter (str): delimiter that separates the row values
         ordered (bool): return either list of OrderedDict objects or dict objects
 
     Returns:
@@ -180,20 +183,22 @@
         DeprecationWarning,
         stacklevel=2,
     )
 
     return from_csv_to_dicts(filepath, encoding, newline, delimiter, ordered)
 
 
-def read_file(filepath: str, encoding: str = "utf-8", strip: bool = True) -> List[str]:
+def read_file(
+    filepath: pathlib.Path | str, encoding: str = "utf-8", strip: bool = True
+) -> List[str]:
     """Read text file line by line. Remove whitespace and trailing newline
     escape character.
 
     Parameters:
-        filepath (str): absolute or relative path to source file
+        filepath (pathlib.Path | str): absolute or relative path to source file
         encoding (str): name of encoding used to decode the file.
         strip (bool): remove white space, newline escape characters
 
     Returns
         list: list of lines in file
     """
 
@@ -202,20 +207,20 @@
         DeprecationWarning,
         stacklevel=2,
     )
 
     return from_txt(filepath, encoding, strip)
 
 
-def read_json(filepath: str, encoding: str = "utf-8") -> dict | list:
+def read_json(filepath: pathlib.Path | str, encoding: str = "utf-8") -> dict | list:
     """Reads a JSON document, decodes the file content, and returns a list or dictionary if
     provided with a valid filepath.
 
     Parameters:
-        filepath (str): absolute or relative path to source file
+        filepath (pathlib.Path | str): absolute or relative path to source file
         encoding (str): name of encoding used to decode the file
 
     Returns:
         dict | list: dict or list representations of the decoded JSON document
     """
 
     warn(
@@ -223,19 +228,19 @@
         DeprecationWarning,
         stacklevel=2,
     )
 
     return from_json(filepath, encoding)
 
 
-def read_yaml(filepath: str) -> dict | list:
+def read_yaml(filepath: pathlib.Path | str) -> dict | list:
     """Read a YAML (Yet Another Markup Language) file given a valid filepath.
 
     Parameters:
-        filepath (str): absolute or relative path to source file
+        filepath (pathlib.Path | str): absolute or relative path to source file
 
     Returns:
         dict | list: typically a list or dictionary representation of the file object
     """
 
     warn(
         "read_yaml() is deprecated and will be removed from umpyutl 3.0.0. Use from_yaml().",
```

### Comparing `umpyutl-2.1.0/src/umpyutl/write.py` & `umpyutl-2.1.1/src/umpyutl/write.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import csv
 import json
+import pathlib
 import requests
 from typing import List, Optional, Tuple
 from warnings import warn
 
 
 def dicts_to_csv(
-    filepath: str,
+    filepath: pathlib.Path | str,
     data: List[dict],
     fieldnames: list | tuple,
     encoding: str = "utf-8",
     newline: str = "",
 ) -> None:
     """
     Writes dictionary data to a target CSV file as row data using the csv.DictWriter().
@@ -18,15 +19,15 @@
     in which each dictionary's key-value pairs are written to the row.
 
     WARN: This function is not designed to handle dictionaries that include key-value
     pairs in which the values are sequences or dictionaries. In such cases, serialize the
     object as JSON and write to a file using < write.to_json >.
 
     Parameters:
-        filepath (str): path to target file (if file does not exist it will be created)
+        filepath (pathlib.Path | str): path to target file (if file does not exist it will be created)
         data (list): dictionary content to be written to the target file
         fieldnames (seq): sequence specifing order in which key-value pairs are written to each row
         encoding (str): name of encoding used to encode the file
         newline (str): specifies replacement value for newline '\n'
                        or '\r\n' (Windows) character sequences
 
     Returns:
@@ -36,30 +37,30 @@
     with open(filepath, "w", encoding=encoding, newline=newline) as file_obj:
         writer = csv.DictWriter(file_obj, fieldnames=fieldnames)
         writer.writeheader()
         writer.writerows(data)
 
 
 def to_csv(
-    filepath: str,
+    filepath: pathlib.Path | str,
     data: list | tuple,
     headers: Optional[list | tuple] = None,
     encoding: str = "utf-8",
     newline: str = "",
 ) -> None:
     """
     Writes data to a target CSV file. Column headers are written as the first
     row of the CSV file if optional headers are specified.
 
-    WARN: If newline='' is not specified, newlines '\n' or '\r\n' embedded inside quoted
+    WARN: If newline='' is not specified, newlines '\n' or '\r\n' embedded inside quoted
     fields may not be interpreted correctly by the csv.reader. On platforms that utilize
     `\r\n` an extra `\r` will be added.
 
     Parameters:
-        filepath (str): path to target file (if file does not exist it will be created)
+        filepath (pathlib.Path | str): path to target file (if file does not exist it will be created)
         data (list | tuple): sequence to be written to the target file
         headers (seq): optional header row list or tuple
         encoding (str): name of encoding used to encode the file
         newline (str): specifies replacement value for newline '\n'
                        or '\r\n' (Windows) character sequences
 
     Returns:
@@ -73,47 +74,50 @@
             for row in data:
                 writer.writerow(row)
         else:
             writer.writerows(data)
 
 
 def to_file_response_chunked(
-    filepath: str, response: requests.Response, mode: str = "w", chunk_size: int = 1024
+    filepath: pathlib.Path | str,
+    response: requests.Response,
+    mode: str = "w",
+    chunk_size: int = 1024,
 ) -> None:
     """Writes < requests.Response > to a target file as a stream of data chunks.
     Override the optional write mode value if binary content <class 'bytes'> is to
     be written to file (i.e., mode='wb') or an append operation is intended on an
     existing file (i.e., mode='a' or 'ab').
 
     Parameters:
-        filepath (str): absolute or relative path to target file
+        filepath (pathlib.Path | str): absolute or relative path to target file
         response (requests.Response): data to be written to the target file
         mode (str): write operation mode
         chunk_size (int); size of data chunks to stream
 
     Returns:
         None
     """
 
     with open(filepath, mode) as file_object:
         for chunk in response.iter_content(chunk_size=chunk_size):
             file_object.write(chunk)
 
 
 def to_json(
-    filepath: str,
+    filepath: pathlib.Path | str,
     data: dict | list,
     encoding: str = "utf-8",
     ensure_ascii: bool = False,
     indent: int = 2,
 ) -> None:
     """Serializes object as JSON. Writes content to the provided filepath.
 
     Parameters:
-        filepath (str): the path to the file
+        filepath (pathlib.Path | str): the path to the file
         data (dict | list): the data to be encoded as JSON and written to the file
         encoding (str): name of encoding used to encode the file
         ensure_ascii (str): if False non-ASCII characters are printed as is; otherwise
                             non-ASCII characters are escaped.
         indent (int): number of "pretty printed" indention spaces applied to encoded JSON
 
     Returns:
@@ -121,24 +125,24 @@
     """
 
     with open(filepath, "w", encoding=encoding) as file_obj:
         json.dump(data, file_obj, ensure_ascii=ensure_ascii, indent=indent)
 
 
 def to_txt(
-    filepath: str,
+    filepath: pathlib.Path | str,
     data: List[str] | Tuple[str],
     encoding: str = "utf-8",
     newline: bool = True,
 ) -> None:
     """Write content to a target file encoded as UTF-8. If optional newline is specified
     append each line with a newline escape sequence (`\n`).
 
     Parameters:
-        filepath (str): path to target file (if file does not exist it will be created)
+        filepath (pathlib.Path | str): path to target file (if file does not exist it will be created)
         data (list | tuple): sequence of strings comprising the content to be written to the
                              target file
         encoding (str): name of encoding used to encode the file.
         newline (bool): add newline escape sequence to line
 
     Returns:
         None
@@ -149,15 +153,15 @@
             for line in data:
                 file_obj.write(f"{line}\n")  # add newline
         else:
             file_obj.writelines(data)  # write sequence to file
 
 
 def write_csv(
-    filepath: str,
+    filepath: pathlib.Path | str,
     data: list | tuple,
     headers: Optional[list | tuple] = None,
     encoding: str = "utf-8",
     newline: str = "",
 ) -> None:
     """
 
@@ -165,15 +169,15 @@
     row of the CSV file if optional headers are specified.
 
     WARN: If newline='' is not specified, newlines '\n' or '\r\n' embedded inside quoted
     fields may not be interpreted correctly by the csv.reader. On platforms that utilize
     `\r\n` an extra `\r` will be added.
 
     Parameters:
-        filepath (str): path to target file (if file does not exist it will be created)
+        filepath (pathlib.Path | str): path to target file (if file does not exist it will be created)
         data (list | tuple): sequence to be written to the target file
         headers (seq): optional header row list or tuple
         encoding (str): name of encoding used to encode the file
         newline (str): specifies replacement value for newline '\n'
                        or '\r\n' (Windows) character sequences
 
     Returns:
@@ -186,15 +190,15 @@
         stacklevel=2,
     )
 
     return to_csv(filepath, data, headers, encoding, newline)
 
 
 def write_dicts_to_csv(
-    filepath: str,
+    filepath: pathlib.Path | str,
     data: List[dict],
     fieldnames: list | tuple,
     encoding: str = "utf-8",
     newline: str = "",
 ) -> None:
     """
     Writes dictionary data to a target CSV file as row data using the csv.DictWriter().
@@ -202,15 +206,15 @@
     in which each dictionary's key-value pairs are written to the row.
 
     WARN: This function is not designed to handle dictionaries that include key-value
     pairs in which the values are sequences or dictionaries. In such cases, serialize the
     object as JSON and write to a file using < write.write_json >.
 
     Parameters:
-        filepath (str): path to target file (if file does not exist it will be created)
+        filepath (pathlib.Path | str): path to target file (if file does not exist it will be created)
         data (list): dictionary content to be written to the target file
         fieldnames (seq): sequence specifing order in which key-value pairs are written to each row
         encoding (str): name of encoding used to encode the file
         newline (str): specifies replacement value for newline '\n'
                        or '\r\n' (Windows) character sequences
 
     Returns:
@@ -223,24 +227,24 @@
         stacklevel=2,
     )
 
     return dicts_to_csv(filepath, data, fieldnames, encoding, newline)
 
 
 def write_file(
-    filepath: str,
+    filepath: pathlib.Path | str,
     data: List[str] | Tuple[str],
     encoding: str = "utf-8",
     newline: bool = True,
 ) -> None:
     """Write content to a target file encoded as UTF-8. If optional newline is specified
     append each line with a newline escape sequence (`\n`).
 
     Parameters:
-        filepath (str): path to target file (if file does not exist it will be created)
+        filepath (pathlib.Path | str): path to target file (if file does not exist it will be created)
         data (list | tuple): sequence of strings comprising the content to be written to the
                              target file
         encoding (str): name of encoding used to encode the file.
         newline (bool): add newline escape sequence to line
 
     Returns:
         None
@@ -252,23 +256,26 @@
         stacklevel=2,
     )
 
     return to_txt(filepath, data, encoding, newline)
 
 
 def write_file_response_chunked(
-    filepath: str, response: requests.Response, mode: str = "w", chunk_size: int = 1024
+    filepath: pathlib.Path | str,
+    response: requests.Response,
+    mode: str = "w",
+    chunk_size: int = 1024,
 ) -> None:
     """Writes < requests.Response > to a target file as a stream of data chunks.
     Override the optional write mode value if binary content <class 'bytes'> is to
     be written to file (i.e., mode='wb') or an append operation is intended on an
     existing file (i.e., mode='a' or 'ab').
 
     Parameters:
-        filepath (str): absolute or relative path to target file
+        filepath (pathlib.Path | str): absolute or relative path to target file
         response (requests.Response): data to be written to the target file
         mode (str): write operation mode
         chunk_size (int); size of data chunks to stream
 
     Returns:
         None
     """
@@ -279,24 +286,24 @@
         stacklevel=2,
     )
 
     return to_file_response_chunked(filepath, response, mode, chunk_size)
 
 
 def write_json(
-    filepath: str,
+    filepath: pathlib.Path | str,
     data: dict | list,
     encoding: str = "utf-8",
     ensure_ascii: bool = False,
     indent: int = 2,
 ) -> None:
     """Serializes object as JSON. Writes content to the provided filepath.
 
     Parameters:
-        filepath (str): the path to the file
+        filepath (pathlib.Path | str): the path to the file
         data (dict | list): the data to be encoded as JSON and written to the file
         encoding (str): name of encoding used to encode the file
         ensure_ascii (str): if False non-ASCII characters are printed as is; otherwise
                             non-ASCII characters are escaped.
         indent (int): number of "pretty printed" indention spaces applied to encoded JSON
 
     Returns:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `umpyutl-2.1.0/.gitignore` & `umpyutl-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `umpyutl-2.1.0/LICENSE` & `umpyutl-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `umpyutl-2.1.0/pyproject.toml` & `umpyutl-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `umpyutl-2.1.0/PKG-INFO` & `umpyutl-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: umpyutl
-Version: 2.1.0
+Version: 2.1.1
 Summary: Utility classes and functions.
 Project-URL: Homepage, https://github.com/umsi-arwhyte/umpyutl
 Author-email: Anthony Whyte <anthwhyte@gmail.com>
 License: BSD-3-Clause
 License-File: LICENSE
 Keywords: arwhyte,umpyutl,utilities
 Classifier: License :: OSI Approved :: BSD License
```

