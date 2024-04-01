# Comparing `tmp/parseid-0.1.2-py3-none-any.whl.zip` & `tmp/parseid-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6888 bytes, number of entries: 11
--rw-r--r--  2.0 unx      147 b- defN 24-Apr-01 14:14 parseid/__init__.py
--rw-r--r--  2.0 unx      236 b- defN 24-Apr-01 14:14 parseid/constants.py
--rw-r--r--  2.0 unx     1980 b- defN 24-Apr-01 14:14 parseid/ditrie.py
--rw-r--r--  2.0 unx     2063 b- defN 24-Apr-01 14:14 parseid/process_id.py
--rw-r--r--  2.0 unx      696 b- defN 24-Apr-01 14:14 parseid/read_file.py
--rw-r--r--  2.0 unx     5912 b- defN 24-Apr-01 14:14 parseid/trie.py
--rw-r--r--  2.0 unx     1629 b- defN 24-Apr-01 14:14 parseid/trie_node.py
--rw-r--r--  2.0 unx     2449 b- defN 24-Apr-01 14:14 parseid-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-01 14:14 parseid-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-01 14:14 parseid-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      825 b- defN 24-Apr-01 14:14 parseid-0.1.2.dist-info/RECORD
-11 files, 16037 bytes uncompressed, 5510 bytes compressed:  65.6%
+Zip file size: 5343 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 14:16 tests/__init__.py
+-rw-r--r--  2.0 unx      384 b- defN 24-Apr-01 14:16 tests/helper.py
+-rw-r--r--  2.0 unx     1286 b- defN 24-Apr-01 14:16 tests/test_ditrie.py
+-rw-r--r--  2.0 unx      206 b- defN 24-Apr-01 14:16 tests/test_env.py
+-rw-r--r--  2.0 unx      894 b- defN 24-Apr-01 14:16 tests/test_process_id.py
+-rw-r--r--  2.0 unx     4757 b- defN 24-Apr-01 14:16 tests/test_trie.py
+-rw-r--r--  2.0 unx     1073 b- defN 24-Apr-01 14:16 tests/test_trie_node.py
+-rw-r--r--  2.0 unx     2449 b- defN 24-Apr-01 14:16 parseid-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-01 14:16 parseid-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-01 14:16 parseid-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      824 b- defN 24-Apr-01 14:16 parseid-0.1.3.dist-info/RECORD
+11 files, 11971 bytes uncompressed, 3961 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -1,34 +1,34 @@
-Filename: parseid/__init__.py
+Filename: tests/__init__.py
 Comment: 
 
-Filename: parseid/constants.py
+Filename: tests/helper.py
 Comment: 
 
-Filename: parseid/ditrie.py
+Filename: tests/test_ditrie.py
 Comment: 
 
-Filename: parseid/process_id.py
+Filename: tests/test_env.py
 Comment: 
 
-Filename: parseid/read_file.py
+Filename: tests/test_process_id.py
 Comment: 
 
-Filename: parseid/trie.py
+Filename: tests/test_trie.py
 Comment: 
 
-Filename: parseid/trie_node.py
+Filename: tests/test_trie_node.py
 Comment: 
 
-Filename: parseid-0.1.2.dist-info/METADATA
+Filename: parseid-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: parseid-0.1.2.dist-info/WHEEL
+Filename: parseid-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: parseid-0.1.2.dist-info/top_level.txt
+Filename: parseid-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: parseid-0.1.2.dist-info/RECORD
+Filename: parseid-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `parseid-0.1.2.dist-info/METADATA` & `parseid-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parseid
-Version: 0.1.2
+Version: 0.1.3
 Summary: suck, parse identifiers or accession numbers
 Home-page: https://github.com/Tiezhengyuan/parse_identifier
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

