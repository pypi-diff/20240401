# Comparing `tmp/importmonkey-1.0.0-py3-none-any.whl.zip` & `tmp/importmonkey-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 4612 bytes, number of entries: 5
--rw-r--r--  2.0 unx     5612 b- defN 23-Nov-04 10:51 importmonkey/__init__.py
--rw-r--r--  2.0 unx     4131 b- defN 23-Nov-04 10:52 importmonkey-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Nov-04 10:52 importmonkey-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Nov-04 10:52 importmonkey-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      399 b- defN 23-Nov-04 10:52 importmonkey-1.0.0.dist-info/RECORD
-5 files, 10247 bytes uncompressed, 3866 bytes compressed:  62.3%
+Zip file size: 4597 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     5535 b- defN 24-Apr-01 13:39 importmonkey/__init__.py
+-rw-r--r--  2.0 unx     4131 b- defN 24-Apr-01 13:40 importmonkey-2.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-01 13:40 importmonkey-2.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-01 13:40 importmonkey-2.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      399 b- defN 24-Apr-01 13:40 importmonkey-2.0.0.dist-info/RECORD
+5 files, 10170 bytes uncompressed, 3851 bytes compressed:  62.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: importmonkey/__init__.py
 Comment: 
 
-Filename: importmonkey-1.0.0.dist-info/METADATA
+Filename: importmonkey-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: importmonkey-1.0.0.dist-info/WHEEL
+Filename: importmonkey-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: importmonkey-1.0.0.dist-info/top_level.txt
+Filename: importmonkey-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: importmonkey-1.0.0.dist-info/RECORD
+Filename: importmonkey-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## importmonkey/__init__.py

```diff
@@ -1,31 +1,31 @@
 #!/usr/bin/env python3
 
 """This is importmonkey. See the only function, add_path, for documentation."""
 
+import inspect
+import pathlib
+import sys
+
 # Updating __version__ information:
 #     * Format is <major>.<minor>.<patch>
-#     * Never use leading or trailing zeroes in any of minor/major/patch.
+#     * Never use leading or trailing zeroes in any of major/minor/patch.
 #     * A lone zero is allowed.
 #     * Increment more if an increment results in a leading or trailing zero.
 #     * Incrementing major resets minor and patch to 0.
 #     * Incrementing minor resets patch to 0.
 #     * Incrementing patch does not affect other numbers.
 #     * Never decrement a number except when resetting to zero like above.
 
-__version__ = "1.0.0"
+__version__ = "2.0.0"
 __all__ = ["add_path"]
 __author__ = "Markus Hirsimäki"
 __copyright__ = "This work is dedicated to public domain under The Unlicense."
 __license__ = "The Unlicense (https://choosealicense.com/licenses/unlicense/)"
 
-import sys
-import inspect
-import pathlib
-
 
 def add_path(new_path, allow_backslashes=False):
     """Adds a new path to sys.path relative to the caller's file's directory.
 
     The basis for the relative path being added is the __file__ attribute of
     the caller. You can inspect the path by simply doing print(__file__). If
     new_path argument is an absolute path, the base path from __file__ is
@@ -62,20 +62,20 @@
     Args:
         new_path (str): The path to be added, relative to the caller's file.
         allow_backslashes (bool, optional): Allow backslashes in path. Default
             is False. You should only use this if you are certain you need
             backslashes. Unix-style paths can and should be used on Windows.
 
     Returns:
-        str: The path that was added to sys.path.
+        str: The path that was added to sys.path or empty string if the path
+            was already found in sys.path.
 
     Raises:
         TypeError: If new_path or allow_backslashes has wrong type.
         ValueError: If new_path does not resolve to a valid directory.
-        ValueError: If new_path already exists in sys.path.
         FileNotFoundError: If the caller's filepath can not be determined.
         RuntimeError: For unexpected exceptions.
     """
     if type(new_path) is not str:
         msg = (
             "Was expecting the new_path argument to be a string."
             f" Found {repr(type(new_path))} instead."
@@ -130,11 +130,10 @@
         )
         raise ValueError(msg)
 
     final_path_str = str(final_path)
 
     if final_path_str not in sys.path:
         sys.path.append(final_path_str)
+        return final_path_str
     else:
-        msg = f"The path {repr(final_path_str)} is already found in sys.path."
-        raise ValueError(msg)
-    return final_path_str
+        return ""
```

## Comparing `importmonkey-1.0.0.dist-info/METADATA` & `importmonkey-2.0.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importmonkey
-Version: 1.0.0
+Version: 2.0.0
 Summary: Utility for adding new import paths.
 Author: Markus Hirsimäki
 License: The Unlicense
 Project-URL: homepage, https://github.com/hirsimaki-markus/importmonkey
 Project-URL: license, https://choosealicense.com/licenses/unlicense/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: importmonkey Version: 1.0.0 Summary: Utility for
+Metadata-Version: 2.1 Name: importmonkey Version: 2.0.0 Summary: Utility for
 adding new import paths. Author: Markus HirsimÃ¤ki License: The Unlicense
 Project-URL: homepage, https://github.com/hirsimaki-markus/importmonkey
 Project-URL: license, https://choosealicense.com/licenses/unlicense/
 Classifier: Development Status :: 5 - Production/Stable Classifier: Programming
 Language :: Python Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Classifier:
 Programming Language :: Python :: 3.3 Classifier: Programming Language ::
```

