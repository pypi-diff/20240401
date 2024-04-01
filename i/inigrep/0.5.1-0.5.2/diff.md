# Comparing `tmp/inigrep-0.5.1.tar.gz` & `tmp/inigrep-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inigrep-0.5.1.tar", last modified: Wed Mar  6 13:06:54 2024, max compression
+gzip compressed data, was "inigrep-0.5.2.tar", last modified: Mon Apr  1 15:45:18 2024, max compression
```

## Comparing `inigrep-0.5.1.tar` & `inigrep-0.5.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-03-06 13:06:54.133042 inigrep-0.5.1/
--rw-r--r--   0 netvor    (9860) netvor    (9860)    26338 2020-08-03 17:39:27.000000 inigrep-0.5.1/LICENSE.md
--rw-r--r--   0 netvor    (9860) netvor    (9860)     1657 2024-03-06 13:06:54.133042 inigrep-0.5.1/PKG-INFO
--rw-r--r--   0 netvor    (9860) netvor    (9860)       38 2023-04-05 14:47:14.000000 inigrep-0.5.1/README.md
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-03-06 13:06:54.133042 inigrep-0.5.1/inigrep.egg-info/
--rw-r--r--   0 netvor    (9860) netvor    (9860)     1657 2024-03-06 13:06:54.000000 inigrep-0.5.1/inigrep.egg-info/PKG-INFO
--rw-r--r--   0 netvor    (9860) netvor    (9860)      306 2024-03-06 13:06:54.000000 inigrep-0.5.1/inigrep.egg-info/SOURCES.txt
--rw-r--r--   0 netvor    (9860) netvor    (9860)        1 2024-03-06 13:06:54.000000 inigrep-0.5.1/inigrep.egg-info/dependency_links.txt
--rw-r--r--   0 netvor    (9860) netvor    (9860)        8 2024-03-06 13:06:54.000000 inigrep-0.5.1/inigrep.egg-info/top_level.txt
--rw-r--r--   0 netvor    (9860) netvor    (9860)       38 2024-03-06 13:06:54.133042 inigrep-0.5.1/setup.cfg
--rw-r--r--   0 netvor    (9860) netvor    (9860)    12693 2024-03-06 13:06:49.000000 inigrep-0.5.1/setup.py
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-03-06 13:06:54.129042 inigrep-0.5.1/src/
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-03-06 13:06:54.129042 inigrep-0.5.1/src/inigrep/
--rw-r--r--   0 netvor    (9860) netvor    (9860)      175 2023-03-12 00:22:00.000000 inigrep-0.5.1/src/inigrep/__init__.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)     7441 2023-03-12 00:22:00.000000 inigrep-0.5.1/src/inigrep/__main__.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)      546 2024-03-06 13:06:48.000000 inigrep-0.5.1/src/inigrep/_meta.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)    14059 2023-03-12 00:22:00.000000 inigrep-0.5.1/src/inigrep/core.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)    10558 2023-03-12 00:22:00.000000 inigrep-0.5.1/src/inigrep/front.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)        0 2023-03-12 00:22:00.000000 inigrep-0.5.1/src/inigrep/py.typed
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-03-06 13:06:54.129042 inigrep-0.5.1/tests/
--rw-r--r--   0 netvor    (9860) netvor    (9860)    26767 2024-02-20 21:47:27.000000 inigrep-0.5.1/tests/test_inigrep.py
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-01 15:45:18.095987 inigrep-0.5.2/
+-rw-r--r--   0 netvor    (9860) netvor    (9860)    26338 2020-08-03 17:39:27.000000 inigrep-0.5.2/LICENSE.md
+-rw-r--r--   0 netvor    (9860) netvor    (9860)     1689 2024-04-01 15:45:18.095987 inigrep-0.5.2/PKG-INFO
+-rw-r--r--   0 netvor    (9860) netvor    (9860)       38 2023-04-05 14:47:14.000000 inigrep-0.5.2/README.md
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-01 15:45:18.095987 inigrep-0.5.2/inigrep.egg-info/
+-rw-r--r--   0 netvor    (9860) netvor    (9860)     1689 2024-04-01 15:45:18.000000 inigrep-0.5.2/inigrep.egg-info/PKG-INFO
+-rw-r--r--   0 netvor    (9860) netvor    (9860)      325 2024-04-01 15:45:18.000000 inigrep-0.5.2/inigrep.egg-info/SOURCES.txt
+-rw-r--r--   0 netvor    (9860) netvor    (9860)        1 2024-04-01 15:45:18.000000 inigrep-0.5.2/inigrep.egg-info/dependency_links.txt
+-rw-r--r--   0 netvor    (9860) netvor    (9860)        8 2024-04-01 15:45:18.000000 inigrep-0.5.2/inigrep.egg-info/top_level.txt
+-rw-r--r--   0 netvor    (9860) netvor    (9860)       38 2024-04-01 15:45:18.095987 inigrep-0.5.2/setup.cfg
+-rw-r--r--   0 netvor    (9860) netvor    (9860)    12664 2024-04-01 15:45:13.000000 inigrep-0.5.2/setup.py
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-01 15:45:18.095987 inigrep-0.5.2/src/
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-01 15:45:18.095987 inigrep-0.5.2/src/inigrep/
+-rw-r--r--   0 netvor    (9860) netvor    (9860)      175 2023-03-12 00:22:00.000000 inigrep-0.5.2/src/inigrep/__init__.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)       68 2024-04-01 15:37:56.000000 inigrep-0.5.2/src/inigrep/__main__.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)      546 2024-04-01 15:45:12.000000 inigrep-0.5.2/src/inigrep/_meta.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)     7401 2024-04-01 15:37:56.000000 inigrep-0.5.2/src/inigrep/cli.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)    15540 2024-04-01 15:37:56.000000 inigrep-0.5.2/src/inigrep/core.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)    10558 2023-03-12 00:22:00.000000 inigrep-0.5.2/src/inigrep/front.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)        0 2023-03-12 00:22:00.000000 inigrep-0.5.2/src/inigrep/py.typed
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2024-04-01 15:45:18.095987 inigrep-0.5.2/tests/
+-rw-r--r--   0 netvor    (9860) netvor    (9860)    26767 2024-04-01 15:44:20.000000 inigrep-0.5.2/tests/test_inigrep.py
```

### Comparing `inigrep-0.5.1/LICENSE.md` & `inigrep-0.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `inigrep-0.5.1/PKG-INFO` & `inigrep-0.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inigrep
-Version: 0.5.1
+Version: 0.5.2
 Summary: inigrep - grep for (some) INIs
 Home-page: https://gitlab.com/vornet/python/python-inigrep
 Maintainer-email: Alois Mahdal <netvor+inigrep@vornet.cz>
 License: LGPLv2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Natural Language :: English
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires: __VDK_PYPI_REQUIRES__
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 inigrep is designed to read a particular simplistic dialect of
 INI configuration files.  In a sense, it can be considered as
 a "grep for INIs", in that rather than parsing the file into
 a typed memory structure for later access, it passes file each
```

