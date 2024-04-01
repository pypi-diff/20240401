# Comparing `tmp/eseq-0.0.3.tar.gz` & `tmp/eseq-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eseq-0.0.3.tar", last modified: Tue Mar 26 00:31:53 2024, max compression
+gzip compressed data, was "eseq-0.0.4.tar", last modified: Mon Apr  1 20:04:29 2024, max compression
```

## Comparing `eseq-0.0.3.tar` & `eseq-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 00:31:53.893596 eseq-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-26 00:31:49.000000 eseq-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-26 00:31:53.889596 eseq-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-26 00:31:49.000000 eseq-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 00:31:53.889596 eseq-0.0.3/eseq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-26 00:31:53.000000 eseq-0.0.3/eseq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-26 00:31:53.000000 eseq-0.0.3/eseq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 00:31:53.000000 eseq-0.0.3/eseq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-26 00:31:53.000000 eseq-0.0.3/eseq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-26 00:31:53.000000 eseq-0.0.3/eseq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 00:31:53.893596 eseq-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-03-26 00:31:49.000000 eseq-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 00:31:53.889596 eseq-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 00:31:49.000000 eseq-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-26 00:31:49.000000 eseq-0.0.3/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-26 00:31:49.000000 eseq-0.0.3/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 00:31:53.889596 eseq-0.0.3/tests/unittests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 00:31:49.000000 eseq-0.0.3/tests/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-03-26 00:31:49.000000 eseq-0.0.3/tests/unittests/test_bio_dna.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-03-26 00:31:49.000000 eseq-0.0.3/tests/unittests/test_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-26 00:31:49.000000 eseq-0.0.3/tests/unittests/test_dna.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-03-26 00:31:49.000000 eseq-0.0.3/tests/unittests/test_orf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-26 00:31:49.000000 eseq-0.0.3/tests/unittests/test_palindromic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-26 00:31:49.000000 eseq-0.0.3/tests/unittests/test_prosite.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-26 00:31:49.000000 eseq-0.0.3/tests/unittests/test_protein.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-26 00:31:49.000000 eseq-0.0.3/tests/unittests/test_rna.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-03-26 00:31:49.000000 eseq-0.0.3/tests/unittests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-03-26 00:31:49.000000 eseq-0.0.3/tests/unittests/test_seq.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-26 00:31:49.000000 eseq-0.0.3/tests/unittests/test_seq_trie.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-26 00:31:49.000000 eseq-0.0.3/tests/unittests/test_trim_seq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:04:29.283542 eseq-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 20:04:22.000000 eseq-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-01 20:04:29.283542 eseq-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-01 20:04:22.000000 eseq-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:04:29.283542 eseq-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-01 20:04:22.000000 eseq-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:04:29.279542 eseq-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:04:29.279542 eseq-0.0.4/src/eseq/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-01 20:04:22.000000 eseq-0.0.4/src/eseq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-01 20:04:22.000000 eseq-0.0.4/src/eseq/bio_dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-01 20:04:22.000000 eseq-0.0.4/src/eseq/dna.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:04:29.283542 eseq-0.0.4/src/eseq/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:04:22.000000 eseq-0.0.4/src/eseq/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-01 20:04:22.000000 eseq-0.0.4/src/eseq/model/compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-01 20:04:22.000000 eseq-0.0.4/src/eseq/model/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-01 20:04:22.000000 eseq-0.0.4/src/eseq/model/seq_trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-01 20:04:22.000000 eseq-0.0.4/src/eseq/orf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-01 20:04:22.000000 eseq-0.0.4/src/eseq/palindromic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-01 20:04:22.000000 eseq-0.0.4/src/eseq/prosite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-01 20:04:22.000000 eseq-0.0.4/src/eseq/protein.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-01 20:04:22.000000 eseq-0.0.4/src/eseq/rna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-01 20:04:22.000000 eseq-0.0.4/src/eseq/seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-01 20:04:22.000000 eseq-0.0.4/src/eseq/trim_seq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:04:29.283542 eseq-0.0.4/src/eseq/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-01 20:04:22.000000 eseq-0.0.4/src/eseq/utils/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:04:29.283542 eseq-0.0.4/src/eseq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-01 20:04:29.000000 eseq-0.0.4/src/eseq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-01 20:04:29.000000 eseq-0.0.4/src/eseq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:04:29.000000 eseq-0.0.4/src/eseq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-01 20:04:29.000000 eseq-0.0.4/src/eseq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 20:04:29.000000 eseq-0.0.4/src/eseq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:04:29.283542 eseq-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-01 20:04:22.000000 eseq-0.0.4/tests/test_env.py
```

### Comparing `eseq-0.0.3/LICENSE` & `eseq-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eseq-0.0.3/PKG-INFO` & `eseq-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eseq
-Version: 0.0.3
+Version: 0.0.4
 Summary: Process genomic sequences.
 Home-page: https://github.com/Tiezhengyuan/bio_sequence.git
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `eseq-0.0.3/README.md` & `eseq-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `eseq-0.0.3/eseq.egg-info/PKG-INFO` & `eseq-0.0.4/src/eseq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eseq
-Version: 0.0.3
+Version: 0.0.4
 Summary: Process genomic sequences.
 Home-page: https://github.com/Tiezhengyuan/bio_sequence.git
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `eseq-0.0.3/setup.py` & `eseq-0.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="eseq",
-    version='0.0.3',
+    version='0.0.4',
     author="Tiezheng Yuan",
     author_email="tiezhengyuan@hotmail.com",
     description="Process genomic sequences.",
     url = "https://github.com/Tiezhengyuan/bio_sequence.git",
     long_description_content_type="text/markdown",
     long_description=long_description,
-    packages=find_packages(),
+    package_dir={'': 'src'},
     install_requires=['Bio',],
     keywords=['pypi', 'cicd', 'python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

