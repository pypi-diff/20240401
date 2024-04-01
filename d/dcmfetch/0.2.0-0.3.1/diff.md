# Comparing `tmp/dcmfetch-0.2.0.tar.gz` & `tmp/dcmfetch-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dcmfetch-0.2.0.tar", last modified: Wed Jun 10 15:10:12 2020, max compression
+gzip compressed data, was "dcmfetch-0.3.1.tar", last modified: Mon Apr  1 15:50:02 2024, max compression
```

## Comparing `dcmfetch-0.2.0.tar` & `dcmfetch-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,41 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-10 15:10:12.000000 dcmfetch-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     3012 2020-06-10 15:10:12.000000 dcmfetch-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1917 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-10 15:10:11.000000 dcmfetch-0.2.0/dcmfetch/
--rw-rw-rw-   0 root         (0) root         (0)      195 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4340 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/aettable.py
--rw-rw-rw-   0 root         (0) root         (0)    14744 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/dcmfetch.py
--rwxrwxrwx   0 root         (0) root         (0)     6182 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/dcmfetchtool.py
--rw-rw-rw-   0 root         (0) root         (0)    16054 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/dicomweb.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-10 15:10:12.000000 dcmfetch-0.2.0/dcmfetch/ext/
--rw-rw-rw-   0 root         (0) root         (0)     1002 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/ext/dcmnodes.cf
--rwxrwxrwx   0 root         (0) root         (0)  1170649 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/ext/findscu
--rwxrwxrwx   0 root         (0) root         (0)  1200138 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/ext/findscu.exe
--rwxrwxrwx   0 root         (0) root         (0)  1173715 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/ext/getscu
--rwxrwxrwx   0 root         (0) root         (0)  1203204 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/ext/getscu.exe
--rw-rw-rw-   0 root         (0) root         (0)     8423 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/ext/store-tcs.properties
--rw-rw-rw-   0 root         (0) root         (0)    31175 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/fetchdialog.py
--rw-rw-rw-   0 root         (0) root         (0)    19807 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/qidcm4che3.py
--rw-rw-rw-   0 root         (0) root         (0)     1549 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/qimock.py
--rw-rw-rw-   0 root         (0) root         (0)    16461 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/qipynetdicom.py
--rw-rw-rw-   0 root         (0) root         (0)    11293 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/queryinterface.py
--rw-rw-rw-   0 root         (0) root         (0)     1573 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/structures.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/dcmfetch/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-10 15:10:11.000000 dcmfetch-0.2.0/dcmfetch.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     3012 2020-06-10 15:10:11.000000 dcmfetch-0.2.0/dcmfetch.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      641 2020-06-10 15:10:11.000000 dcmfetch-0.2.0/dcmfetch.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2020-06-10 15:10:11.000000 dcmfetch-0.2.0/dcmfetch.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      110 2020-06-10 15:10:11.000000 dcmfetch-0.2.0/dcmfetch.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2020-06-10 15:10:11.000000 dcmfetch-0.2.0/dcmfetch.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2020-06-10 15:10:11.000000 dcmfetch-0.2.0/dcmfetch.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      108 2020-06-10 15:10:12.000000 dcmfetch-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2006 2020-06-10 15:09:44.000000 dcmfetch-0.2.0/setup.py
+drwxr-xr-x   0 ron        (501) staff       (20)        0 2024-04-01 15:50:02.937762 dcmfetch-0.3.1/
+-rw-r--r--   0 ron        (501) staff       (20)     1062 2024-04-01 12:17:14.000000 dcmfetch-0.3.1/LICENCE
+-rw-r--r--   0 ron        (501) staff       (20)     3024 2024-04-01 15:50:02.936111 dcmfetch-0.3.1/PKG-INFO
+-rw-r--r--   0 ron        (501) staff       (20)     1911 2024-04-01 13:52:00.000000 dcmfetch-0.3.1/README.md
+drwxr-xr-x   0 ron        (501) staff       (20)        0 2024-04-01 15:50:02.545589 dcmfetch-0.3.1/dcmfetch/
+-rw-r--r--   0 ron        (501) staff       (20)      195 2024-04-01 14:59:03.000000 dcmfetch-0.3.1/dcmfetch/__init__.py
+-rw-r--r--   0 ron        (501) staff       (20)     4274 2024-04-01 12:17:14.000000 dcmfetch-0.3.1/dcmfetch/aettable.py
+-rw-r--r--   0 ron        (501) staff       (20)    14683 2024-04-01 15:08:52.000000 dcmfetch-0.3.1/dcmfetch/dcmfetch.py
+-rwxr-xr-x   0 ron        (501) staff       (20)     6162 2024-04-01 15:08:52.000000 dcmfetch-0.3.1/dcmfetch/dcmfetchtool.py
+-rw-r--r--   0 ron        (501) staff       (20)    15647 2024-04-01 15:08:52.000000 dcmfetch-0.3.1/dcmfetch/dicomweb.py
+drwxr-xr-x   0 ron        (501) staff       (20)        0 2024-04-01 15:50:02.751330 dcmfetch-0.3.1/dcmfetch/ext/
+-rw-r--r--   0 ron        (501) staff       (20)     1002 2024-04-01 12:17:14.000000 dcmfetch-0.3.1/dcmfetch/ext/dcmnodes.cf
+-rwxr-xr-x   0 ron        (501) staff       (20)  1170649 2024-04-01 12:17:14.000000 dcmfetch-0.3.1/dcmfetch/ext/findscu
+-rwxr-xr-x   0 ron        (501) staff       (20)  1200138 2024-04-01 12:17:14.000000 dcmfetch-0.3.1/dcmfetch/ext/findscu.exe
+-rwxr-xr-x   0 ron        (501) staff       (20)  1173715 2024-04-01 12:17:14.000000 dcmfetch-0.3.1/dcmfetch/ext/getscu
+-rwxr-xr-x   0 ron        (501) staff       (20)  1203204 2024-04-01 12:17:14.000000 dcmfetch-0.3.1/dcmfetch/ext/getscu.exe
+-rw-r--r--   0 ron        (501) staff       (20)     8423 2024-04-01 12:17:14.000000 dcmfetch-0.3.1/dcmfetch/ext/store-tcs.properties
+-rw-r--r--   0 ron        (501) staff       (20)    31110 2024-04-01 15:08:52.000000 dcmfetch-0.3.1/dcmfetch/fetchdialog.py
+-rw-r--r--   0 ron        (501) staff       (20)    19742 2024-04-01 15:08:52.000000 dcmfetch-0.3.1/dcmfetch/qidcm4che3.py
+-rw-r--r--   0 ron        (501) staff       (20)     1483 2024-04-01 15:08:52.000000 dcmfetch-0.3.1/dcmfetch/qimock.py
+-rw-r--r--   0 ron        (501) staff       (20)    16687 2024-04-01 15:08:52.000000 dcmfetch-0.3.1/dcmfetch/qipynetdicom.py
+-rw-r--r--   0 ron        (501) staff       (20)    11227 2024-04-01 15:08:52.000000 dcmfetch-0.3.1/dcmfetch/queryinterface.py
+-rw-r--r--   0 ron        (501) staff       (20)     1506 2024-04-01 15:08:52.000000 dcmfetch-0.3.1/dcmfetch/structures.py
+-rw-r--r--   0 ron        (501) staff       (20)       22 2024-04-01 15:12:53.000000 dcmfetch-0.3.1/dcmfetch/version.py
+drwxr-xr-x   0 ron        (501) staff       (20)        0 2024-04-01 15:50:02.926544 dcmfetch-0.3.1/dcmfetch.egg-info/
+-rw-r--r--   0 ron        (501) staff       (20)     3024 2024-04-01 15:50:01.000000 dcmfetch-0.3.1/dcmfetch.egg-info/PKG-INFO
+-rw-r--r--   0 ron        (501) staff       (20)      824 2024-04-01 15:50:01.000000 dcmfetch-0.3.1/dcmfetch.egg-info/SOURCES.txt
+-rw-r--r--   0 ron        (501) staff       (20)        1 2024-04-01 15:50:01.000000 dcmfetch-0.3.1/dcmfetch.egg-info/dependency_links.txt
+-rw-r--r--   0 ron        (501) staff       (20)      109 2024-04-01 15:50:01.000000 dcmfetch-0.3.1/dcmfetch.egg-info/entry_points.txt
+-rw-r--r--   0 ron        (501) staff       (20)       75 2024-04-01 15:50:01.000000 dcmfetch-0.3.1/dcmfetch.egg-info/requires.txt
+-rw-r--r--   0 ron        (501) staff       (20)        9 2024-04-01 15:50:01.000000 dcmfetch-0.3.1/dcmfetch.egg-info/top_level.txt
+-rw-r--r--   0 ron        (501) staff       (20)      108 2024-04-01 15:50:02.939567 dcmfetch-0.3.1/setup.cfg
+-rw-r--r--   0 ron        (501) staff       (20)     1958 2024-04-01 15:09:41.000000 dcmfetch-0.3.1/setup.py
+drwxr-xr-x   0 ron        (501) staff       (20)        0 2024-04-01 15:50:02.795061 dcmfetch-0.3.1/tests/
+-rw-r--r--   0 ron        (501) staff       (20)     2548 2024-04-01 12:17:14.000000 dcmfetch-0.3.1/tests/test_aettable.py
+-rw-r--r--   0 ron        (501) staff       (20)     5068 2024-04-01 12:17:14.000000 dcmfetch-0.3.1/tests/test_dcmfetch.py
+-rw-r--r--   0 ron        (501) staff       (20)    14287 2024-04-01 13:30:22.000000 dcmfetch-0.3.1/tests/test_dicomweb.py
+-rw-r--r--   0 ron        (501) staff       (20)     3471 2024-04-01 13:31:28.000000 dcmfetch-0.3.1/tests/test_qidcm4che3.py
+-rw-r--r--   0 ron        (501) staff       (20)     3647 2024-04-01 13:25:24.000000 dcmfetch-0.3.1/tests/test_qipynetdicom.py
+-rw-r--r--   0 ron        (501) staff       (20)     3484 2024-04-01 13:32:29.000000 dcmfetch-0.3.1/tests/test_queryinterface.py
+-rw-r--r--   0 ron        (501) staff       (20)     1539 2024-04-01 12:17:14.000000 dcmfetch-0.3.1/tests/test_structures.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dcmfetch-0.2.0/PKG-INFO` & `dcmfetch-0.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 Metadata-Version: 2.1
 Name: dcmfetch
