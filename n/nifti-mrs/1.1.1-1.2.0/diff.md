# Comparing `tmp/nifti_mrs-1.1.1.tar.gz` & `tmp/nifti_mrs-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifti_mrs-1.1.1.tar", last modified: Wed Dec  6 20:01:32 2023, max compression
+gzip compressed data, was "nifti_mrs-1.2.0.tar", last modified: Mon Apr  1 20:35:41 2024, max compression
```

## Comparing `nifti_mrs-1.1.1.tar` & `nifti_mrs-1.2.0.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:01:32.836078 nifti_mrs-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2023-12-06 20:01:32.836078 nifti_mrs-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2023-12-06 20:01:32.836078 nifti_mrs-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:01:32.832078 nifti_mrs-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:01:32.832078 nifti_mrs-1.1.1/src/mrs_tools/
--rw-r--r--   0 runner    (1001) docker     (127)    16945 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/src/mrs_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/src/mrs_tools/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:01:32.832078 nifti_mrs-1.1.1/src/nifti_mrs/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/src/nifti_mrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-12-06 20:01:32.836078 nifti_mrs-1.1.1/src/nifti_mrs/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/src/nifti_mrs/create_nmrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9252 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/src/nifti_mrs/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10233 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/src/nifti_mrs/hdr_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)    24172 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/src/nifti_mrs/nifti_mrs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:01:32.836078 nifti_mrs-1.1.1/src/nifti_mrs/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/src/nifti_mrs/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/src/nifti_mrs/tools/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/src/nifti_mrs/tools/reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/src/nifti_mrs/tools/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)    12785 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/src/nifti_mrs/tools/split_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/src/nifti_mrs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10686 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/src/nifti_mrs/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:01:32.836078 nifti_mrs-1.1.1/src/nifti_mrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2023-12-06 20:01:32.000000 nifti_mrs-1.1.1/src/nifti_mrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2023-12-06 20:01:32.000000 nifti_mrs-1.1.1/src/nifti_mrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 20:01:32.000000 nifti_mrs-1.1.1/src/nifti_mrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-06 20:01:32.000000 nifti_mrs-1.1.1/src/nifti_mrs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-06 20:01:32.000000 nifti_mrs-1.1.1/src/nifti_mrs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-06 20:01:32.000000 nifti_mrs-1.1.1/src/nifti_mrs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 20:01:32.836078 nifti_mrs-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/tests/test_create_nmrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/tests/test_hdr_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)    12272 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/tests/test_nifti_mrs.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/tests/test_nifti_mrs_tools_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/tests/test_nifti_mrs_tools_reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/tests/test_nifti_mrs_tools_reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)    27119 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/tests/test_nifti_mrs_tools_split_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/tests/test_nifti_mrs_tools_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11038 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/tests/test_script_mrs_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2023-12-06 20:01:27.000000 nifti_mrs-1.1.1/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.820174 nifti_mrs-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-01 20:35:41.820174 nifti_mrs-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-01 20:35:41.820174 nifti_mrs-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.812173 nifti_mrs-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.816174 nifti_mrs-1.2.0/src/mrs_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    16945 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/mrs_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/mrs_tools/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.816174 nifti_mrs-1.2.0/src/nifti_mrs/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-01 20:35:41.820174 nifti_mrs-1.2.0/src/nifti_mrs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/create_nmrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/hdr_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24172 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/nifti_mrs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.816174 nifti_mrs-1.2.0/src/nifti_mrs/standard/
+-rw-r--r--   0 runner    (1001) docker     (127)     9549 2024-04-01 20:35:33.000000 nifti_mrs-1.2.0/src/nifti_mrs/standard/definitions.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.816174 nifti_mrs-1.2.0/src/nifti_mrs/standard/explanatory_doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-01 20:35:33.000000 nifti_mrs-1.2.0/src/nifti_mrs/standard/explanatory_doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.816174 nifti_mrs-1.2.0/src/nifti_mrs/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/tools/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/tools/reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/tools/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/tools/split_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10707 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.820174 nifti_mrs-1.2.0/src/nifti_mrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-01 20:35:41.000000 nifti_mrs-1.2.0/src/nifti_mrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-01 20:35:41.000000 nifti_mrs-1.2.0/src/nifti_mrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:35:41.000000 nifti_mrs-1.2.0/src/nifti_mrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 20:35:41.000000 nifti_mrs-1.2.0/src/nifti_mrs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-01 20:35:41.000000 nifti_mrs-1.2.0/src/nifti_mrs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 20:35:41.000000 nifti_mrs-1.2.0/src/nifti_mrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.820174 nifti_mrs-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_create_nmrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_hdr_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_nifti_mrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27119 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_split_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_script_mrs_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_validator.py
```

### Comparing `nifti_mrs-1.1.1/LICENSE` & `nifti_mrs-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.1.1/PKG-INFO` & `nifti_mrs-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifti_mrs
-Version: 1.1.1
+Version: 1.2.0
 Summary: Software tools for the NIfTI-MRS data format
 Home-page: https://github.com/wtclarke/nifti_mrs_tools
 Author: William Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 License: BSD 3-Clause License
 Keywords: MRS
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: nibabel
 Requires-Dist: fslpy
