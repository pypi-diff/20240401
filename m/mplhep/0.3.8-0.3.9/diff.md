# Comparing `tmp/mplhep-0.3.8.tar.gz` & `tmp/mplhep-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/mplhep/mplhep/dist/tmpurb5_f7f/mplhep-0.3.8.tar", last modified: Mon Jun  7 23:36:36 2021, max compression
+gzip compressed data, was "/home/runner/work/mplhep/mplhep/dist/tmpw7xkvkt9/mplhep-0.3.9.tar", last modified: Mon Jun 14 18:41:24 2021, max compression
```

## Comparing `mplhep-0.3.8.tar` & `mplhep-0.3.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 23:36:36.538973 mplhep-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-06-07 23:36:27.000000 mplhep-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      121 2021-06-07 23:36:27.000000 mplhep-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8792 2021-06-07 23:36:36.538973 mplhep-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7936 2021-06-07 23:36:27.000000 mplhep-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      303 2021-06-07 23:36:27.000000 mplhep-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2021-06-07 23:36:36.538973 mplhep-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      612 2021-06-07 23:36:27.000000 mplhep-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 23:36:36.534973 mplhep-0.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 23:36:36.538973 mplhep-0.3.8/src/mplhep/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-06-07 23:36:27.000000 mplhep-0.3.8/src/mplhep/.VERSION
--rw-r--r--   0 runner    (1001) docker     (121)     1651 2021-06-07 23:36:27.000000 mplhep-0.3.8/src/mplhep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4542 2021-06-07 23:36:27.000000 mplhep-0.3.8/src/mplhep/_deprecate.py
--rw-r--r--   0 runner    (1001) docker     (121)      300 2021-06-07 23:36:27.000000 mplhep-0.3.8/src/mplhep/_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2021-06-07 23:36:27.000000 mplhep-0.3.8/src/mplhep/alice.py
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2021-06-07 23:36:27.000000 mplhep-0.3.8/src/mplhep/atlas.py
--rw-r--r--   0 runner    (1001) docker     (121)     1446 2021-06-07 23:36:27.000000 mplhep-0.3.8/src/mplhep/cms.py
--rw-r--r--   0 runner    (1001) docker     (121)     2174 2021-06-07 23:36:27.000000 mplhep-0.3.8/src/mplhep/error_estimation.py
--rw-r--r--   0 runner    (1001) docker     (121)    13713 2021-06-07 23:36:27.000000 mplhep-0.3.8/src/mplhep/label.py
--rw-r--r--   0 runner    (1001) docker     (121)     2410 2021-06-07 23:36:27.000000 mplhep-0.3.8/src/mplhep/lhcb.py
--rw-r--r--   0 runner    (1001) docker     (121)    30767 2021-06-07 23:36:27.000000 mplhep-0.3.8/src/mplhep/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 23:36:36.538973 mplhep-0.3.8/src/mplhep/styles/
--rw-r--r--   0 runner    (1001) docker     (121)     1933 2021-06-07 23:36:27.000000 mplhep-0.3.8/src/mplhep/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2021-06-07 23:36:27.000000 mplhep-0.3.8/src/mplhep/styles/alice.py
--rw-r--r--   0 runner    (1001) docker     (121)     3724 2021-06-07 23:36:27.000000 mplhep-0.3.8/src/mplhep/styles/atlas.py
--rw-r--r--   0 runner    (1001) docker     (121)     2426 2021-06-07 23:36:27.000000 mplhep-0.3.8/src/mplhep/styles/cms.py
--rw-r--r--   0 runner    (1001) docker     (121)     6126 2021-06-07 23:36:27.000000 mplhep-0.3.8/src/mplhep/styles/lhcb.py
--rw-r--r--   0 runner    (1001) docker     (121)     4199 2021-06-07 23:36:27.000000 mplhep-0.3.8/src/mplhep/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 23:36:36.538973 mplhep-0.3.8/src/mplhep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8792 2021-06-07 23:36:36.000000 mplhep-0.3.8/src/mplhep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      656 2021-06-07 23:36:36.000000 mplhep-0.3.8/src/mplhep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-07 23:36:36.000000 mplhep-0.3.8/src/mplhep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-07 23:36:36.000000 mplhep-0.3.8/src/mplhep.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      449 2021-06-07 23:36:36.000000 mplhep-0.3.8/src/mplhep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-07 23:36:36.000000 mplhep-0.3.8/src/mplhep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 18:41:24.951963 mplhep-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-06-14 18:41:16.000000 mplhep-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2021-06-14 18:41:16.000000 mplhep-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     8792 2021-06-14 18:41:24.951963 mplhep-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7936 2021-06-14 18:41:16.000000 mplhep-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2021-06-14 18:41:16.000000 mplhep-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1309 2021-06-14 18:41:24.951963 mplhep-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      612 2021-06-14 18:41:16.000000 mplhep-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 18:41:24.939963 mplhep-0.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 18:41:24.947963 mplhep-0.3.9/src/mplhep/
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-06-14 18:41:16.000000 mplhep-0.3.9/src/mplhep/.VERSION
+-rw-r--r--   0 runner    (1001) docker     (121)     1651 2021-06-14 18:41:16.000000 mplhep-0.3.9/src/mplhep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4542 2021-06-14 18:41:16.000000 mplhep-0.3.9/src/mplhep/_deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2021-06-14 18:41:16.000000 mplhep-0.3.9/src/mplhep/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1187 2021-06-14 18:41:16.000000 mplhep-0.3.9/src/mplhep/alice.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2279 2021-06-14 18:41:16.000000 mplhep-0.3.9/src/mplhep/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1446 2021-06-14 18:41:16.000000 mplhep-0.3.9/src/mplhep/cms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2174 2021-06-14 18:41:16.000000 mplhep-0.3.9/src/mplhep/error_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13713 2021-06-14 18:41:16.000000 mplhep-0.3.9/src/mplhep/label.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2410 2021-06-14 18:41:16.000000 mplhep-0.3.9/src/mplhep/lhcb.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30771 2021-06-14 18:41:16.000000 mplhep-0.3.9/src/mplhep/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 18:41:24.951963 mplhep-0.3.9/src/mplhep/styles/
+-rw-r--r--   0 runner    (1001) docker     (121)     1933 2021-06-14 18:41:16.000000 mplhep-0.3.9/src/mplhep/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1266 2021-06-14 18:41:16.000000 mplhep-0.3.9/src/mplhep/styles/alice.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3724 2021-06-14 18:41:16.000000 mplhep-0.3.9/src/mplhep/styles/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2426 2021-06-14 18:41:16.000000 mplhep-0.3.9/src/mplhep/styles/cms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6126 2021-06-14 18:41:16.000000 mplhep-0.3.9/src/mplhep/styles/lhcb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4199 2021-06-14 18:41:16.000000 mplhep-0.3.9/src/mplhep/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 18:41:24.947963 mplhep-0.3.9/src/mplhep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8792 2021-06-14 18:41:24.000000 mplhep-0.3.9/src/mplhep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2021-06-14 18:41:24.000000 mplhep-0.3.9/src/mplhep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-14 18:41:24.000000 mplhep-0.3.9/src/mplhep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-14 18:41:24.000000 mplhep-0.3.9/src/mplhep.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      449 2021-06-14 18:41:24.000000 mplhep-0.3.9/src/mplhep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-14 18:41:24.000000 mplhep-0.3.9/src/mplhep.egg-info/top_level.txt
```

### Comparing `mplhep-0.3.8/LICENSE` & `mplhep-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/PKG-INFO` & `mplhep-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mplhep
-Version: 0.3.8
+Version: 0.3.9
 Summary: Matplotlib styles for HEP
 Home-page: https://github.com/scikit-hep/mplhep
 Author: andrzejnovak
 Author-email: "novak5andrzej@gmail.com"
 Maintainer: Scikit-HEP
 Maintainer-email: scikit-hep-admins@googlegroups.com
 License: MIT License
