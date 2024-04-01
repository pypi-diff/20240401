# Comparing `tmp/bioomics-0.1.6.tar.gz` & `tmp/bioomics-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioomics-0.1.6.tar", last modified: Mon Mar 25 20:02:11 2024, max compression
+gzip compressed data, was "bioomics-0.1.7.tar", last modified: Mon Apr  1 16:34:07 2024, max compression
```

## Comparing `bioomics-0.1.6.tar` & `bioomics-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:02:11.149359 bioomics-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-25 20:02:04.000000 bioomics-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-25 20:02:11.149359 bioomics-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-25 20:02:04.000000 bioomics-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:02:11.149359 bioomics-0.1.6/bioomics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-25 20:02:11.000000 bioomics-0.1.6/bioomics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-25 20:02:11.000000 bioomics-0.1.6/bioomics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 20:02:11.000000 bioomics-0.1.6/bioomics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-25 20:02:11.000000 bioomics-0.1.6/bioomics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-25 20:02:11.000000 bioomics-0.1.6/bioomics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 20:02:11.149359 bioomics-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-25 20:02:04.000000 bioomics-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:02:11.149359 bioomics-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 20:02:04.000000 bioomics-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-25 20:02:04.000000 bioomics-0.1.6/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-25 20:02:04.000000 bioomics-0.1.6/tests/test_conn_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-03-25 20:02:04.000000 bioomics-0.1.6/tests/test_conn_ftplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-03-25 20:02:04.000000 bioomics-0.1.6/tests/test_conn_redis.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-25 20:02:04.000000 bioomics-0.1.6/tests/test_expasy.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-25 20:02:04.000000 bioomics-0.1.6/tests/test_mirbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-25 20:02:04.000000 bioomics-0.1.6/tests/test_ncbi.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-25 20:02:04.000000 bioomics-0.1.6/tests/test_rnacentral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:34:07.020427 bioomics-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 16:34:03.000000 bioomics-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-01 16:34:07.020427 bioomics-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-01 16:34:03.000000 bioomics-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 16:34:07.020427 bioomics-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-01 16:34:03.000000 bioomics-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:34:07.016427 bioomics-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:34:07.016427 bioomics-0.1.7/src/bioomics/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-01 16:34:03.000000 bioomics-0.1.7/src/bioomics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-01 16:34:03.000000 bioomics-0.1.7/src/bioomics/expasy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-01 16:34:03.000000 bioomics-0.1.7/src/bioomics/mirbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-01 16:34:03.000000 bioomics-0.1.7/src/bioomics/ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-01 16:34:03.000000 bioomics-0.1.7/src/bioomics/rnacentral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:34:07.020427 bioomics-0.1.7/src/bioomics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-01 16:34:07.000000 bioomics-0.1.7/src/bioomics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-01 16:34:07.000000 bioomics-0.1.7/src/bioomics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:34:07.000000 bioomics-0.1.7/src/bioomics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 16:34:07.000000 bioomics-0.1.7/src/bioomics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 16:34:07.000000 bioomics-0.1.7/src/bioomics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:34:07.020427 bioomics-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-01 16:34:03.000000 bioomics-0.1.7/tests/test_conn_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-01 16:34:03.000000 bioomics-0.1.7/tests/test_conn_ftplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-01 16:34:03.000000 bioomics-0.1.7/tests/test_conn_redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-01 16:34:03.000000 bioomics-0.1.7/tests/test_expasy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-01 16:34:03.000000 bioomics-0.1.7/tests/test_mirbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-01 16:34:03.000000 bioomics-0.1.7/tests/test_ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-01 16:34:03.000000 bioomics-0.1.7/tests/test_rnacentral.py
```

### Comparing `bioomics-0.1.6/LICENSE` & `bioomics-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bioomics-0.1.6/PKG-INFO` & `bioomics-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioomics
-Version: 0.1.6
+Version: 0.1.7
 Summary: Download, retrieve and process omics data for further bioinformatics
 Home-page: https://github.com/Tiezhengyuan/bio_omics
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `bioomics-0.1.6/bioomics.egg-info/PKG-INFO` & `bioomics-0.1.7/src/bioomics.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioomics
-Version: 0.1.6
+Version: 0.1.7
 Summary: Download, retrieve and process omics data for further bioinformatics
 Home-page: https://github.com/Tiezhengyuan/bio_omics
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `bioomics-0.1.6/setup.py` & `bioomics-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="bioomics",
-    version='0.1.6',
+    version='0.1.7',
     author="Tiezheng Yuan",
     author_email="tiezhengyuan@hotmail.com",
     description="Download, retrieve and process omics data for further bioinformatics",
     url = "https://github.com/Tiezhengyuan/bio_omics",
     long_description_content_type="text/markdown",
     long_description=long_description,
