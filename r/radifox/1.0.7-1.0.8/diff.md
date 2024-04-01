# Comparing `tmp/radifox-1.0.7.tar.gz` & `tmp/radifox-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radifox-1.0.7.tar", last modified: Tue Mar 19 16:32:14 2024, max compression
+gzip compressed data, was "radifox-1.0.8.tar", last modified: Mon Apr  1 21:10:30 2024, max compression
```

## Comparing `radifox-1.0.7.tar` & `radifox-1.0.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:32:14.845890 radifox-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-19 16:32:07.000000 radifox-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    46888 2024-03-19 16:32:14.845890 radifox-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    45907 2024-03-19 16:32:07.000000 radifox-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:32:14.845890 radifox-1.0.7/radifox/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-19 16:32:14.845890 radifox-1.0.7/radifox/_static_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:32:14.841890 radifox-1.0.7/radifox/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42431 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/conversion/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/conversion/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    13538 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/conversion/dicom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/conversion/exec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/conversion/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/conversion/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/conversion/lut.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/conversion/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    55768 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/conversion/nib_parrec_fork.py
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/conversion/parrec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:32:14.841890 radifox-1.0.7/radifox/conversion/parrec_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/conversion/parrec_templates/gen_info.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/conversion/parrec_templates/pixel_values.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/conversion/parrec_templates/top_header.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/conversion/parrec_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/conversion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:32:14.841890 radifox-1.0.7/radifox/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16756 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/modules/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:32:14.841890 radifox-1.0.7/radifox/naming/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/naming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/naming/imagefile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:32:14.845890 radifox-1.0.7/radifox/qa/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/qa/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/qa/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/qa/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:32:14.845890 radifox-1.0.7/radifox/qa/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/qa/templates/conversion.html
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/qa/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/qa/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/qa/templates/processing.html
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/qa/templates/project.html
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/qa/templates/subject.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:32:14.845890 radifox-1.0.7/radifox/records/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/records/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-19 16:32:07.000000 radifox-1.0.7/radifox/records/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:32:14.845890 radifox-1.0.7/radifox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46888 2024-03-19 16:32:14.000000 radifox-1.0.7/radifox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-19 16:32:14.000000 radifox-1.0.7/radifox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 16:32:14.000000 radifox-1.0.7/radifox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-19 16:32:14.000000 radifox-1.0.7/radifox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-19 16:32:14.000000 radifox-1.0.7/radifox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-19 16:32:14.000000 radifox-1.0.7/radifox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 16:32:14.845890 radifox-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-03-19 16:32:07.000000 radifox-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.169299 radifox-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-01 21:10:25.000000 radifox-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    46888 2024-04-01 21:10:30.169299 radifox-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    45907 2024-04-01 21:10:25.000000 radifox-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.169299 radifox-1.0.8/radifox/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 21:10:30.169299 radifox-1.0.8/radifox/_static_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.161299 radifox-1.0.8/radifox/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42431 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13538 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/dicom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/lut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55768 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/nib_parrec_fork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/parrec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.165299 radifox-1.0.8/radifox/conversion/parrec_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/parrec_templates/gen_info.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/parrec_templates/pixel_values.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/parrec_templates/top_header.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/parrec_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/conversion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.165299 radifox-1.0.8/radifox/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16756 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/modules/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.165299 radifox-1.0.8/radifox/naming/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/naming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/naming/imagefile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.165299 radifox-1.0.8/radifox/qa/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.165299 radifox-1.0.8/radifox/qa/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/templates/conversion.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/templates/processing.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/templates/project.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/qa/templates/subject.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.165299 radifox-1.0.8/radifox/records/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/records/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-01 21:10:25.000000 radifox-1.0.8/radifox/records/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:30.165299 radifox-1.0.8/radifox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46888 2024-04-01 21:10:30.000000 radifox-1.0.8/radifox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-01 21:10:30.000000 radifox-1.0.8/radifox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:10:30.000000 radifox-1.0.8/radifox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 21:10:30.000000 radifox-1.0.8/radifox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-01 21:10:30.000000 radifox-1.0.8/radifox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 21:10:30.000000 radifox-1.0.8/radifox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:10:30.169299 radifox-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-01 21:10:25.000000 radifox-1.0.8/setup.py
```

### Comparing `radifox-1.0.7/LICENSE` & `radifox-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/PKG-INFO` & `radifox-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radifox
-Version: 1.0.7
+Version: 1.0.8
 Summary: RADIFOX is the RADiological Image File Ontology eXtension, a Python package for the organization and management of medical images.
 Home-page: https://github.com/jh-mipc/radifox
 Author: Blake Dewey
 Author-email: blake.dewey@jhu.edu
 License: Apache License, 2.0
 Keywords: mri conversion
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `radifox-1.0.7/README.md` & `radifox-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/_version.py` & `radifox-1.0.8/radifox/_version.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/conversion/base.py` & `radifox-1.0.8/radifox/conversion/base.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/conversion/cli.py` & `radifox-1.0.8/radifox/conversion/cli.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/conversion/dicom.py` & `radifox-1.0.8/radifox/conversion/dicom.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/conversion/exec.py` & `radifox-1.0.8/radifox/conversion/exec.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from .metadata import Metadata
 from .lut import LookupTable
 from .parrec import ParrecSet, sort_parrecs
 from .utils import (
     mkdir_p,
     extract_archive,
     allowed_archives,
-    recursive_chmod,
     copytree_link,
     DIR_OCTAL,
     has_permissions,
     hash_value,
 )
 
 
@@ -91,20 +90,18 @@
             elif any([source.name.endswith(ext) for ext in allowed_archives()[1]]):
                 extract_archive(source, type_folder)
             else:
                 raise ValueError(
                     "Source is not a directory, but does not match one of "
                     "the available archive formats (%s)" % ", ".join(allowed_archives()[0])
                 )
-            recursive_chmod(type_folder)
             if parrec:
                 sort_parrecs(type_folder)
             else:
                 sort_dicoms(type_folder, force_dicom)
-            recursive_chmod(type_folder)
 
         if parrec:
             img_set = ParrecSet(
                 source,
                 output_root,
                 metadata,
                 lut,
@@ -122,19 +119,16 @@
                 lut,
                 remove_identifiers,
                 date_shift_days,
                 manual_names,
                 input_hash=input_hash,
             )
         img_set.create_all_nii()
-        recursive_chmod(session_path / "nii")
-        recursive_chmod(session_path / "qa")
         img_set.generate_unconverted_info()
 
-        recursive_chmod(session_path / "logs")
         if remove_identifiers:
             shutil.rmtree(type_folder)
         logging.info("RADIFOX conversion finished: %s" % metadata.dir_to_str())
     except KeyboardInterrupt:
         raise
     except:
         logging.exception("Fatal error occurred.")
```

