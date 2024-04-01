# Comparing `tmp/KeyDnn-0.8.0.tar.gz` & `tmp/KeyDnn-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KeyDnn-0.8.0.tar", last modified: Sun Jan  7 11:59:00 2024, max compression
+gzip compressed data, was "KeyDnn-0.9.0.tar", last modified: Thu Jan 25 14:29:06 2024, max compression
```

## Comparing `KeyDnn-0.8.0.tar` & `KeyDnn-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-01-07 11:59:00.169808 KeyDnn-0.8.0/
--rw-rw-rw-   0        0        0     1066 2023-12-26 16:46:07.000000 KeyDnn-0.8.0/LICENSE
--rw-rw-rw-   0        0        0      762 2024-01-07 11:59:00.168300 KeyDnn-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0       46 2023-12-26 16:58:03.000000 KeyDnn-0.8.0/README.md
--rw-rw-rw-   0        0        0      102 2023-12-26 16:46:38.000000 KeyDnn-0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-07 11:59:00.170818 KeyDnn-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1395 2024-01-07 11:34:23.000000 KeyDnn-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-07 11:59:00.100256 KeyDnn-0.8.0/src/
-drwxrwxrwx   0        0        0        0 2024-01-07 11:59:00.167299 KeyDnn-0.8.0/src/KeyDnn.egg-info/
--rw-rw-rw-   0        0        0      762 2024-01-07 11:59:00.000000 KeyDnn-0.8.0/src/KeyDnn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2024-01-07 11:59:00.000000 KeyDnn-0.8.0/src/KeyDnn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-07 11:59:00.000000 KeyDnn-0.8.0/src/KeyDnn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-01-07 11:59:00.000000 KeyDnn-0.8.0/src/KeyDnn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-01-07 11:59:00.000000 KeyDnn-0.8.0/src/KeyDnn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-07 11:59:00.159026 KeyDnn-0.8.0/src/keydnn/
--rw-rw-rw-   0        0        0      222 2023-12-28 16:19:52.000000 KeyDnn-0.8.0/src/keydnn/__init__.py
--rw-rw-rw-   0        0        0     9670 2024-01-07 07:07:28.000000 KeyDnn-0.8.0/src/keydnn/activations.py
-drwxrwxrwx   0        0        0        0 2024-01-07 11:59:00.164066 KeyDnn-0.8.0/src/keydnn/bin/
--rw-rw-rw-   0        0        0    20120 2023-12-29 09:22:54.000000 KeyDnn-0.8.0/src/keydnn/bin/conv_lib_linux.so
--rw-rw-rw-   0        0        0    57715 2023-12-29 09:20:32.000000 KeyDnn-0.8.0/src/keydnn/bin/conv_lib_windows.dll
--rw-rw-rw-   0        0        0    15742 2023-12-29 09:27:52.000000 KeyDnn-0.8.0/src/keydnn/conv_utils.py
--rw-rw-rw-   0        0        0    28692 2024-01-07 11:56:28.000000 KeyDnn-0.8.0/src/keydnn/layers.py
--rw-rw-rw-   0        0        0     5976 2023-12-30 10:40:15.000000 KeyDnn-0.8.0/src/keydnn/losses.py
--rw-rw-rw-   0        0        0     9592 2024-01-07 06:18:05.000000 KeyDnn-0.8.0/src/keydnn/models.py
--rw-rw-rw-   0        0        0     2506 2023-12-29 05:14:28.000000 KeyDnn-0.8.0/src/keydnn/threading_utils.py
--rw-rw-rw-   0        0        0     6551 2023-12-30 11:10:12.000000 KeyDnn-0.8.0/src/keydnn/utilities.py
+drwxrwxrwx   0        0        0        0 2024-01-25 14:29:06.263359 KeyDnn-0.9.0/
+-rw-rw-rw-   0        0        0     1066 2023-12-26 16:46:07.000000 KeyDnn-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      762 2024-01-25 14:29:06.261359 KeyDnn-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2023-12-26 16:58:03.000000 KeyDnn-0.9.0/README.md
+-rw-rw-rw-   0        0        0      102 2023-12-26 16:46:38.000000 KeyDnn-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-01-25 14:29:06.264362 KeyDnn-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1395 2024-01-25 14:28:08.000000 KeyDnn-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-25 14:29:06.123747 KeyDnn-0.9.0/src/
+drwxrwxrwx   0        0        0        0 2024-01-25 14:29:06.259355 KeyDnn-0.9.0/src/KeyDnn.egg-info/
+-rw-rw-rw-   0        0        0      762 2024-01-25 14:29:06.000000 KeyDnn-0.9.0/src/KeyDnn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2024-01-25 14:29:06.000000 KeyDnn-0.9.0/src/KeyDnn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-25 14:29:06.000000 KeyDnn-0.9.0/src/KeyDnn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-01-25 14:29:06.000000 KeyDnn-0.9.0/src/KeyDnn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-01-25 14:29:06.000000 KeyDnn-0.9.0/src/KeyDnn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-01-25 14:29:06.224853 KeyDnn-0.9.0/src/keydnn/
+-rw-rw-rw-   0        0        0      222 2023-12-28 16:19:52.000000 KeyDnn-0.9.0/src/keydnn/__init__.py
+-rw-rw-rw-   0        0        0     9670 2024-01-07 07:07:28.000000 KeyDnn-0.9.0/src/keydnn/activations.py
+drwxrwxrwx   0        0        0        0 2024-01-25 14:29:06.256355 KeyDnn-0.9.0/src/keydnn/bin/
+-rw-rw-rw-   0        0        0    20120 2023-12-29 09:22:54.000000 KeyDnn-0.9.0/src/keydnn/bin/conv_lib_linux.so
+-rw-rw-rw-   0        0        0    57715 2023-12-29 09:20:32.000000 KeyDnn-0.9.0/src/keydnn/bin/conv_lib_windows.dll
+-rw-rw-rw-   0        0        0    15742 2023-12-29 09:27:52.000000 KeyDnn-0.9.0/src/keydnn/conv_utils.py
+-rw-rw-rw-   0        0        0    28692 2024-01-07 11:56:28.000000 KeyDnn-0.9.0/src/keydnn/layers.py
+-rw-rw-rw-   0        0        0     5976 2023-12-30 10:40:15.000000 KeyDnn-0.9.0/src/keydnn/losses.py
+-rw-rw-rw-   0        0        0     9592 2024-01-07 06:18:05.000000 KeyDnn-0.9.0/src/keydnn/models.py
+-rw-rw-rw-   0        0        0     2506 2023-12-29 05:14:28.000000 KeyDnn-0.9.0/src/keydnn/threading_utils.py
+-rw-rw-rw-   0        0        0     8155 2024-01-25 14:27:49.000000 KeyDnn-0.9.0/src/keydnn/utilities.py
```

### Comparing `KeyDnn-0.8.0/LICENSE` & `KeyDnn-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `KeyDnn-0.8.0/PKG-INFO` & `KeyDnn-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyDnn
-Version: 0.8.0
+Version: 0.9.0
 Summary: Deep Learning Framework Implemented by Kevin Sheu.
 Home-page: https://github.com/keywind127/keydnn
 Author: Keywind
 Author-email: watersprayer127@gmail.com
 Project-URL: Bug Tracker, https://github.com/keywind127/keydnn/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `KeyDnn-0.8.0/setup.py` & `KeyDnn-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", mode = "r", encoding = "utf-8") as fh:
 	long_description = fh.read()
 	
 setuptools.setup(
 	
 	name                          = "KeyDnn",
-	version                       = "0.8.0",
+	version                       = "0.9.0",
 	author                        = "Keywind",
 	author_email                  = "watersprayer127@gmail.com",
 	description                   = "Deep Learning Framework Implemented by Kevin Sheu.",
 	long_description              = long_description,
 	long_description_content_type = "text/markdown",
 	url                           = "https://github.com/keywind127/keydnn",
 	project_urls                  = {
```

### Comparing `KeyDnn-0.8.0/src/KeyDnn.egg-info/PKG-INFO` & `KeyDnn-0.9.0/src/KeyDnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyDnn
-Version: 0.8.0
+Version: 0.9.0
 Summary: Deep Learning Framework Implemented by Kevin Sheu.
 Home-page: https://github.com/keywind127/keydnn
 Author: Keywind
 Author-email: watersprayer127@gmail.com
 Project-URL: Bug Tracker, https://github.com/keywind127/keydnn/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `KeyDnn-0.8.0/src/keydnn/activations.py` & `KeyDnn-0.9.0/src/keydnn/activations.py`

 * *Files identical despite different names*

### Comparing `KeyDnn-0.8.0/src/keydnn/bin/conv_lib_linux.so` & `KeyDnn-0.9.0/src/keydnn/bin/conv_lib_linux.so`

 * *Files identical despite different names*

### Comparing `KeyDnn-0.8.0/src/keydnn/bin/conv_lib_windows.dll` & `KeyDnn-0.9.0/src/keydnn/bin/conv_lib_windows.dll`

 * *Files identical despite different names*

### Comparing `KeyDnn-0.8.0/src/keydnn/conv_utils.py` & `KeyDnn-0.9.0/src/keydnn/conv_utils.py`

 * *Files identical despite different names*

### Comparing `KeyDnn-0.8.0/src/keydnn/layers.py` & `KeyDnn-0.9.0/src/keydnn/layers.py`

 * *Files identical despite different names*

### Comparing `KeyDnn-0.8.0/src/keydnn/losses.py` & `KeyDnn-0.9.0/src/keydnn/losses.py`

 * *Files identical despite different names*

### Comparing `KeyDnn-0.8.0/src/keydnn/models.py` & `KeyDnn-0.9.0/src/keydnn/models.py`

 * *Files identical despite different names*

### Comparing `KeyDnn-0.8.0/src/keydnn/threading_utils.py` & `KeyDnn-0.9.0/src/keydnn/threading_utils.py`

 * *Files identical despite different names*

### Comparing `KeyDnn-0.8.0/src/keydnn/utilities.py` & `KeyDnn-0.9.0/src/keydnn/utilities.py`

 * *Files 20% similar despite different names*

```diff
@@ -201,14 +201,58 @@
         return __catch_error
     
     return _catch_error
 
 def initialize_weights(target_size : tuple, n_input_nodes : int) -> np.ndarray:
     return np.random.randn(*target_size).reshape(target_size) * np.sqrt(2.0 / n_input_nodes)
 
+class NeoVisUtils(object):
+
+    SAFE_MODE = True
+
+    @classmethod
+    def apply_filter_condition(cls, f_query_string : str, condition : Dict[ str, str ]) -> str:
+
+        if (cls.SAFE_MODE):
+
+            assert isinstance(f_query_string, str)
+
+            assert isinstance(condition, dict)
+
+        return f_query_string.format(f"""{{{  ",".join(map(lambda x : f"{x[0]}: {repr(x[1])}", condition.items()))  }}}""")
+
+    @classmethod
+    def create_node_query_string(cls, counter : int, query_data : List[ Dict[ str, str ] ]) -> str:
+
+        if (cls.SAFE_MODE):
+
+            assert isinstance(counter, int)
+
+            assert isinstance(query_data, list)
+
+        if (counter == 1):
+            return f"p{counter} = (n{counter}: `{query_data[counter-1][0]}`{{}})"
+
+        return f"p{counter} = (n{counter}) - [r{counter}] -> (n{counter}: `{query_data[counter-1][0]}`{{}})"
+
+    @classmethod
+    def format_query(cls, query_data : List[ Dict[ str, str ] ]) -> str:
+
+        if (cls.SAFE_MODE):
+            assert isinstance(query_data, list)
+
+        query_string = cls.apply_filter_condition(f"MATCH {cls.create_node_query_string(1, query_data)}", query_data[0][1])
+
+        for counter in range(2, len(query_data) + 1):
+            query_string += cls.apply_filter_condition(f" OPTIONAL MATCH p{counter} = (n{counter-1}) - [r{counter-1}] -> (n{counter}: `{query_data[counter-1][0]}`{{}})", query_data[counter-1][1])
+
+        query_string += " RETURN " + ", ".join(f"p{counter}" for counter in range(1, len(query_data) + 1))
+
+        return query_string
+
 epsilon = 1e-7
 
 if (__name__ == "__main__"):
 
     @catch_error()
     def parse_int(string : str) -> int:
         return int(string)
```

