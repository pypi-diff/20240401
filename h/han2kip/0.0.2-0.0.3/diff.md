# Comparing `tmp/han2kip-0.0.2.tar.gz` & `tmp/han2kip-0.0.3.tar.gz`

## Comparing `han2kip-0.0.2.tar` & `han2kip-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0   901007 2020-02-02 00:00:00.000000 han2kip-0.0.2/data/dict.txt
--rw-r--r--   0        0        0  2312337 2020-02-02 00:00:00.000000 han2kip-0.0.2/data/words.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 han2kip-0.0.2/han2kip/__init__.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 han2kip-0.0.2/han2kip/kip_converter.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 han2kip-0.0.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 han2kip-0.0.2/LICENSE
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 han2kip-0.0.2/README.md
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 han2kip-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 han2kip-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 han2kip-0.0.3/data/__init__.py
+-rw-r--r--   0        0        0   901007 2020-02-02 00:00:00.000000 han2kip-0.0.3/data/dict.txt
+-rw-r--r--   0        0        0  2312337 2020-02-02 00:00:00.000000 han2kip-0.0.3/data/words.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 han2kip-0.0.3/han2kip/__init__.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 han2kip-0.0.3/han2kip/kip_converter.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 han2kip-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 han2kip-0.0.3/LICENSE
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 han2kip-0.0.3/README.md
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 han2kip-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 han2kip-0.0.3/PKG-INFO
```

### Comparing `han2kip-0.0.2/data/dict.txt` & `han2kip-0.0.3/data/dict.txt`

 * *Files identical despite different names*

### Comparing `han2kip-0.0.2/data/words.json` & `han2kip-0.0.3/data/words.json`

 * *Files identical despite different names*

### Comparing `han2kip-0.0.2/han2kip/kip_converter.py` & `han2kip-0.0.3/han2kip/kip_converter.py`

 * *Files identical despite different names*

### Comparing `han2kip-0.0.2/.gitignore` & `han2kip-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `han2kip-0.0.2/LICENSE` & `han2kip-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `han2kip-0.0.2/pyproject.toml` & `han2kip-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6861 6e32 6b69 7022 0d0a 7665 7273   "han2kip"..vers
-00000070: 696f 6e20 3d20 2230 2e30 2e32 220d 0a61  ion = "0.0.2"..a
+00000070: 696f 6e20 3d20 2230 2e30 2e33 220d 0a61  ion = "0.0.3"..a
 00000080: 7574 686f 7273 203d 205b 0d0a 2020 7b20  uthors = [..  { 
 00000090: 6e61 6d65 3d22 e69e 97e6 80a1 e890 b122  name="........."
 000000a0: 2c20 656d 6169 6c3d 2271 7731 3233 3435  , email="qw12345
 000000b0: 3535 3434 4067 6d61 696c 2e63 6f6d 227d  5544@gmail.com"}
 000000c0: 2c20 7b20 6e61 6d65 3d22 e69e 97e6 9f8f  , { name="......
 000000d0: e5bb b722 2c20 656d 6169 6c3d 2262 6f74  ...", email="bot
 000000e0: 696e 686f 6c6d 6573 4067 6d61 696c 2e63  inholmes@gmail.c
```

### Comparing `han2kip-0.0.2/PKG-INFO` & `han2kip-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: han2kip
-Version: 0.0.2
+Version: 0.0.3
 Summary: han2kip is a package for converting Taiwanese Hokkien Hanzi to its phonetic representation.
 Project-URL: Homepage, https://github.com/juliaouo/han2kip
 Author-email: 林怡萱 <qw123455544@gmail.com>, 林柏廷 <botinholmes@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 juliaouo
```

