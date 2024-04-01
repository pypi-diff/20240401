# Comparing `tmp/amilib-0.0.1a1.tar.gz` & `tmp/amilib-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amilib-0.0.1a1.tar", last modified: Mon Apr  1 16:42:55 2024, max compression
+gzip compressed data, was "dist/amilib-0.0.1a2.tar", last modified: Mon Apr  1 17:02:24 2024, max compression
```

## Comparing `amilib-0.0.1a1.tar` & `amilib-0.0.1a2.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-01 16:42:55.793325 amilib-0.0.1a1/
--rw-r--r--   0 pm286      (503) staff       (20)    11357 2024-03-27 16:20:01.000000 amilib-0.0.1a1/LICENSE
--rw-r--r--   0 pm286      (503) staff       (20)      818 2024-04-01 16:42:55.793196 amilib-0.0.1a1/PKG-INFO
--rw-r--r--   0 pm286      (503) staff       (20)       76 2024-03-27 16:22:55.000000 amilib-0.0.1a1/README.md
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-01 16:42:55.788668 amilib-0.0.1a1/amilib/
--rw-r--r--   0 pm286      (503) staff       (20)        0 2024-03-27 18:27:17.000000 amilib-0.0.1a1/amilib/__init__.py
--rw-r--r--   0 pm286      (503) staff       (20)     5132 2024-04-01 09:44:34.000000 amilib-0.0.1a1/amilib/ami_bib.py
--rw-r--r--   0 pm286      (503) staff       (20)      285 2024-04-01 09:12:21.000000 amilib-0.0.1a1/amilib/ami_csv.py
--rw-r--r--   0 pm286      (503) staff       (20)   168207 2024-04-01 09:44:34.000000 amilib-0.0.1a1/amilib/ami_html.py
--rw-r--r--   0 pm286      (503) staff       (20)    16712 2024-04-01 09:44:34.000000 amilib-0.0.1a1/amilib/ami_integrate.py
--rw-r--r--   0 pm286      (503) staff       (20)     8293 2024-03-31 19:36:35.000000 amilib-0.0.1a1/amilib/ami_nlp.py
--rw-r--r--   0 pm286      (503) staff       (20)    27357 2024-04-01 09:44:34.000000 amilib-0.0.1a1/amilib/ami_pdf.py
--rw-r--r--   0 pm286      (503) staff       (20)    82090 2024-04-01 09:44:34.000000 amilib-0.0.1a1/amilib/ami_pdf_libs.py
--rw-r--r--   0 pm286      (503) staff       (20)     4978 2024-04-01 09:44:34.000000 amilib-0.0.1a1/amilib/ami_svg.py
--rw-r--r--   0 pm286      (503) staff       (20)    10651 2024-03-31 14:07:47.000000 amilib-0.0.1a1/amilib/ami_util.py
--rw-r--r--   0 pm286      (503) staff       (20)     8422 2024-03-31 17:50:56.000000 amilib-0.0.1a1/amilib/amidriver.py
--rw-r--r--   0 pm286      (503) staff       (20)    50146 2024-04-01 09:44:34.000000 amilib-0.0.1a1/amilib/amix.py
--rw-r--r--   0 pm286      (503) staff       (20)    19721 2024-04-01 09:44:34.000000 amilib-0.0.1a1/amilib/bbox.py
--rw-r--r--   0 pm286      (503) staff       (20)    14093 2024-03-28 20:25:22.000000 amilib-0.0.1a1/amilib/file_lib.py
--rw-r--r--   0 pm286      (503) staff       (20)    16712 2024-04-01 09:44:34.000000 amilib-0.0.1a1/amilib/html_generator.py
--rw-r--r--   0 pm286      (503) staff       (20)    48233 2024-04-01 09:44:34.000000 amilib-0.0.1a1/amilib/html_marker.py
--rw-r--r--   0 pm286      (503) staff       (20)    36840 2024-04-01 09:44:34.000000 amilib-0.0.1a1/amilib/util.py
--rw-r--r--   0 pm286      (503) staff       (20)    35077 2024-04-01 09:44:34.000000 amilib-0.0.1a1/amilib/wikimedia.py
--rw-r--r--   0 pm286      (503) staff       (20)    54688 2024-04-01 09:44:34.000000 amilib-0.0.1a1/amilib/xml_lib.py
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-01 16:42:55.789710 amilib-0.0.1a1/amilib.egg-info/
--rw-r--r--   0 pm286      (503) staff       (20)      818 2024-04-01 16:42:55.000000 amilib-0.0.1a1/amilib.egg-info/PKG-INFO
--rw-r--r--   0 pm286      (503) staff       (20)      798 2024-04-01 16:42:55.000000 amilib-0.0.1a1/amilib.egg-info/SOURCES.txt
--rw-r--r--   0 pm286      (503) staff       (20)        1 2024-04-01 16:42:55.000000 amilib-0.0.1a1/amilib.egg-info/dependency_links.txt
--rw-r--r--   0 pm286      (503) staff       (20)       44 2024-04-01 16:42:55.000000 amilib-0.0.1a1/amilib.egg-info/entry_points.txt
--rw-r--r--   0 pm286      (503) staff       (20)        1 2024-04-01 16:42:55.000000 amilib-0.0.1a1/amilib.egg-info/not-zip-safe
--rw-r--r--   0 pm286      (503) staff       (20)      111 2024-04-01 16:42:55.000000 amilib-0.0.1a1/amilib.egg-info/requires.txt
--rw-r--r--   0 pm286      (503) staff       (20)        7 2024-04-01 16:42:55.000000 amilib-0.0.1a1/amilib.egg-info/top_level.txt
--rw-r--r--   0 pm286      (503) staff       (20)      596 2024-04-01 15:55:47.000000 amilib-0.0.1a1/pyproject.toml
--rw-r--r--   0 pm286      (503) staff       (20)       38 2024-04-01 16:42:55.793372 amilib-0.0.1a1/setup.cfg
--rw-r--r--   0 pm286      (503) staff       (20)     1627 2024-04-01 16:42:36.000000 amilib-0.0.1a1/setup.py
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-01 16:42:55.792904 amilib-0.0.1a1/test/
--rw-r--r--   0 pm286      (503) staff       (20)     7614 2024-04-01 09:44:34.000000 amilib-0.0.1a1/test/test_all.py
--rw-r--r--   0 pm286      (503) staff       (20)     5098 2024-04-01 09:44:34.000000 amilib-0.0.1a1/test/test_file.py
--rw-r--r--   0 pm286      (503) staff       (20)    38379 2024-04-01 09:44:34.000000 amilib-0.0.1a1/test/test_headless.py
--rw-r--r--   0 pm286      (503) staff       (20)   121224 2024-04-01 09:44:34.000000 amilib-0.0.1a1/test/test_html.py
--rw-r--r--   0 pm286      (503) staff       (20)     1133 2024-04-01 09:44:34.000000 amilib-0.0.1a1/test/test_nlp.py
--rw-r--r--   0 pm286      (503) staff       (20)    80006 2024-04-01 09:44:34.000000 amilib-0.0.1a1/test/test_pdf.py
--rw-r--r--   0 pm286      (503) staff       (20)     1065 2024-04-01 09:44:34.000000 amilib-0.0.1a1/test/test_svg.py
--rw-r--r--   0 pm286      (503) staff       (20)    10141 2024-04-01 09:44:34.000000 amilib-0.0.1a1/test/test_util.py
--rw-r--r--   0 pm286      (503) staff       (20)    35925 2024-04-01 09:44:34.000000 amilib-0.0.1a1/test/test_wikidata.py
--rw-r--r--   0 pm286      (503) staff       (20)     1973 2024-04-01 09:44:34.000000 amilib-0.0.1a1/test/test_xml.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-01 17:02:24.385952 amilib-0.0.1a2/
+-rw-r--r--   0 pm286      (503) staff       (20)    11357 2024-03-27 16:20:01.000000 amilib-0.0.1a2/LICENSE
+-rw-r--r--   0 pm286      (503) staff       (20)      818 2024-04-01 17:02:24.385826 amilib-0.0.1a2/PKG-INFO
+-rw-r--r--   0 pm286      (503) staff       (20)       76 2024-03-27 16:22:55.000000 amilib-0.0.1a2/README.md
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-01 17:02:24.383329 amilib-0.0.1a2/amilib/
+-rw-r--r--   0 pm286      (503) staff       (20)        0 2024-03-27 18:27:17.000000 amilib-0.0.1a2/amilib/__init__.py
+-rw-r--r--   0 pm286      (503) staff       (20)     5132 2024-04-01 09:44:34.000000 amilib-0.0.1a2/amilib/ami_bib.py
+-rw-r--r--   0 pm286      (503) staff       (20)      285 2024-04-01 09:12:21.000000 amilib-0.0.1a2/amilib/ami_csv.py
+-rw-r--r--   0 pm286      (503) staff       (20)   168207 2024-04-01 09:44:34.000000 amilib-0.0.1a2/amilib/ami_html.py
+-rw-r--r--   0 pm286      (503) staff       (20)    16712 2024-04-01 09:44:34.000000 amilib-0.0.1a2/amilib/ami_integrate.py
+-rw-r--r--   0 pm286      (503) staff       (20)     8293 2024-03-31 19:36:35.000000 amilib-0.0.1a2/amilib/ami_nlp.py
+-rw-r--r--   0 pm286      (503) staff       (20)    27357 2024-04-01 09:44:34.000000 amilib-0.0.1a2/amilib/ami_pdf.py
+-rw-r--r--   0 pm286      (503) staff       (20)    82090 2024-04-01 09:44:34.000000 amilib-0.0.1a2/amilib/ami_pdf_libs.py
+-rw-r--r--   0 pm286      (503) staff       (20)     4978 2024-04-01 09:44:34.000000 amilib-0.0.1a2/amilib/ami_svg.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10651 2024-03-31 14:07:47.000000 amilib-0.0.1a2/amilib/ami_util.py
+-rw-r--r--   0 pm286      (503) staff       (20)     8422 2024-03-31 17:50:56.000000 amilib-0.0.1a2/amilib/amidriver.py
+-rw-r--r--   0 pm286      (503) staff       (20)    50146 2024-04-01 09:44:34.000000 amilib-0.0.1a2/amilib/amix.py
+-rw-r--r--   0 pm286      (503) staff       (20)    19721 2024-04-01 09:44:34.000000 amilib-0.0.1a2/amilib/bbox.py
+-rw-r--r--   0 pm286      (503) staff       (20)    14093 2024-03-28 20:25:22.000000 amilib-0.0.1a2/amilib/file_lib.py
+-rw-r--r--   0 pm286      (503) staff       (20)    16712 2024-04-01 09:44:34.000000 amilib-0.0.1a2/amilib/html_generator.py
+-rw-r--r--   0 pm286      (503) staff       (20)    48233 2024-04-01 09:44:34.000000 amilib-0.0.1a2/amilib/html_marker.py
+-rw-r--r--   0 pm286      (503) staff       (20)    36840 2024-04-01 09:44:34.000000 amilib-0.0.1a2/amilib/util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    35077 2024-04-01 09:44:34.000000 amilib-0.0.1a2/amilib/wikimedia.py
+-rw-r--r--   0 pm286      (503) staff       (20)    54688 2024-04-01 09:44:34.000000 amilib-0.0.1a2/amilib/xml_lib.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-01 17:02:24.384282 amilib-0.0.1a2/amilib.egg-info/
+-rw-r--r--   0 pm286      (503) staff       (20)      818 2024-04-01 17:02:23.000000 amilib-0.0.1a2/amilib.egg-info/PKG-INFO
+-rw-r--r--   0 pm286      (503) staff       (20)      783 2024-04-01 17:02:24.000000 amilib-0.0.1a2/amilib.egg-info/SOURCES.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2024-04-01 17:02:24.000000 amilib-0.0.1a2/amilib.egg-info/dependency_links.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       44 2024-04-01 17:02:24.000000 amilib-0.0.1a2/amilib.egg-info/entry_points.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2024-04-01 16:42:55.000000 amilib-0.0.1a2/amilib.egg-info/not-zip-safe
+-rw-r--r--   0 pm286      (503) staff       (20)      111 2024-04-01 17:02:24.000000 amilib-0.0.1a2/amilib.egg-info/requires.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        7 2024-04-01 17:02:24.000000 amilib-0.0.1a2/amilib.egg-info/top_level.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       38 2024-04-01 17:02:24.386011 amilib-0.0.1a2/setup.cfg
+-rw-r--r--   0 pm286      (503) staff       (20)     1627 2024-04-01 17:02:19.000000 amilib-0.0.1a2/setup.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-01 17:02:24.385671 amilib-0.0.1a2/test/
+-rw-r--r--   0 pm286      (503) staff       (20)     7614 2024-04-01 09:44:34.000000 amilib-0.0.1a2/test/test_all.py
+-rw-r--r--   0 pm286      (503) staff       (20)     5098 2024-04-01 09:44:34.000000 amilib-0.0.1a2/test/test_file.py
+-rw-r--r--   0 pm286      (503) staff       (20)    38379 2024-04-01 09:44:34.000000 amilib-0.0.1a2/test/test_headless.py
+-rw-r--r--   0 pm286      (503) staff       (20)   121224 2024-04-01 09:44:34.000000 amilib-0.0.1a2/test/test_html.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1133 2024-04-01 09:44:34.000000 amilib-0.0.1a2/test/test_nlp.py
+-rw-r--r--   0 pm286      (503) staff       (20)    80006 2024-04-01 09:44:34.000000 amilib-0.0.1a2/test/test_pdf.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1065 2024-04-01 09:44:34.000000 amilib-0.0.1a2/test/test_svg.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10141 2024-04-01 09:44:34.000000 amilib-0.0.1a2/test/test_util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    35925 2024-04-01 09:44:34.000000 amilib-0.0.1a2/test/test_wikidata.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1973 2024-04-01 09:44:34.000000 amilib-0.0.1a2/test/test_xml.py
```

### Comparing `amilib-0.0.1a1/LICENSE` & `amilib-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/PKG-INFO` & `amilib-0.0.1a2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amilib
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: document download, cleaning, managemenr
 Home-page: https://github.com/petermr/amilib
 Author: Peter Murray-Rust
 Author-email: petermurrayrust@googlemail.com
 License: Apache2
 Keywords: text and data mining
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `amilib-0.0.1a1/amilib/ami_bib.py` & `amilib-0.0.1a2/amilib/ami_bib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/amilib/ami_html.py` & `amilib-0.0.1a2/amilib/ami_html.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/amilib/ami_integrate.py` & `amilib-0.0.1a2/amilib/ami_integrate.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/amilib/ami_nlp.py` & `amilib-0.0.1a2/amilib/ami_nlp.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/amilib/ami_pdf.py` & `amilib-0.0.1a2/amilib/ami_pdf.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/amilib/ami_pdf_libs.py` & `amilib-0.0.1a2/amilib/ami_pdf_libs.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/amilib/ami_svg.py` & `amilib-0.0.1a2/amilib/ami_svg.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/amilib/ami_util.py` & `amilib-0.0.1a2/amilib/ami_util.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/amilib/amidriver.py` & `amilib-0.0.1a2/amilib/amidriver.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/amilib/amix.py` & `amilib-0.0.1a2/amilib/amix.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/amilib/bbox.py` & `amilib-0.0.1a2/amilib/bbox.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/amilib/file_lib.py` & `amilib-0.0.1a2/amilib/file_lib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/amilib/html_generator.py` & `amilib-0.0.1a2/amilib/html_generator.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/amilib/html_marker.py` & `amilib-0.0.1a2/amilib/html_marker.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/amilib/util.py` & `amilib-0.0.1a2/amilib/util.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/amilib/wikimedia.py` & `amilib-0.0.1a2/amilib/wikimedia.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/amilib/xml_lib.py` & `amilib-0.0.1a2/amilib/xml_lib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/amilib.egg-info/PKG-INFO` & `amilib-0.0.1a2/amilib.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amilib
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: document download, cleaning, managemenr
 Home-page: https://github.com/petermr/amilib
 Author: Peter Murray-Rust
 Author-email: petermurrayrust@googlemail.com
 License: Apache2
 Keywords: text and data mining
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `amilib-0.0.1a1/amilib.egg-info/SOURCES.txt` & `amilib-0.0.1a2/amilib.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE
 README.md