### Comparing `radifox-1.0.7/radifox/conversion/json.py` & `radifox-1.0.8/radifox/conversion/json.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/conversion/logging.py` & `radifox-1.0.8/radifox/conversion/logging.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/conversion/lut.py` & `radifox-1.0.8/radifox/conversion/lut.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/conversion/metadata.py` & `radifox-1.0.8/radifox/conversion/metadata.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/conversion/nib_parrec_fork.py` & `radifox-1.0.8/radifox/conversion/nib_parrec_fork.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/conversion/parrec.py` & `radifox-1.0.8/radifox/conversion/parrec.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/conversion/parrec_templates/gen_info.txt` & `radifox-1.0.8/radifox/conversion/parrec_templates/gen_info.txt`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/conversion/parrec_templates/pixel_values.txt` & `radifox-1.0.8/radifox/conversion/parrec_templates/pixel_values.txt`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/conversion/parrec_writer.py` & `radifox-1.0.8/radifox/conversion/parrec_writer.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/conversion/utils.py` & `radifox-1.0.8/radifox/conversion/utils.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/modules/staging.py` & `radifox-1.0.8/radifox/modules/staging.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/naming/imagefile.py` & `radifox-1.0.8/radifox/naming/imagefile.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/qa/app.py` & `radifox-1.0.8/radifox/qa/app.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/qa/create.py` & `radifox-1.0.8/radifox/qa/create.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/qa/run.py` & `radifox-1.0.8/radifox/qa/run.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/qa/templates/conversion.html` & `radifox-1.0.8/radifox/qa/templates/conversion.html`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/qa/templates/index.html` & `radifox-1.0.8/radifox/qa/templates/index.html`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/qa/templates/login.html` & `radifox-1.0.8/radifox/qa/templates/login.html`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/qa/templates/processing.html` & `radifox-1.0.8/radifox/qa/templates/processing.html`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/qa/templates/project.html` & `radifox-1.0.8/radifox/qa/templates/project.html`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/qa/templates/subject.html` & `radifox-1.0.8/radifox/qa/templates/subject.html`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/records/processing.py` & `radifox-1.0.8/radifox/records/processing.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox/records/utils.py` & `radifox-1.0.8/radifox/records/utils.py`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/radifox.egg-info/PKG-INFO` & `radifox-1.0.8/radifox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radifox
-Version: 1.0.7
+Version: 1.0.8
 Summary: RADIFOX is the RADiological Image File Ontology eXtension, a Python package for the organization and management of medical images.
 Home-page: https://github.com/jh-mipc/radifox
 Author: Blake Dewey
 Author-email: blake.dewey@jhu.edu
 License: Apache License, 2.0
 Keywords: mri conversion
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `radifox-1.0.7/radifox.egg-info/SOURCES.txt` & `radifox-1.0.8/radifox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radifox-1.0.7/setup.py` & `radifox-1.0.8/setup.py`

 * *Files identical despite different names*

