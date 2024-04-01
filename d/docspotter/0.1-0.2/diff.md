# Comparing `tmp/docspotter-0.1.tar.gz` & `tmp/docspotter-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docspotter-0.1.tar", last modified: Mon Apr  1 11:43:21 2024, max compression
+gzip compressed data, was "docspotter-0.2.tar", last modified: Mon Apr  1 12:07:57 2024, max compression
```

## Comparing `docspotter-0.1.tar` & `docspotter-0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 11:43:21.918990 docspotter-0.1/
--rw-rw-rw-   0        0        0      685 2024-04-01 11:43:21.918990 docspotter-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-01 11:43:21.917976 docspotter-0.1/docspotter/
--rw-rw-rw-   0        0        0        0 2024-04-01 11:16:13.387370 docspotter-0.1/docspotter/__init__.py
--rw-rw-rw-   0        0        0     4951 2024-04-01 11:36:12.929276 docspotter-0.1/docspotter/docspotter.py
--rw-rw-rw-   0        0        0       40 2024-04-01 11:31:26.397884 docspotter-0.1/setup.cfg
--rw-rw-rw-   0        0        0      976 2024-04-01 11:30:50.980682 docspotter-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:07:57.031307 docspotter-0.2/
+-rw-rw-rw-   0        0        0      685 2024-04-01 12:07:57.031307 docspotter-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-01 12:07:57.030305 docspotter-0.2/docspotter/
+-rw-rw-rw-   0        0        0        0 2024-04-01 11:16:13.387370 docspotter-0.2/docspotter/__init__.py
+-rw-rw-rw-   0        0        0     4951 2024-04-01 11:36:12.929276 docspotter-0.2/docspotter/docspotter.py
+-rw-rw-rw-   0        0        0       40 2024-04-01 11:31:26.397884 docspotter-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-04-01 12:06:12.643128 docspotter-0.2/setup.py
```

### Comparing `docspotter-0.1/PKG-INFO` & `docspotter-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: docspotter
-Version: 0.1
+Version: 0.2
 Summary: DocSpotter is a Python library designed to extract specific information from document images by combining text detection and extraction technologies.
 Home-page: https://github.com/user/reponame
 Author: Nlaraki
 Author-email: larakinarjis@gmail.com
 License: MIT
 Download-URL: https://github.com/narjislaraki/docspotter
 Description: UNKNOWN
```

### Comparing `docspotter-0.1/docspotter/docspotter.py` & `docspotter-0.2/docspotter/docspotter.py`

 * *Files identical despite different names*

### Comparing `docspotter-0.1/setup.py` & `docspotter-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from distutils.core import setup
 setup(
   name = 'docspotter',        
   packages = ['docspotter'],  
-  version = '0.1',      
+  version = '0.2',      
   license='MIT',        
   description = 'DocSpotter is a Python library designed to extract specific information from document images by combining text detection and extraction technologies.',  
   author = 'Nlaraki',                   
   author_email = 'larakinarjis@gmail.com',     
   url = 'https://github.com/user/reponame',   
   download_url = 'https://github.com/narjislaraki/docspotter',   
   keywords = ['OCR', 'CRAFT', 'text', 'detection', 'extraction', 'easy'],   
   install_requires=[           
           'pytesseract',
-          'opencv',
+          'opencv-python',
           'craft-text-detector',
           'numpy',
       ],
   classifiers=[
     'Development Status :: 4 - Beta',     
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
```