-pyproject.toml
 setup.py
 amilib/__init__.py
 amilib/ami_bib.py
 amilib/ami_csv.py
 amilib/ami_html.py
 amilib/ami_integrate.py
 amilib/ami_nlp.py
```

### Comparing `amilib-0.0.1a1/setup.py` & `amilib-0.0.1a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'scikit-learn',
 
 ]
 
 setup(
     name='amilib',
     url='https://github.com/petermr/amilib',
-    version='0.0.1a1',
+    version='0.0.1a2',
     description='document download, cleaning, managemenr',
     long_description_content_type='text/markdown',
     long_description=readme,
     author="Peter Murray-Rust",
     author_email='petermurrayrust@googlemail.com',
     license='Apache2',
     install_requires=requirements,
```

### Comparing `amilib-0.0.1a1/test/test_all.py` & `amilib-0.0.1a2/test/test_all.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/test/test_file.py` & `amilib-0.0.1a2/test/test_file.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/test/test_headless.py` & `amilib-0.0.1a2/test/test_headless.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/test/test_html.py` & `amilib-0.0.1a2/test/test_html.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/test/test_nlp.py` & `amilib-0.0.1a2/test/test_nlp.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/test/test_pdf.py` & `amilib-0.0.1a2/test/test_pdf.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/test/test_svg.py` & `amilib-0.0.1a2/test/test_svg.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/test/test_util.py` & `amilib-0.0.1a2/test/test_util.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/test/test_wikidata.py` & `amilib-0.0.1a2/test/test_wikidata.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a1/test/test_xml.py` & `amilib-0.0.1a2/test/test_xml.py`

 * *Files identical despite different names*

