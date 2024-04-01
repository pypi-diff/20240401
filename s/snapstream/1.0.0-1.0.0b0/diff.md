# Comparing `tmp/snapstream-1.0.0.tar.gz` & `tmp/snapstream-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapstream-1.0.0.tar", max compression
+gzip compressed data, was "snapstream-1.0.0b0.tar", max compression
```

## Comparing `snapstream-1.0.0.tar` & `snapstream-1.0.0b0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2024-04-01 19:16:01.293168 snapstream-1.0.0/LICENSE
--rw-r--r--   0        0        0     2536 2024-04-01 19:16:01.293168 snapstream-1.0.0/README.md
--rw-r--r--   0        0        0     2034 2024-04-01 19:16:12.165234 snapstream-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2280 2024-04-01 19:16:01.297168 snapstream-1.0.0/snapstream/__init__.py
--rw-r--r--   0        0        0     8347 2024-04-01 19:16:01.297168 snapstream-1.0.0/snapstream/__main__.py
--rw-r--r--   0        0        0    10462 2024-04-01 19:16:01.297168 snapstream-1.0.0/snapstream/caching.py
--rw-r--r--   0        0        0     2889 2024-04-01 19:16:01.297168 snapstream-1.0.0/snapstream/codecs.py
--rw-r--r--   0        0        0    11072 2024-04-01 19:16:01.297168 snapstream-1.0.0/snapstream/core.py
--rw-r--r--   0        0        0     3623 2024-04-01 19:16:01.297168 snapstream-1.0.0/snapstream/utils.py
--rw-r--r--   0        0        0     4199 1970-01-01 00:00:00.000000 snapstream-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-22 22:36:56.125909 snapstream-1.0.0b0/LICENSE
+-rw-r--r--   0        0        0     2536 2024-03-22 22:36:56.125909 snapstream-1.0.0b0/README.md
+-rw-r--r--   0        0        0     2039 2024-03-22 22:37:07.985930 snapstream-1.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0     2280 2024-03-22 22:36:56.133909 snapstream-1.0.0b0/snapstream/__init__.py
+-rw-r--r--   0        0        0     8333 2024-03-22 22:36:56.133909 snapstream-1.0.0b0/snapstream/__main__.py
+-rw-r--r--   0        0        0    10462 2024-03-22 22:36:56.133909 snapstream-1.0.0b0/snapstream/caching.py
+-rw-r--r--   0        0        0     2889 2024-03-22 22:36:56.133909 snapstream-1.0.0b0/snapstream/codecs.py
+-rw-r--r--   0        0        0    11072 2024-03-22 22:36:56.133909 snapstream-1.0.0b0/snapstream/core.py
+-rw-r--r--   0        0        0     3623 2024-03-22 22:36:56.133909 snapstream-1.0.0b0/snapstream/utils.py
+-rw-r--r--   0        0        0     4201 1970-01-01 00:00:00.000000 snapstream-1.0.0b0/PKG-INFO
```

### Comparing `snapstream-1.0.0/LICENSE` & `snapstream-1.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `snapstream-1.0.0/README.md` & `snapstream-1.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `snapstream-1.0.0/pyproject.toml` & `snapstream-1.0.0b0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snapstream"
-version = "1.0.0"
+version = "1.0.0-beta"
 description = "Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions."
 authors = ["Menziess <stefan_schenk@hotmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Menziess/snapstream"
 documentation = "https://snapstream.readthedocs.io"
 license = "MIT"
 keywords = ["kafka", "pubsub"]
```

### Comparing `snapstream-1.0.0/snapstream/__init__.py` & `snapstream-1.0.0b0/snapstream/__init__.py`

 * *Files identical despite different names*

### Comparing `snapstream-1.0.0/snapstream/__main__.py` & `snapstream-1.0.0b0/snapstream/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,32 +187,32 @@
     """Read records from cache."""
     if not path.isdir(args.path):
         raise OSError(f'Folder doesn\'t exist: {args.path}')
     cache = Cache(
         args.path,
         access_type=AccessType.read_only(),
     )
-    if args.stats:
-        print()
-        print('Statistics:')
-        print(dumps(cache.live_files(), indent=4))
-        print('Folder size:', folder_size(args.path + '/**/*', 'mb'), 'mb')
-        return
     key_filter = curry(regex_filter)(args.key_filter)
     val_filter = curry(regex_filter)(args.val_filter)
     for key, val in cache.items():
         if key_filter(str(key)) and val_filter(str(val)):
             if args.columns and not isinstance(val, dict):
                 raise ValueError(f'Columns could not be extracted from {type(val)}: {val}')
             print()
             print('>>> key:', key)
             print(val) if not args.columns else print({
                 k: v for k, v in val.items() if k in args.columns.split(',')
             })
 
+    if args.stats:
+        print()
+        print('Statistics:')
+        print(dumps(cache.live_files(), indent=4))
+        print('Folder size:', folder_size(args.path + '/**/*', 'mb'), 'mb')
+
 
 def main():
     """Run main program."""
     args = get_args()
     try:
         # Construct config path
         config_path = path.join(
```

### Comparing `snapstream-1.0.0/snapstream/caching.py` & `snapstream-1.0.0b0/snapstream/caching.py`

 * *Files identical despite different names*

### Comparing `snapstream-1.0.0/snapstream/codecs.py` & `snapstream-1.0.0b0/snapstream/codecs.py`

 * *Files identical despite different names*

### Comparing `snapstream-1.0.0/snapstream/core.py` & `snapstream-1.0.0b0/snapstream/core.py`

 * *Files identical despite different names*

### Comparing `snapstream-1.0.0/snapstream/utils.py` & `snapstream-1.0.0b0/snapstream/utils.py`

 * *Files identical despite different names*

### Comparing `snapstream-1.0.0/PKG-INFO` & `snapstream-1.0.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapstream
-Version: 1.0.0
+Version: 1.0.0b0
 Summary: Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions.
 Home-page: https://github.com/Menziess/snapstream
 License: MIT
 Keywords: kafka,pubsub
 Author: Menziess
 Author-email: stefan_schenk@hotmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