### Comparing `inigrep-0.5.1/inigrep.egg-info/PKG-INFO` & `inigrep-0.5.2/inigrep.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inigrep
-Version: 0.5.1
+Version: 0.5.2
 Summary: inigrep - grep for (some) INIs
 Home-page: https://gitlab.com/vornet/python/python-inigrep
 Maintainer-email: Alois Mahdal <netvor+inigrep@vornet.cz>
 License: LGPLv2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Natural Language :: English
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires: __VDK_PYPI_REQUIRES__
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 inigrep is designed to read a particular simplistic dialect of
 INI configuration files.  In a sense, it can be considered as
 a "grep for INIs", in that rather than parsing the file into
 a typed memory structure for later access, it passes file each
```

### Comparing `inigrep-0.5.1/setup.py` & `inigrep-0.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,18 +136,14 @@
     '__VDK_PYLIB_PKGMAP__',
 ]
 
 VDK_PYLIB_DEFAULT_PKGMAP = """
 inigrep src/inigrep py.typed
 """
 
-VDK_PYLIB_REQUIRES_PYSTUFF = [
-    '__VDK_PYLIB_REQUIRES_PYSTUFF__',
-]
-
 VDK_PYLIB_CLASSIFIERS_OVERRIDE = [
     '__VDK_PYLIB_CLASSIFIERS_OVERRIDE__',
 ]
 
 VDK_PYLIB_CLASSIFIERS = [
     'Intended Audience :: Developers',
     'Intended Audience :: Information Technology',
@@ -158,14 +154,18 @@
 __VDK_PYLIB_PYTHON_GE__
 """
 
 VDK_PYLIB_PYTHON_LT = """
 __VDK_PYLIB_PYTHON_LT__
 """
 
+VDK_PYPI_REQUIRES = [
+    '__VDK_PYPI_REQUIRES__',
+]
+
 MKIT_PROJ_LICENSE = """
 LGPLv2
 """
 
 
 class PackageMapItem:
 
@@ -358,13 +358,13 @@
     long_description_content_type='text/markdown',
     maintainer_email='Alois Mahdal <netvor+inigrep@vornet.cz>',
     name='inigrep',
     packages=VDK_PACKAGEINFO['packages'],
     package_dir=VDK_PACKAGEINFO['package_dir'],
     package_data=VDK_PACKAGEINFO['package_data'],
     url='https://gitlab.com/vornet/python/python-inigrep',
-    requires=vdk_cleanup(VDK_PYLIB_REQUIRES_PYSTUFF),
-    version='0.5.1',
+    requires=vdk_cleanup(VDK_PYPI_REQUIRES),
+    version='0.5.2',
     classifiers=VDK_PACKAGEINFO['classifiers'],
 )
 
-# setup.py built with MKit 0.0.60 and vdk-pylib-0.0.36
+# setup.py built with MKit 0.1.3 and vdk-pylib-0.1.1
```

### Comparing `inigrep-0.5.1/src/inigrep/__main__.py` & `inigrep-0.5.2/src/inigrep/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,11 +251,7 @@
         for line in gen:
             print(line)
             if options.oneline:
                 break
     except inigrep.core.KeypathError as e:
         sys.stderr.write('%s\n' % e)
         sys.exit(2)
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `inigrep-0.5.1/src/inigrep/_meta.py` & `inigrep-0.5.2/src/inigrep/_meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 CODENAME: str = """
 
 """.strip()
 
 GIT_LASTHASH: str = """
-5982eb804fe4d69df8e2f05215b71f71903da589
+b4e61008e20de4be7668eb67fe728c7038557c05
 """.strip()
 
 GIT_LASTSUMMARY: str = """
-Bump version to 0.5.1
+Bump version to 0.5.2
 """.strip()
 
 LICENSE: str = """
 LGPLv2
 """.strip()
 
 MAINTAINER: str = """
@@ -31,9 +31,9 @@
 """.strip()
 
 VCS_BROWSER: str = """
 https://gitlab.com/vornet/python/python-inigrep
 """.strip()
 
 VERSION: str = """
-0.5.1
+0.5.2
 """.strip()
```

### Comparing `inigrep-0.5.1/src/inigrep/core.py` & `inigrep-0.5.2/src/inigrep/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/python3
 
 from __future__ import annotations
 
-import functools
 import os
 import re
 import sys
 import typing
 
 
 class NIL:
@@ -387,14 +386,66 @@
         cond=Cond.from_arg(kpath, require_sct=False, require_key=False),
         extractor=extract_clones,
     )
     for line in pipe:
         yield ClonedLineT(line)
 
 
+def _r_data(reader: LineGenT) -> dict[KeyT, list[ValueT]]:
+    """
+    Return dict of all keypaths and values found by *reader*
+
+    *reader* must be instance of FileReader generator or any similar
+    generator that will yield lines.
+    """
+    lines = list(reader)
+    keypath_pipe = mkpipe(
+        reader=iter(lines),
+        cond=AlwaysMatchingCond(),
+        extractor=extract_keypaths,
+    )
+    out: dict[KeyT, list[ValueT]] = {}
+    for keypath in keypath_pipe:
+        value_pipe = mkpipe(
+            reader=iter(lines),
+            cond=Cond.from_arg(keypath),
+            extractor=extract_values,
+        )
+        if keypath not in out:
+            out[keypath] = []
+        out[keypath].extend(value_pipe)
+    return out
+
+
+def _r_raw_data(reader: LineGenT) -> dict[KeyT, list[RawValueT]]:
+    """
+    Return dict of all keypaths and raw values found by *reader*
+
+    *reader* must be instance of FileReader generator or any similar
+    generator that will yield lines.
+    """
+    lines = list(reader)
+    keypath_pipe = mkpipe(
+        reader=iter(lines),
+        cond=AlwaysMatchingCond(),
+        extractor=extract_keypaths,
+    )
+    out: dict[KeyT, list[RawValueT]] = {}
+    for keypath in keypath_pipe:
+        value_pipe = mkpipe(
+            reader=iter(lines),
+            cond=Cond.from_arg(keypath),
+            extractor=extract_raw_values,
+        )
+        if keypath not in out:
+            out[keypath] = []
+        out[keypath].extend(value_pipe)
+    return out
+
+
 def _r_values(reader: LineGenT, kpath: str) -> ValueGenT:
     """
     Return list of values found by *reader* at key path *kpath*.
 
     *kpath* must be key path, i.e. string containing section and
     key names delimited by period.
```

### Comparing `inigrep-0.5.1/src/inigrep/front.py` & `inigrep-0.5.2/src/inigrep/front.py`

 * *Files identical despite different names*

### Comparing `inigrep-0.5.1/tests/test_inigrep.py` & `inigrep-0.5.2/tests/test_inigrep.py`

 * *Files identical despite different names*