-    packages=find_packages(),
+    packages=['bioomics'],
+    package_dir={'': 'src'},
     install_requires=[
         "Bio",
         "biosequtils",
         "lxml",
         "redis",
         "sh",
     ],
```

### Comparing `bioomics-0.1.6/tests/test_conn_ftp.py` & `bioomics-0.1.7/tests/test_conn_ftp.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.1.6/tests/test_conn_ftplib.py` & `bioomics-0.1.7/tests/test_conn_ftplib.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,52 +38,52 @@
         res = cf.scan_tree(endpoint, ftp_path, pattern)
 
     @data(
         ['ftp.ncbi.nlm.nih.gov', '/pubmed', 'gz'],
     )
     @unpack
     def test_download_tree(self, endpoint, ftp_path, pattern):
-        local_path = os.path.join(env['DIR_DOWNLOAD'], 'NCBI')
+        '''
+        download all files
+        '''
+        local_path = os.path.join(DIR_DATA, 'NCBI')
         cf.download_tree(endpoint, ftp_path, pattern, local_path)
 
 
     @skip
     @data(
         ['ftp.ncbi.nlm.nih.gov', '/pubmed',
             {'/pubmed/baseline', '/pubmed/pubmedcommons', '/pubmed/updatefiles'},
             {'deleted.pmids.gz', 'id_list.txt.gz', 'J_Entrez.gz', 'J_Medline.gz'},
         ],
     )
     @unpack
-    @mock.patch.dict(os.environ, env)
     def test_parse_contents(self, endpoint, ftp_path, expect_dirs, expect_files):
         res = cf.parse_contents(endpoint, ftp_path, 'gz')
         assert set(res['dirs']) == expect_dirs
         assert res['current_path'] == ftp_path
         assert set(res['files']) == expect_files
 
 
     @skip
     @data(
         ['/pubmed/updatefiles', 'pubmed23n1237.xml.gz', True],
         ['/pubmed/updatefiles', 'wrong_file_name', False],
     )
     @unpack
-    @mock.patch.dict(os.environ, env)
     def test_download_file(self, ftp_path, file_name, expect):
         endpoint = 'ftp.ncbi.nlm.nih.gov'
         res = cf.download_file(endpoint, ftp_path, file_name, DIR_DATA)
         assert res == expect
 
     @skip
     @data(
         ['/pubmed/baseline', 'gz', False],
         ['/pubmed', 'gz', False],
         ['/wrong_path', 'gz', True],
         ['/pubmed', 'unmatched', True],
     )
     @unpack
-    @mock.patch.dict(os.environ, env)
     def test_retrieve_file_names(self, path, pattern, expect):
         endpoint = 'ftp.ncbi.nlm.nih.gov'
         res = cf.retrieve_file_names(endpoint, path, pattern)
         assert (len(res)==0) == expect
```

### Comparing `bioomics-0.1.6/tests/test_conn_redis.py` & `bioomics-0.1.7/tests/test_conn_redis.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.1.6/tests/test_mirbase.py` & `bioomics-0.1.7/tests/test_mirbase.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.1.6/tests/test_ncbi.py` & `bioomics-0.1.7/tests/test_ncbi.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,26 +3,24 @@
 '''
 from tests.helper import *
 from src.bioomics import NCBI
 
 @ddt
 class TestNCBI(TestCase):
 
-    @skip
     @data(
         ['vertebrate_mammalian', {'vertebrate_mammalian': os.path.join(DIR_DATA, \
             'NCBI/assembly_summary/vertebrate_mammalian/assembly_summary.txt')}],
         ['wrong', {}],
     )
     @unpack
     def test_download_assembly_summary(self, input, expect):
         _, res = NCBI(DIR_DATA).download_assembly_summary([input,])
         assert res == expect
 
-    @skip
     @data(
         ['https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/000/001/405/GCF_000001405.40_GRCh38.p14',
             'Homo sapiens', 'GRCh38.p14', os.path.join(DIR_DATA, 'NCBI', 'genome', \
             'Homo sapiens', 'GRCh38.p14'), 16],
     )
     @unpack
     def test_download_genome(self, ftp_path, specie, version, expect_path, expect_files):
```

### Comparing `bioomics-0.1.6/tests/test_rnacentral.py` & `bioomics-0.1.7/tests/test_rnacentral.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,10 +10,10 @@
     @data(
         ['lncbook.fasta', os.path.join(DIR_DATA, 'RNACentral', 'lncbook.fasta')],
         ['pirbase.fasta', os.path.join(DIR_DATA, 'RNACentral', 'pirbase.fasta')],
         ['wrong', None],
     )
     @unpack
     def test_download_sequence(self, file_name, expect):
-        local_path, local_file = RNACentral(DIR_DATA, False).download_sequence(file_name)
+        local_path, local_file = RNACentral(DIR_DATA, True).download_sequence(file_name)
         assert local_path == os.path.join(DIR_DATA, 'RNACentral')
         assert local_file == expect
```