+Requires-Dist: importlib_resources; python_version < "3.10"
 Provides-Extra: vis
 Requires-Dist: fsl-mrs; extra == "vis"
 
 # Python Tools for NIfTI-MRS
 
 ![PyPI](https://img.shields.io/pypi/v/nifti-mrs)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nifti-mrs)
```

### Comparing `nifti_mrs-1.1.1/README.md` & `nifti_mrs-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.1.1/setup.cfg` & `nifti_mrs-1.2.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -17,15 +17,26 @@
 author_email = william.clarke@ndcn.ox.ac.uk
 
 [options]
 install_requires = 
 	numpy
 	nibabel
 	fslpy
+	importlib_resources;python_version<'3.10'
 python_requires = >=3.8
+packages = find_namespace:
+package_dir = 
+	= src
+
+[options.packages.find]
+where = src
+
+[options.package_data]
+nifti_mrs.standard = 
+	definitions.json
 
 [options.extras_require]
 VIS = 
 	fsl-mrs
 
 [options.entry_points]
 console_scripts =
```

### Comparing `nifti_mrs-1.1.1/src/mrs_tools/__init__.py` & `nifti_mrs-1.2.0/src/mrs_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.1.1/src/nifti_mrs/create_nmrs.py` & `nifti_mrs-1.2.0/src/nifti_mrs/create_nmrs.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.1.1/src/nifti_mrs/hdr_ext.py` & `nifti_mrs-1.2.0/src/nifti_mrs/hdr_ext.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,28 +86,43 @@
                     hdr = None
                 obj.set_dim_info(idx - 5, tag, info=info, hdr=hdr)
 
         for key in optional_dict:
             if key in standard_defined:
                 obj.set_standard_def(key, hdr_ext_dict[key])
             else:
-                if 'Value' in hdr_ext_dict[key]\
+                if isinstance(hdr_ext_dict[key], dict)\
+                        and 'Value' in hdr_ext_dict[key]\
                         and 'Description' in hdr_ext_dict[key]:
                     obj.set_user_def(
                         key,
                         hdr_ext_dict[key]['Value'],
                         hdr_ext_dict[key]['Description'])
                 elif isinstance(hdr_ext_dict[key], dict)\
                         and 'Description' in hdr_ext_dict[key]:
                     obj.set_user_def(
                         key,
                         hdr_ext_dict[key],
                         hdr_ext_dict[key]['Description'])
                 else:
-                    raise ValueError(f'User-defined key {key} must contain a "Description" field"')
+                    print(
+                        "This file's header extension is currently invalid. "
+                        f"Reason: User-defined key {key} does not contain a 'Description' field. "
+                        "Setting empty 'Description'.")
+                    if isinstance(hdr_ext_dict[key], dict)\
+                            and 'Value' in hdr_ext_dict[key]:
+                        obj.set_user_def(
+                            key,
+                            hdr_ext_dict[key]['Value'],
+                            '')
+                    else:
+                        obj.set_user_def(
+                            key,
+                            hdr_ext_dict[key],
+                            '')
 
         return obj
 
     @property
     def ndim(self):
         """Returns the number of dimensions implied by the 'dim_{5,6,7}' tags"""
         ndim = 4
```

### Comparing `nifti_mrs-1.1.1/src/nifti_mrs/nifti_mrs.py` & `nifti_mrs-1.2.0/src/nifti_mrs/nifti_mrs.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.1.1/src/nifti_mrs/tools/reorder.py` & `nifti_mrs-1.2.0/src/nifti_mrs/tools/reorder.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.1.1/src/nifti_mrs/tools/reshape.py` & `nifti_mrs-1.2.0/src/nifti_mrs/tools/reshape.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.1.1/src/nifti_mrs/tools/split_merge.py` & `nifti_mrs-1.2.0/src/nifti_mrs/tools/split_merge.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.1.1/src/nifti_mrs/utils.py` & `nifti_mrs-1.2.0/src/nifti_mrs/utils.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.1.1/src/nifti_mrs/validator.py` & `nifti_mrs-1.2.0/src/nifti_mrs/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,27 +214,27 @@
                         )
     # print('Header extension validated!')
 
 
 def check_type(value, json_type):
     '''Checks that values is of type json_type
        json_type may be a tuple to handle array types
-       e.g. (list, float) indicates a list of floats.
+       e.g. (list, str) indicates a list of strings.
     '''