-Version: 0.2.0
+Version: 0.3.1
 Summary: DICOM query retrieve tools
 Home-page: https://bitbucket.org/rtrhd/dcmfetch
+Download-URL: https://bitbucket.org/rtrhd/dcmfetch/get/v0.3.1.zip
 Author: Ron Hartley-Davies
 Author-email: R.Hartley-Davies@bristol.ac.uk
 License: MIT
-Download-URL: https://bitbucket.org/rtrhd/dcmfetch/get/v0.2.0.zip
-Description: # DICOM Server Access
-        
-        Dcmfetch is a python package for retrieving images from a [DICOM](http://medical.nema.org/) server. The package does not provide a DICOm trnasport itself but wraps either the command line utilies from  [dcm4che3](https://sourceforge.net/projects/dcm4che/files/dcm4che3/) or the native python library[pynetdicom](https://github.com/pydicom/pynetdicom). In addition, bundled standalone versions of the required dcm4che3 tools are included so the only mandatory external (non-python) dependency for the dcm4che3 option is a working java runtime. Further details on installation and use are available [here](docs/dcmfetch.md).
-        
-        The DICOM server must support the dicom `c-find` and `c-get` protocols (not just `c-move`).
-        This is the case for the
-        [dcm4chee](https://sourceforge.net/projects/dcm4che/files/dcm4chee/) server, though several other common servers do not as yet support `c-get`. In addition though, `dcmfetch` supports access to servers such as [orthanc](http://www.orthanc-server.com/) using the `QIDO-RS` and `WADO-RS` web *REST* APIs instead.
-        
-        DICOM servers are identified by keys in the configuration file `dcmnodes.cf`. This file encodes the server details (AET, most, port) together with a string representing facilities supported by the server (including the web API if available). This file is typically installed to the directory `/etc` on a unix system.
-        
-        As well as the python package `dcmfetch` two utilities are provided: `dcmfetch` a command line program to retrieve series and `dcmfetchtool` a [PyQt](https://riverbankcomputing.com/software/pyqt/intro) based graphical tool.
-        
-        ## Licences
-        
-        This package is made available under the [MIT](LICENCE) licence. The included dcm4che3 programs are distributed under the [Mozilla](https://github.com/dcm4che/dcm4che/blob/master/LICENSE.txt) public licence; the only modification here has been to bundle them into single executables.
-         
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
-Provides-Extra: PyNetDicom
+License-File: LICENCE
+Requires-Dist: requests>=2.2.1
+Requires-Dist: QtPy>=1.0.2
+Requires-Dist: pydicom>=1.2.1
+Provides-Extra: pynetdicom
+Requires-Dist: pynetdicom>=1.5.1; extra == "pynetdicom"
+
+# DICOM Server Access
+
+Dcmfetch is a python package for retrieving images from a [DICOM](http://medical.nema.org/) server. The package does not provide a DICOM transport itself but wraps either the command line utilies from  [dcm4che3](https://sourceforge.net/projects/dcm4che/files/dcm4che3/) or the native python library [pynetdicom](https://github.com/pydicom/pynetdicom). In addition, bundled standalone versions of the required dcm4che3 tools are included so the only mandatory external (non-python) dependency for the dcm4che3 option is a working java runtime. Further details on installation and use are available [here](docs/dcmfetch.md).
+
+The DICOM server must support the dicom `c-find` and `c-get` protocols (not just `c-move`).
+This is the case for the
+[dcm4chee](https://sourceforge.net/projects/dcm4che/files/dcm4chee/) server, though several other common servers do not as yet support `c-get`. In addition, `dcmfetch` supports access to servers such as [orthanc](http://www.orthanc-server.com/) using the `QIDO-RS` and `WADO-RS` web *REST* APIs instead.
+
+DICOM servers are identified by keys in the configuration file `dcmnodes.cf`. This file encodes the server details (AET, host, port) together with a string representing facilities supported by the server (including the web API if available). This file is typically installed to the directory `/etc` on a unix system.
+
+As well as the python package `dcmfetch`, two utilities are provided: `dcmfetch` a command line program to retrieve series and `dcmfetchtool` a [PyQt](https://riverbankcomputing.com/software/pyqt/intro) based graphical tool.
+
+## Licences
+
+This package is made available under the [MIT](LICENCE) licence. The included dcm4che3 programs are distributed under the [Mozilla](https://github.com/dcm4che/dcm4che/blob/master/LICENSE.txt) public licence; the only modification here has been to bundle them into single executables.
```

### Comparing `dcmfetch-0.2.0/README.md` & `dcmfetch-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # DICOM Server Access
 
-Dcmfetch is a python package for retrieving images from a [DICOM](http://medical.nema.org/) server. The package does not provide a DICOm trnasport itself but wraps either the command line utilies from  [dcm4che3](https://sourceforge.net/projects/dcm4che/files/dcm4che3/) or the native python library[pynetdicom](https://github.com/pydicom/pynetdicom). In addition, bundled standalone versions of the required dcm4che3 tools are included so the only mandatory external (non-python) dependency for the dcm4che3 option is a working java runtime. Further details on installation and use are available [here](docs/dcmfetch.md).
+Dcmfetch is a python package for retrieving images from a [DICOM](http://medical.nema.org/) server. The package does not provide a DICOM transport itself but wraps either the command line utilies from  [dcm4che3](https://sourceforge.net/projects/dcm4che/files/dcm4che3/) or the native python library [pynetdicom](https://github.com/pydicom/pynetdicom). In addition, bundled standalone versions of the required dcm4che3 tools are included so the only mandatory external (non-python) dependency for the dcm4che3 option is a working java runtime. Further details on installation and use are available [here](docs/dcmfetch.md).
 
 The DICOM server must support the dicom `c-find` and `c-get` protocols (not just `c-move`).
 This is the case for the
-[dcm4chee](https://sourceforge.net/projects/dcm4che/files/dcm4chee/) server, though several other common servers do not as yet support `c-get`. In addition though, `dcmfetch` supports access to servers such as [orthanc](http://www.orthanc-server.com/) using the `QIDO-RS` and `WADO-RS` web *REST* APIs instead.
+[dcm4chee](https://sourceforge.net/projects/dcm4che/files/dcm4chee/) server, though several other common servers do not as yet support `c-get`. In addition, `dcmfetch` supports access to servers such as [orthanc](http://www.orthanc-server.com/) using the `QIDO-RS` and `WADO-RS` web *REST* APIs instead.
 
-DICOM servers are identified by keys in the configuration file `dcmnodes.cf`. This file encodes the server details (AET, most, port) together with a string representing facilities supported by the server (including the web API if available). This file is typically installed to the directory `/etc` on a unix system.
+DICOM servers are identified by keys in the configuration file `dcmnodes.cf`. This file encodes the server details (AET, host, port) together with a string representing facilities supported by the server (including the web API if available). This file is typically installed to the directory `/etc` on a unix system.
 
-As well as the python package `dcmfetch` two utilities are provided: `dcmfetch` a command line program to retrieve series and `dcmfetchtool` a [PyQt](https://riverbankcomputing.com/software/pyqt/intro) based graphical tool.
+As well as the python package `dcmfetch`, two utilities are provided: `dcmfetch` a command line program to retrieve series and `dcmfetchtool` a [PyQt](https://riverbankcomputing.com/software/pyqt/intro) based graphical tool.
 
 ## Licences
 
 This package is made available under the [MIT](LICENCE) licence. The included dcm4che3 programs are distributed under the [Mozilla](https://github.com/dcm4che/dcm4che/blob/master/LICENSE.txt) public licence; the only modification here has been to bundle them into single executables.
-
```

### Comparing `dcmfetch-0.2.0/dcmfetch/aettable.py` & `dcmfetch-0.3.1/dcmfetch/aettable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 DICOM node table support.
 
 Provides look up of DICOM server details read fromn a dcmnoeds.cf configuration file.
 """
 
-from __future__ import print_function, division, absolute_import
-
 from collections import OrderedDict, namedtuple
 
 from os.path import join, expanduser, exists
 import os
 import re
 import pkg_resources
```

### Comparing `dcmfetch-0.2.0/dcmfetch/dcmfetch.py` & `dcmfetch-0.3.1/dcmfetch/dcmfetch.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 """Top level api for dcmfetch package.
 
 Provides high level routines for downloading DICOM series
 and a command line program "dcmfetch"
 """
 
-from __future__ import print_function, division, absolute_import
-
 from os.path import join, isdir, normpath, abspath, isfile, exists
 from os import mkdir, access, W_OK, X_OK
 from shutil import rmtree, move
 from tempfile import mkdtemp
 from zipfile import ZipFile, is_zipfile, ZIP_STORED
 from io import BytesIO
 from fnmatch import fnmatchcase
@@ -25,24 +23,15 @@
 
 from . queryinterface import QueryInterface
 from . aettable import AetTable
 from . version import __version__
 
 __all__ = ['fetch_series', 'fetch_series_to_disk', 'read_series']
 
-# PY3K
-try:
-    basestring # py2
-except NameError:
-    basestring = str
-
-try:
-    from collections.abc import Sequence, Callable # py3
-except ImportError:
-    from collections import Sequence, Callable
+from collections.abc import Sequence, Callable
 
 
 def _filter_by_date(dobjs, studydate='all'):
     """Filter on ISO date.
 
     Used to handle StudyID ambiguity.
     Selects closest study to specified (ISO) date if multiple dates present.
@@ -118,15 +107,15 @@
     """
     qi = QueryInterface(aettable=aettable, localaet=localaet)
     if server is None:
         # first entry in table by default
         server = next(iter(qi.aettable))
 
     # Fix up for strings and single objects
-    if isinstance(sernos, basestring) or not isinstance(sernos, Sequence):
+    if isinstance(sernos, str) or not isinstance(sernos, Sequence):
         sernos = [sernos]
     sernos = list(map(int, sernos))
 
     # Remove duplicates
     sernos = list(set(sernos))
 
     seriess = [
@@ -151,16 +140,19 @@
     # TODO: if many studies may need to filter early w/o holding all in memory
     dobjs = _filter_by_date(dobjs, studydate=studydate)
 
     # Remove non-image objects.
     # Useful for Philips, which includes PresentationState objects among images
     if imagesonly:
         dobjs = [dobj for dobj in dobjs if 'PixelData' in dobj]
+
+    # Sort by series and instance. Since any retained non-image objects
+    # may lack series or image numbers we sort all these to the end of the list.
     return sorted(
-        dobjs, key=lambda d: (int(d.SeriesNumber), int(d.InstanceNumber))
+        dobjs, key=lambda d: (int(getattr(d, 'SeriesNumber', 1e6)), int(getattr(d, 'InstanceNumber', 1e6)))
     )
 
 
 def read_series(fileordirname, key=None, numeric=False,
                 reverse=False, globspec='*.dcm'):
     """
     Read a DICOM series from a directory or a zip file of DICOM files.
@@ -184,20 +176,20 @@
 
     Returns
     -------
     out:
         List of dicom objects.
 
     """
-    if not isinstance(fileordirname, basestring):
+    if not isinstance(fileordirname, str):
         # Assume a sequence is just a list of simple filenames
         dobjs = [dcmread(fname) for fname in sorted(set(fileordirname))]
     elif isdir(fileordirname):
         # A directory name
-        if isinstance(globspec, basestring):
+        if isinstance(globspec, str):
             # General case is a list of globspecs
             globspec = [globspec]
         # NB: set comprehension takes account of duplicate matches
         # for multiple glob patterns
         files = sorted({
             f for glb in globspec for f in glob(join(fileordirname, glb))
         })
@@ -274,15 +266,15 @@
     """
     qi = QueryInterface()
     if server is None:
         # first entry in table by default
         server = next(iter(qi.aettable))
 
     # Fix up for strings and single objects
-    if isinstance(sernos, basestring) or not isinstance(sernos, Sequence):
+    if isinstance(sernos, str) or not isinstance(sernos, Sequence):
         sernos = [sernos]
     sernos = list(map(int, sernos))
 
     # Remove duplicates
     sernos = list(set(sernos))
 
     # Filter for the specified study ids and series numbers
```

### Comparing `dcmfetch-0.2.0/dcmfetch/dcmfetchtool.py` & `dcmfetch-0.3.1/dcmfetch/dcmfetchtool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """A DICOM server browser and fetch tool dialog."""
 
-from __future__ import print_function, division, absolute_import
 import sys
 from os.path import join, dirname
 from os import getenv
 from zipfile import ZipFile, ZIP_STORED
 from itertools import takewhile
 
 # user interface
 from qtpy.QtWidgets import (
     QPushButton, QDialog, QMessageBox,
-    QApplication, QGridLayout,
+    QApplication, QGridLayout
 )
 from qtpy.QtCore import QTimer
 from qtpy.compat import getsavefilename
 
 from . fetchdialog import FetchDialog
 from . version import __version__
 
@@ -30,17 +29,15 @@
 
 
 class TopLevel(QDialog):
 
     def __init__(self, aetfile=None, savedir=None, multiple=False, parent=None):
         super(TopLevel, self).__init__(parent)
         self._fetchBtn = QPushButton("Fetch")
-
         self._saveBtn = QPushButton("Save")
-
         self._quitBtn = QPushButton("Quit")
 
         self._fetchBtn.clicked.connect(self.fetch)
         self._saveBtn.clicked.connect(self.save)
         self._quitBtn.clicked.connect(self.reject)
 
         self._fetchBtn.setEnabled(True)
@@ -50,15 +47,15 @@
         grid = QGridLayout()
         grid.addWidget(self._fetchBtn, 0, 0)
         grid.addWidget(self._saveBtn, 0, 1)
         grid.addWidget(self._quitBtn, 0, 2)
         self.setLayout(grid)
         self._fetchDlg = FetchDialog(parent=self, aetfile=aetfile, multiple_selection=multiple)
         self._suggestedFile = ""
-        self._fileList = []
+        self._fileLists = []
         if savedir is not None:
             self._saveDir = savedir
         else:
             self._saveDir = getenv('USERPROFILE') or getenv('HOME')
 
     def fetch(self):
         self._fetchDlg.exec_()
@@ -92,32 +89,32 @@
             self._saveBtn.setEnabled(False)
             self._fetchDlg.free_image_files()
             self._suggestedFiles = []
             self._fileLists = []
             self._saveDir = dirname(zip_name)
 
     def checkSave(self):
-        if self._fileList:
+        if self._fileLists:
             msgBox = QMessageBox()
             msgBox.setText("The series has not been saved.")
             msgBox.setInformativeText("Do you want to save it now?")
             msgBox.setStandardButtons(QMessageBox.Save | QMessageBox.Discard | QMessageBox.Cancel)
             msgBox.setDefaultButton(QMessageBox.Save)
 
-        while self._fileList:
-            ret = msgBox.exec_()
-            if ret == QMessageBox.Save:
-                self.save()
-            elif ret == QMessageBox.Discard:
-                self._fetchDlg.free_image_files()
-                self._suggestedFile = ""
-                self._fileList = []
-                return True
-            else:
-                return False
+            while self._fileLists:
+                ret = msgBox.exec_()
+                if ret == QMessageBox.Save:
+                    self.save()
+                elif ret == QMessageBox.Discard:
+                    self._fetchDlg.free_image_files()
+                    self._suggestedFile = ""
+                    self._fileLists = []
+                    return True
+                else:
+                    return False
         return True
 
     def reject(self):
         if self.checkSave():
             self.close()
 
     def closeEvent(self, event):
```

### Comparing `dcmfetch-0.2.0/dcmfetch/dicomweb.py` & `dcmfetch-0.3.1/dcmfetch/dicomweb.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,26 @@
  - stow-rs (c-store).
 
 These are presented here in an api that matches the query interface one
 in queryinterface.py so it can be used as a drop in alternative where
 the dicom server (eg Orthanc) supports this protocol.
 """
 
-from __future__ import division, print_function, absolute_import
 import sys
 from os.path import join
 import email
 from hashlib import md5
 import requests
 
 from . structures import (
     PatientLevelFields, StudyLevelFields,
     SeriesLevelFields, ImageLevelFields,
     CStoreResponse
 )
 
-PY3K = sys.version_info >= (3, 0)
-
 __all__ = [
     'rst_pat_level_find', 'rst_stu_level_find', 'rst_ser_level_find',
     'rst_img_level_find', 'rst_ser_level_get', 'rst_img_level_get'
 ]
 
 
 def _get_simple_tag(json, tagname, default=None):
@@ -377,23 +374,16 @@
         else:
             http_response = s.get(url)
 
     http_response.raise_for_status()
 
     #  Construct valid mime by prepending content type
     hdr = ('Content-Type: ' + http_response.headers['Content-Type']).encode()
-    if PY3K:
-        msg = email.message_from_bytes(hdr + b'\r\n' + http_response.content)
-    else:
-        msg = email.message_from_string(hdr + b'\r\n' + http_response.content)
-
-    if PY3K:
-        serieshash = md5(seriesuid.encode()).digest().hex().upper()
-    else:
-        serieshash = md5(seriesuid).digest().encode('hex').upper()
+    msg = email.message_from_bytes(hdr + b'\r\n' + http_response.content)
+    serieshash = md5(seriesuid.encode()).digest().hex().upper()
 
     fileno = 1
     for part in msg.walk():
         dcmdata = part.get_payload(decode=True)
         if dcmdata is not None:
             filename = join(savedir, 'S%sI%04d.dcm' % (serieshash, fileno))
             with open(filename, 'wb') as f:
@@ -449,18 +439,15 @@
         else:
             http_response = s.get(url)
 
     http_response.raise_for_status()
 
     # Construct valid mime by prepending content type
     hdr = ('Content-Type: ' + http_response.headers['Content-Type']).encode()
-    if PY3K:
-        msg = email.message_from_bytes(hdr + b'\r\n' + http_response.content)
-    else:
-        msg = email.message_from_string(hdr + b'\r\n' + http_response.content)
+    msg = email.message_from_bytes(hdr + b'\r\n' + http_response.content)
 
     fileno = 1
     for part in msg.walk():
         dcmdata = part.get_payload(decode=True)
         if dcmdata is not None:
             filename = join(savedir, '%04d.dcm' % fileno)
             with open(filename, 'wb') as f:
```

### Comparing `dcmfetch-0.2.0/dcmfetch/ext/dcmnodes.cf` & `dcmfetch-0.3.1/dcmfetch/ext/dcmnodes.cf`

 * *Files identical despite different names*

### Comparing `dcmfetch-0.2.0/dcmfetch/ext/findscu` & `dcmfetch-0.3.1/dcmfetch/ext/findscu`

 * *Files identical despite different names*

### Comparing `dcmfetch-0.2.0/dcmfetch/ext/findscu.exe` & `dcmfetch-0.3.1/dcmfetch/ext/findscu.exe`

 * *Files identical despite different names*

### Comparing `dcmfetch-0.2.0/dcmfetch/ext/getscu` & `dcmfetch-0.3.1/dcmfetch/ext/getscu`

 * *Files identical despite different names*

### Comparing `dcmfetch-0.2.0/dcmfetch/ext/getscu.exe` & `dcmfetch-0.3.1/dcmfetch/ext/getscu.exe`

 * *Files identical despite different names*

### Comparing `dcmfetch-0.2.0/dcmfetch/ext/store-tcs.properties` & `dcmfetch-0.3.1/dcmfetch/ext/store-tcs.properties`

 * *Files identical despite different names*

### Comparing `dcmfetch-0.2.0/dcmfetch/fetchdialog.py` & `dcmfetch-0.3.1/dcmfetch/fetchdialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """A Qt based DICOM server browser dialog."""
 
-from __future__ import print_function, division, absolute_import
 from datetime import datetime
 import tempfile
 from shutil import rmtree
 from glob import glob
 from os.path import join, isdir
 import platform
 from collections import Counter
```

### Comparing `dcmfetch-0.2.0/dcmfetch/qidcm4che3.py` & `dcmfetch-0.3.1/dcmfetch/qidcm4che3.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 DICOM query fetch interface based on the dcm4che3 toolkit.
 
 This is a plugin for the generic query interface that uses the more modern dcm4che3
 command line DICOM tools. Both the `findscu` and `getscu` tools are required. These may
 also be installed as standalone tools in the ext subdirectory of the package.
 """
-from __future__ import print_function, division, absolute_import
 
 import subprocess
 import re
 import os
 import sys
 import pkg_resources
```

### Comparing `dcmfetch-0.2.0/dcmfetch/qimock.py` & `dcmfetch-0.3.1/dcmfetch/qimock.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 # -*- coding: utf-8 -*-
 """
 A dummy DICOM query fetch interface.
 
 This is a dummy plugin for the generic query interface. It is for testing and
 allows operation of the web based service even if no dicom tools are installed
 """
-from __future__ import print_function, division, absolute_import
-
 from . structures import QIError
 
 #
 # TODO: not clear if we are better off raising an error or just returning an empty list
 #
 def dcm_pat_level_find(aet, node, port, laet, patname, patid, birthdate, sex):
     """Mock patient level query."""
```

### Comparing `dcmfetch-0.2.0/dcmfetch/qipynetdicom.py` & `dcmfetch-0.3.1/dcmfetch/qipynetdicom.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 DICOM query fetch interface based on pynetdicom at  https://github.com/pydicom/pynetdicom.
 """
 
-from __future__ import print_function, division, absolute_import
-
 import os
 from threading import Thread
 from os.path import join
-
-try:
-    from queue import Queue, Empty
-except ImportError:
-    from Queue import Queue, Empty
-
+from queue import Queue, Empty
 
 from pydicom.dataset import Dataset
 from pydicom.uid import ExplicitVRLittleEndian, ImplicitVRLittleEndian
 
 from pynetdicom import (
     AE, build_role, evt,
     StoragePresentationContexts,
     QueryRetrievePresentationContexts
 )
+
+# typos etc in old versions of pynetdicom
+try:
+    from pynetdicom.sop_class import Verification
+except ImportError:
+    from pynetdicom.sop_class import VerificationSOPClass as Verification
+try:
+    from pynetdicom.sop_class import PerformedImagingAgentAdministrationSRStorage
+except ImportError:
+    from pynetdicom.sop_class import PerformedImagingAgestAdministrationSRStorage as PerformedImagingAgentAdministrationSRStorage
+
 from pynetdicom.sop_class import (
-    VerificationSOPClass,
     PatientRootQueryRetrieveInformationModelFind,
     PatientRootQueryRetrieveInformationModelGet,
     PlannedImagingAgentAdministrationSRStorage,
-    PerformedImagingAgestAdministrationSRStorage,
     EncapsulatedSTLStorage
 )
 
 from . structures import (
     PatientLevelFields, StudyLevelFields, SeriesLevelFields,
     ImageLevelFields,
     CGetResponse, CStoreResponse,
@@ -327,15 +329,15 @@
     query.PatientID = patid
     query.StudyInstanceUID = studyuid
     query.SeriesInstanceUID = seriesuid    
 
     # Add all storage SOP classes except these
     _excluded_contexts = [
         PlannedImagingAgentAdministrationSRStorage,
-        PerformedImagingAgestAdministrationSRStorage,
+        PerformedImagingAgentAdministrationSRStorage,
         EncapsulatedSTLStorage,
     ]
     store_contexts = [
         cx for cx in StoragePresentationContexts
         if cx.abstract_syntax not in _excluded_contexts
     ]
     for cx in store_contexts:
@@ -372,18 +374,18 @@
                     nremaining = nmatches - (ncompleted + nfailed + nwarnings)
                 else:
                     # final
                     ncompleted = state.NumberOfCompletedSuboperations
                     nfailed = state.NumberOfFailedSuboperations
                     nwarnings = state.NumberOfWarningSuboperations
                     nremaining = nmatches - (ncompleted + nfailed + nwarnings)
-            queue.put(CGetResponse(counters[0], nremaining, ncompleted, nfailed, nwarnings, status))
+                queue.put(CGetResponse(counters[0], nremaining, ncompleted, nfailed, nwarnings, status))
         assoc.release()
     else:
-        raise QIError('Association from %s to %s:%3d/%s rejected' % (leat, node, port, aet))
+        raise QIError('Association from %s to %s:%3d/%s rejected' % (laet, node, port, aet))
 
 
 def dcm_img_level_get(aet, node, port, laet, patid, studyuid, seriesuid, imageuid, savedir):
     """
     Use pynetdicom to perform an image level c-get fetch.
 
     This is a coroutine/generator but will yield just a single CGetResponse record to the caller.
@@ -434,15 +436,15 @@
     query.StudyInstanceUID = studyuid
     query.SeriesInstanceUID = seriesuid    
     query.SOPInstanceUID = imageuid    
 
     # Add all storage SOP classes except these
     _excluded_contexts = [
         PlannedImagingAgentAdministrationSRStorage,
-        PerformedImagingAgestAdministrationSRStorage,
+        PerformedImagingAgentAdministrationSRStorage,
         EncapsulatedSTLStorage,
     ]
     store_contexts = [
         cx for cx in StoragePresentationContexts
         if cx.abstract_syntax not in _excluded_contexts
     ]
     for cx in store_contexts:
@@ -468,12 +470,12 @@
             ncompleted = status.NumberOfCompletedSuboperations
             nfailed = status.NumberOfFailedSuboperations
             nwarnings = status.NumberOfWarningSuboperations
             nremaining = 1 - (ncompleted + nfailed + nwarnings)
             yield CGetResponse(index, nremaining, ncompleted, nfailed, nwarnings, status.Status)
         assoc.release()
     else:
-        raise QIError('Association from %s to %s:%3d/%s rejected' % (leat, node, port, aet))
+        raise QIError('Association from %s to %s:%3d/%s rejected' % (laet, node, port, aet))
 
 
 if __name__ == '__main__':
     print("Tests for qipynetdicom.py are in dcmfetch/tests")
```

### Comparing `dcmfetch-0.2.0/dcmfetch/queryinterface.py` & `dcmfetch-0.3.1/dcmfetch/queryinterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from __future__ import print_function, division, absolute_import
-
 from operator import attrgetter
 from platform import node
 from importlib import import_module
 import os
 
 from . aettable import AetTable
 
@@ -153,15 +151,15 @@
                     ComboFields(
                         patid, study.studyuid, study.studyid, study.studydate,
                         series.seriesnumber, series.modality, series.seriesuid, description,
                         nimages, firstimageno, lastimageno
                     )
                 )
 
-        return sorted(comborecords, key=attrgetter('seriesnumber', 'studyid', 'studydate'))
+        return sorted(comborecords, key=attrgetter('studydate', 'studyid', 'seriesnumber'))
 
 
     def image_level_find(self, servername, patid, studyuid, seriesuid):
         """Image level find, returns list of Image records for a series."""
         if servername not in self.aettable:
             raise QIError("%s is not in dicom node table" % servername)
```

### Comparing `dcmfetch-0.2.0/dcmfetch/structures.py` & `dcmfetch-0.3.1/dcmfetch/structures.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 Structures for DICOM requests and responses
 """
-
-from __future__ import print_function, division, absolute_import
-
 from collections import namedtuple
 
 __all__ = [
     'PatientLevelFields', 'StudyLevelFields', 'SeriesLevelFields',
     'ImageLevelFields', 'ComboFields',
     'CGetResponse', 'CStoreResponse',
     'QIError'
```

### Comparing `dcmfetch-0.2.0/dcmfetch.egg-info/PKG-INFO` & `dcmfetch-0.3.1/dcmfetch.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 Metadata-Version: 2.1
 Name: dcmfetch
-Version: 0.2.0
+Version: 0.3.1
 Summary: DICOM query retrieve tools
 Home-page: https://bitbucket.org/rtrhd/dcmfetch
+Download-URL: https://bitbucket.org/rtrhd/dcmfetch/get/v0.3.1.zip
 Author: Ron Hartley-Davies
 Author-email: R.Hartley-Davies@bristol.ac.uk
 License: MIT
-Download-URL: https://bitbucket.org/rtrhd/dcmfetch/get/v0.2.0.zip
-Description: # DICOM Server Access
-        
-        Dcmfetch is a python package for retrieving images from a [DICOM](http://medical.nema.org/) server. The package does not provide a DICOm trnasport itself but wraps either the command line utilies from  [dcm4che3](https://sourceforge.net/projects/dcm4che/files/dcm4che3/) or the native python library[pynetdicom](https://github.com/pydicom/pynetdicom). In addition, bundled standalone versions of the required dcm4che3 tools are included so the only mandatory external (non-python) dependency for the dcm4che3 option is a working java runtime. Further details on installation and use are available [here](docs/dcmfetch.md).
-        
-        The DICOM server must support the dicom `c-find` and `c-get` protocols (not just `c-move`).
-        This is the case for the
-        [dcm4chee](https://sourceforge.net/projects/dcm4che/files/dcm4chee/) server, though several other common servers do not as yet support `c-get`. In addition though, `dcmfetch` supports access to servers such as [orthanc](http://www.orthanc-server.com/) using the `QIDO-RS` and `WADO-RS` web *REST* APIs instead.
-        
-        DICOM servers are identified by keys in the configuration file `dcmnodes.cf`. This file encodes the server details (AET, most, port) together with a string representing facilities supported by the server (including the web API if available). This file is typically installed to the directory `/etc` on a unix system.
-        
-        As well as the python package `dcmfetch` two utilities are provided: `dcmfetch` a command line program to retrieve series and `dcmfetchtool` a [PyQt](https://riverbankcomputing.com/software/pyqt/intro) based graphical tool.
-        
-        ## Licences
-        
-        This package is made available under the [MIT](LICENCE) licence. The included dcm4che3 programs are distributed under the [Mozilla](https://github.com/dcm4che/dcm4che/blob/master/LICENSE.txt) public licence; the only modification here has been to bundle them into single executables.
-         
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
-Provides-Extra: PyNetDicom
+License-File: LICENCE
+Requires-Dist: requests>=2.2.1
+Requires-Dist: QtPy>=1.0.2
+Requires-Dist: pydicom>=1.2.1
+Provides-Extra: pynetdicom
+Requires-Dist: pynetdicom>=1.5.1; extra == "pynetdicom"
+
+# DICOM Server Access
+
+Dcmfetch is a python package for retrieving images from a [DICOM](http://medical.nema.org/) server. The package does not provide a DICOM transport itself but wraps either the command line utilies from  [dcm4che3](https://sourceforge.net/projects/dcm4che/files/dcm4che3/) or the native python library [pynetdicom](https://github.com/pydicom/pynetdicom). In addition, bundled standalone versions of the required dcm4che3 tools are included so the only mandatory external (non-python) dependency for the dcm4che3 option is a working java runtime. Further details on installation and use are available [here](docs/dcmfetch.md).
+
+The DICOM server must support the dicom `c-find` and `c-get` protocols (not just `c-move`).
+This is the case for the
+[dcm4chee](https://sourceforge.net/projects/dcm4che/files/dcm4chee/) server, though several other common servers do not as yet support `c-get`. In addition, `dcmfetch` supports access to servers such as [orthanc](http://www.orthanc-server.com/) using the `QIDO-RS` and `WADO-RS` web *REST* APIs instead.
+
+DICOM servers are identified by keys in the configuration file `dcmnodes.cf`. This file encodes the server details (AET, host, port) together with a string representing facilities supported by the server (including the web API if available). This file is typically installed to the directory `/etc` on a unix system.
+
+As well as the python package `dcmfetch`, two utilities are provided: `dcmfetch` a command line program to retrieve series and `dcmfetchtool` a [PyQt](https://riverbankcomputing.com/software/pyqt/intro) based graphical tool.
+
+## Licences
+
+This package is made available under the [MIT](LICENCE) licence. The included dcm4che3 programs are distributed under the [Mozilla](https://github.com/dcm4che/dcm4che/blob/master/LICENSE.txt) public licence; the only modification here has been to bundle them into single executables.
```

### Comparing `dcmfetch-0.2.0/setup.py` & `dcmfetch-0.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import division, print_function, absolute_import
 from setuptools import setup
 from os.path import join, dirname, abspath
 import sys
 import unittest
 
 # Single definition of version
 __version__ = 'UNDEFINED'
@@ -33,23 +32,25 @@
     install_requires=dependencies,
     extras_require={'PyNetDicom': 'pynetdicom>=1.5.1'},
     packages=['dcmfetch'],
     entry_points={
         'console_scripts': ['dcmfetch = dcmfetch.dcmfetch:main'],
         'gui_scripts': ['dcmfetchtool = dcmfetch.dcmfetchtool:main']
     },
-    package_data={'dcmfetch': ['ext/findscu*', 'ext/getscu*', 'ext/dcmnodes.cf', 'ext/store-tcs.properties']},
+    package_data={
+        'dcmfetch': ['ext/findscu*', 'ext/getscu*', 'ext/dcmnodes.cf', 'ext/store-tcs.properties']
+    },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Medical Science Apps.",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX",
         "Operating System :: Microsoft :: Windows",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8"
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12"
     ]
 )
```