```

### Comparing `mplhep-0.3.8/README.md` & `mplhep-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/setup.cfg` & `mplhep-0.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/setup.py` & `mplhep-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/src/mplhep/__init__.py` & `mplhep-0.3.9/src/mplhep/__init__.py`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/src/mplhep/_deprecate.py` & `mplhep-0.3.9/src/mplhep/_deprecate.py`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/src/mplhep/alice.py` & `mplhep-0.3.9/src/mplhep/alice.py`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/src/mplhep/atlas.py` & `mplhep-0.3.9/src/mplhep/atlas.py`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/src/mplhep/cms.py` & `mplhep-0.3.9/src/mplhep/cms.py`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/src/mplhep/error_estimation.py` & `mplhep-0.3.9/src/mplhep/error_estimation.py`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/src/mplhep/label.py` & `mplhep-0.3.9/src/mplhep/label.py`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/src/mplhep/lhcb.py` & `mplhep-0.3.9/src/mplhep/lhcb.py`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/src/mplhep/plot.py` & `mplhep-0.3.9/src/mplhep/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,15 @@
             )
         _artist = _s
 
     elif histtype == "fill":
         for i in range(len(hists)):
             _kwargs = _chunked_kwargs[i]
             _f = ax.stairs(h[i], final_bins, label=_labels[i], fill=True, **_kwargs)
-        return_artists.append(StairsArtists(_f, None, None))
+            return_artists.append(StairsArtists(_f, None, None))
         _artist = _f
 
     elif histtype == "errorbar":
         err_defaults = {
             "linestyle": "none",
             "marker": ".",
             "markersize": 10.0,
```

### Comparing `mplhep-0.3.8/src/mplhep/styles/__init__.py` & `mplhep-0.3.9/src/mplhep/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/src/mplhep/styles/alice.py` & `mplhep-0.3.9/src/mplhep/styles/alice.py`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/src/mplhep/styles/atlas.py` & `mplhep-0.3.9/src/mplhep/styles/atlas.py`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/src/mplhep/styles/cms.py` & `mplhep-0.3.9/src/mplhep/styles/cms.py`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/src/mplhep/styles/lhcb.py` & `mplhep-0.3.9/src/mplhep/styles/lhcb.py`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/src/mplhep/utils.py` & `mplhep-0.3.9/src/mplhep/utils.py`

 * *Files identical despite different names*

### Comparing `mplhep-0.3.8/src/mplhep.egg-info/PKG-INFO` & `mplhep-0.3.9/src/mplhep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mplhep
-Version: 0.3.8
+Version: 0.3.9
 Summary: Matplotlib styles for HEP
 Home-page: https://github.com/scikit-hep/mplhep
 Author: andrzejnovak
 Author-email: "novak5andrzej@gmail.com"
 Maintainer: Scikit-HEP
 Maintainer-email: scikit-hep-admins@googlegroups.com
 License: MIT License
```

### Comparing `mplhep-0.3.8/src/mplhep.egg-info/SOURCES.txt` & `mplhep-0.3.9/src/mplhep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