-    if isinstance(json_type, tuple):
-        while len(json_type) > 1:
+    if isinstance(json_type, tuple) and len(json_type) > 1:
+        while json_type[0] == list:
             if not check_type(value, json_type[0]):
                 return False
             try:
                 # TO DO: check more than the first element!
                 value = value[0]
             except TypeError:
                 return False
             json_type = json_type[1:]
-        return check_type(value, json_type[0])
+        return check_type(value, json_type)
     else:
         if isinstance(value, json_type):
             return True
     return False
 
 
 def validate_spectralwidth(header_ex, dwelltime):
```

### Comparing `nifti_mrs-1.1.1/src/nifti_mrs.egg-info/PKG-INFO` & `nifti_mrs-1.2.0/src/nifti_mrs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nifti-mrs
-Version: 1.1.1
+Name: nifti_mrs
+Version: 1.2.0
 Summary: Software tools for the NIfTI-MRS data format
 Home-page: https://github.com/wtclarke/nifti_mrs_tools
 Author: William Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 License: BSD 3-Clause License
 Keywords: MRS
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: nibabel
 Requires-Dist: fslpy
+Requires-Dist: importlib_resources; python_version < "3.10"
 Provides-Extra: vis
 Requires-Dist: fsl-mrs; extra == "vis"
 
 # Python Tools for NIfTI-MRS
 
 ![PyPI](https://img.shields.io/pypi/v/nifti-mrs)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nifti-mrs)
```

### Comparing `nifti_mrs-1.1.1/src/nifti_mrs.egg-info/SOURCES.txt` & `nifti_mrs-1.2.0/src/nifti_mrs.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 src/nifti_mrs/validator.py
 src/nifti_mrs.egg-info/PKG-INFO
 src/nifti_mrs.egg-info/SOURCES.txt
 src/nifti_mrs.egg-info/dependency_links.txt
 src/nifti_mrs.egg-info/entry_points.txt
 src/nifti_mrs.egg-info/requires.txt
 src/nifti_mrs.egg-info/top_level.txt
+src/nifti_mrs/standard/definitions.json
+src/nifti_mrs/standard/explanatory_doc/conf.py
 src/nifti_mrs/tools/__init__.py
 src/nifti_mrs/tools/misc.py
 src/nifti_mrs/tools/reorder.py
 src/nifti_mrs/tools/reshape.py
 src/nifti_mrs/tools/split_merge.py
 tests/test_create_nmrs.py
 tests/test_hdr_ext.py
```

### Comparing `nifti_mrs-1.1.1/tests/test_create_nmrs.py` & `nifti_mrs-1.2.0/tests/test_create_nmrs.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.1.1/tests/test_hdr_ext.py` & `nifti_mrs-1.2.0/tests/test_hdr_ext.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,14 +126,20 @@
 
     dict_rep.update({'dim_6': 'DIM_EDIT', 'RepetitionTime': 1.0})
     hdr2 = Hdr_Ext.from_header_ext(dict_rep)
     assert hdr2.ndim == 6
     assert hdr2._dim_info[1] == {"tag": "DIM_EDIT", "info": None, "hdr": None}
     assert 'RepetitionTime' in hdr2._standard_data
 
+    dict_rep['my_value3'] = 5.0
+    dict_rep['my_value4'] = {'foo': 5.0, }
+    hdr3 = Hdr_Ext.from_header_ext(dict_rep)
+    assert hdr3['my_value3'] == {'Value': 5.0, 'Description': ''}
+    assert hdr3['my_value4'] == {'foo': 5.0, 'Description': ''}
+
 
 def test_to_json():
     hdr = Hdr_Ext(100., '1H', dimensions=5)
     hdr.set_standard_def('EchoTime', 0.3)
     hdr.set_user_def('my_value', 123, 'test metadata')
     hdr.set_user_def('my_value2', {'foo': 123, 'bar': 456, }, 'test metadata')
```

### Comparing `nifti_mrs-1.1.1/tests/test_nifti_mrs.py` & `nifti_mrs-1.2.0/tests/test_nifti_mrs.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.1.1/tests/test_nifti_mrs_tools_reorder.py` & `nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_reorder.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.1.1/tests/test_nifti_mrs_tools_reshape.py` & `nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_reshape.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.1.1/tests/test_nifti_mrs_tools_split_merge.py` & `nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_split_merge.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.1.1/tests/test_nifti_mrs_tools_utils.py` & `nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_utils.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.1.1/tests/test_script_mrs_tools.py` & `nifti_mrs-1.2.0/tests/test_script_mrs_tools.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.1.1/tests/test_validator.py` & `nifti_mrs-1.2.0/tests/test_validator.py`

 * *Files 13% similar despite different names*

```diff
@@ -248,7 +248,52 @@
         ResonantNucleus=["1H", ],
     )
 
     validator.validate_spectralwidth(
         json.dumps(test_dict),
         0.001)
 
+
+def test_check_type():
+    assert validator.check_type(
+        0.5, ((float, int), )
+    )
+
+    assert validator.check_type(
+        1, ((float, int), )
+    )
+
+    assert not validator.check_type(
+        'string', ((float, int), )
+    )
+
+    assert validator.check_type(
+        'string', (str, )
+    )
+
+    assert not validator.check_type(
+        'string', (list, str, )
+    )
+
+    assert validator.check_type(
+        ['s', 'tring'], (list, str, )
+    )
+
+    assert not validator.check_type(
+        ['s', 'tring'], (str, )
+    )
+
+    assert validator.check_type(
+        [['s', 'tring'],], (list, list, str, )
+    )
+
+    assert not validator.check_type(
+        [['s', 'tring'],], (list, str, )
+    )
+
+    assert validator.check_type(
+        [[0.5, 1],], (list, list, (float, int), )
+    )
+
+    assert validator.check_type(
+        [{'a': 1, }, ], (list, dict, )
+    )
```

