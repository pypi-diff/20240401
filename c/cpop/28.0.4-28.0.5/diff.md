# Comparing `tmp/cpop-28.0.4.tar.gz` & `tmp/cpop-28.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpop-28.0.4.tar", last modified: Mon Apr  1 21:00:43 2024, max compression
+gzip compressed data, was "cpop-28.0.5.tar", last modified: Mon Apr  1 21:05:50 2024, max compression
```

## Comparing `cpop-28.0.4.tar` & `cpop-28.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:00:43.327643 cpop-28.0.4/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.0.4/LICENSE
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      104 2024-04-01 20:54:49.000000 cpop-28.0.4/MANIFEST.in
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 21:00:43.327643 cpop-28.0.4/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4063 2024-04-01 20:42:25.000000 cpop-28.0.4/README.rst
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:00:43.323643 cpop-28.0.4/cpop.egg-info/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 21:00:43.000000 cpop-28.0.4/cpop.egg-info/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      535 2024-04-01 21:00:43.000000 cpop-28.0.4/cpop.egg-info/SOURCES.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-01 21:00:43.000000 cpop-28.0.4/cpop.egg-info/dependency_links.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-01 21:00:43.000000 cpop-28.0.4/cpop.egg-info/entry_points.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      128 2024-04-01 21:00:43.000000 cpop-28.0.4/cpop.egg-info/requires.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        4 2024-04-01 21:00:43.000000 cpop-28.0.4/cpop.egg-info/top_level.txt
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:00:43.323643 cpop-28.0.4/hub/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.0.4/hub/__init__.py
--rwxrwxr-x   0 akmod     (1000) akmod     (1000)     1979 2024-04-01 18:01:36.000000 cpop-28.0.4/hub/__main__.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:00:43.323643 cpop-28.0.4/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    10888 2024-04-01 16:10:17.000000 cpop-28.0.4/pop/contract.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4379 2024-04-01 16:10:17.000000 cpop-28.0.4/pop/dirs.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.0.4/pop/exc.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    21514 2024-04-01 20:11:42.000000 cpop-28.0.4/pop/hub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11789 2024-04-01 17:46:15.000000 cpop-28.0.4/pop/loader.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:00:43.323643 cpop-28.0.4/pop/log/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4750 2024-04-01 16:10:17.000000 cpop-28.0.4/pop/log/async.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      491 2024-04-01 16:10:17.000000 cpop-28.0.4/pop/log/init.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:00:43.319643 cpop-28.0.4/pop/mods/
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:00:43.327643 cpop-28.0.4/pop/mods/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6077 2024-04-01 20:16:36.000000 cpop-28.0.4/pop/mods/pop/config.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.0.4/pop/mods/pop/contract.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.0.4/pop/mods/pop/dyne.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6985 2024-04-01 17:42:04.000000 cpop-28.0.4/pop/mods/pop/sub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.0.4/pop/mods/pop/test.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)   878107 2024-04-01 20:59:35.000000 cpop-28.0.4/pop/pop.data.c
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6101 2024-04-01 19:03:13.000000 cpop-28.0.4/pop/pop.data.pyx
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.0.4/pop/ref.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1321 2024-03-24 19:08:30.000000 cpop-28.0.4/pop/scanner.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.0.4/pop/verify.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1315 2024-04-01 21:00:35.000000 cpop-28.0.4/pyproject.toml
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-01 21:00:43.327643 cpop-28.0.4/setup.cfg
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1257 2024-04-01 20:59:31.000000 cpop-28.0.4/setup.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:05:50.841166 cpop-28.0.5/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.0.5/LICENSE
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      104 2024-04-01 20:54:49.000000 cpop-28.0.5/MANIFEST.in
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 21:05:50.841166 cpop-28.0.5/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4063 2024-04-01 20:42:25.000000 cpop-28.0.5/README.rst
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:05:50.837166 cpop-28.0.5/cpop.egg-info/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 21:05:50.000000 cpop-28.0.5/cpop.egg-info/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      527 2024-04-01 21:05:50.000000 cpop-28.0.5/cpop.egg-info/SOURCES.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-01 21:05:50.000000 cpop-28.0.5/cpop.egg-info/dependency_links.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-01 21:05:50.000000 cpop-28.0.5/cpop.egg-info/entry_points.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      128 2024-04-01 21:05:50.000000 cpop-28.0.5/cpop.egg-info/requires.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       13 2024-04-01 21:05:50.000000 cpop-28.0.5/cpop.egg-info/top_level.txt
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:05:50.837166 cpop-28.0.5/hub/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.0.5/hub/__init__.py
+-rwxrwxr-x   0 akmod     (1000) akmod     (1000)     1979 2024-04-01 18:01:36.000000 cpop-28.0.5/hub/__main__.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:05:50.841166 cpop-28.0.5/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    10888 2024-04-01 16:10:17.000000 cpop-28.0.5/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)   870672 2024-04-01 21:05:40.000000 cpop-28.0.5/pop/data.c
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6101 2024-04-01 19:03:13.000000 cpop-28.0.5/pop/data.pyx
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4379 2024-04-01 16:10:17.000000 cpop-28.0.5/pop/dirs.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.0.5/pop/exc.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    21514 2024-04-01 20:11:42.000000 cpop-28.0.5/pop/hub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11789 2024-04-01 17:46:15.000000 cpop-28.0.5/pop/loader.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:05:50.841166 cpop-28.0.5/pop/log/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4750 2024-04-01 16:10:17.000000 cpop-28.0.5/pop/log/async.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      491 2024-04-01 16:10:17.000000 cpop-28.0.5/pop/log/init.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:05:50.837166 cpop-28.0.5/pop/mods/
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:05:50.841166 cpop-28.0.5/pop/mods/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6077 2024-04-01 20:16:36.000000 cpop-28.0.5/pop/mods/pop/config.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.0.5/pop/mods/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.0.5/pop/mods/pop/dyne.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6985 2024-04-01 17:42:04.000000 cpop-28.0.5/pop/mods/pop/sub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.0.5/pop/mods/pop/test.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.0.5/pop/ref.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1321 2024-03-24 19:08:30.000000 cpop-28.0.5/pop/scanner.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.0.5/pop/verify.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1315 2024-04-01 21:02:28.000000 cpop-28.0.5/pyproject.toml
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-01 21:05:50.841166 cpop-28.0.5/setup.cfg
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1260 2024-04-01 21:04:14.000000 cpop-28.0.5/setup.py
```

### Comparing `cpop-28.0.4/LICENSE` & `cpop-28.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cpop-28.0.4/PKG-INFO` & `cpop-28.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.0.4
+Version: 28.0.5
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cpop-28.0.4/README.rst` & `cpop-28.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-28.0.4/cpop.egg-info/PKG-INFO` & `cpop-28.0.5/cpop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.0.4
+Version: 28.0.5
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cpop-28.0.4/cpop.egg-info/SOURCES.txt` & `cpop-28.0.5/cpop.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 cpop.egg-info/dependency_links.txt
 cpop.egg-info/entry_points.txt
 cpop.egg-info/requires.txt
 cpop.egg-info/top_level.txt
 hub/__init__.py
 hub/__main__.py
 pop/contract.py
+pop/data.c
+pop/data.pyx
 pop/dirs.py
 pop/exc.py
 pop/hub.py
 pop/loader.py
-pop/pop.data.c
-pop/pop.data.pyx
 pop/ref.py
 pop/scanner.py
 pop/verify.py
 pop/log/async.py
 pop/log/init.py
 pop/mods/pop/config.py
 pop/mods/pop/contract.py
```

### Comparing `cpop-28.0.4/hub/__main__.py` & `cpop-28.0.5/hub/__main__.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.4/pop/contract.py` & `cpop-28.0.5/pop/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.4/pop/dirs.py` & `cpop-28.0.5/pop/dirs.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.4/pop/exc.py` & `cpop-28.0.5/pop/exc.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.4/pop/hub.py` & `cpop-28.0.5/pop/hub.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.4/pop/loader.py` & `cpop-28.0.5/pop/loader.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.4/pop/log/async.py` & `cpop-28.0.5/pop/log/async.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.4/pop/mods/pop/config.py` & `cpop-28.0.5/pop/mods/pop/config.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.4/pop/mods/pop/contract.py` & `cpop-28.0.5/pop/mods/pop/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.4/pop/mods/pop/sub.py` & `cpop-28.0.5/pop/mods/pop/sub.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.4/pop/mods/pop/test.py` & `cpop-28.0.5/pop/mods/pop/test.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.4/pop/pop.data.c` & `cpop-28.0.5/pop/data.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
-        "name": "pop.data",
+        "name": "data",
         "sources": [
-            "pop/pop.data.pyx"
+            "pop/data.pyx"
         ]
     },
-    "module_name": "pop.data"
+    "module_name": "data"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
@@ -1242,16 +1242,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__pop__data
-#define __PYX_HAVE_API__pop__data
+#define __PYX_HAVE__data
+#define __PYX_HAVE_API__data
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include <stddef.h>
 #include "pythread.h"
 #ifdef _OPENMP
 #include <omp.h>
@@ -1497,15 +1497,15 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "pop/pop.data.pyx",
+  "pop/data.pyx",
   "contextvars.pxd",
   "<stringsource>",
   "type.pxd",
   "bool.pxd",
   "complex.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
@@ -1515,21 +1515,21 @@
 #endif
 
 /* #### Code section: numeric_typedefs ### */
 /* #### Code section: complex_type_declarations ### */
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
-struct __pyx_obj_3pop_4data_NamespaceDict;
-struct __pyx_obj_3pop_4data_MultidictCache;
-struct __pyx_obj_3pop_4data_ImmutableNamespaceDict;
-struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__;
-struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr;
-struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr;
-struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr;
+struct __pyx_obj_4data_NamespaceDict;
+struct __pyx_obj_4data_MultidictCache;
+struct __pyx_obj_4data_ImmutableNamespaceDict;
+struct __pyx_obj_4data___pyx_scope_struct____contains__;
+struct __pyx_obj_4data___pyx_scope_struct_1_genexpr;
+struct __pyx_obj_4data___pyx_scope_struct_2_genexpr;
+struct __pyx_obj_4data___pyx_scope_struct_3_genexpr;
 struct __pyx_opt_args_7cpython_11contextvars_get_value;
 struct __pyx_opt_args_7cpython_11contextvars_get_value_no_default;
 
 /* "cpython/contextvars.pxd":112
  * 
  * 
  * cdef inline object get_value(var, default_value=None):             # <<<<<<<<<<<<<<
@@ -1548,145 +1548,145 @@
  *     """Return a new reference to the value of the context variable,
  *     or the provided default value if no such value was found.
  */
 struct __pyx_opt_args_7cpython_11contextvars_get_value_no_default {
   int __pyx_n;
   PyObject *default_value;
 };
-struct __pyx_opt_args_3pop_4data_update;
+struct __pyx_opt_args_4data_update;
 
-/* "pop/pop.data.pyx":166
+/* "data.pyx":166
  * 
  * 
  * cpdef update(dest, upd, bint recursive_update=True, bint merge_lists=False):             # <<<<<<<<<<<<<<
  *     """
  *     Recursive version of the default dict.update
  */
-struct __pyx_opt_args_3pop_4data_update {
+struct __pyx_opt_args_4data_update {
   int __pyx_n;
   int recursive_update;
   int merge_lists;
 };
 
-/* "pop/pop.data.pyx":11
+/* "data.pyx":11
  * cdef frozenset DICT_ATTRS = frozenset(dir(dict))
  * 
  * cdef class NamespaceDict(dict[str, object]):             # <<<<<<<<<<<<<<
  *     def __getattr__(self, key: str):
  *         if key.startswith("__") and key.endswith("__"):
  */
-struct __pyx_obj_3pop_4data_NamespaceDict {
+struct __pyx_obj_4data_NamespaceDict {
   PyDictObject __pyx_base;
 };
 
 
-/* "pop/pop.data.pyx":26
+/* "data.pyx":26
  * 
  * 
  * cdef class MultidictCache:             # <<<<<<<<<<<<<<
  *     cdef dict[str, object] _cache
  *     cdef list[dict[str, object]] _base_dicts
  */
-struct __pyx_obj_3pop_4data_MultidictCache {
+struct __pyx_obj_4data_MultidictCache {
   PyObject_HEAD
-  struct __pyx_vtabstruct_3pop_4data_MultidictCache *__pyx_vtab;
+  struct __pyx_vtabstruct_4data_MultidictCache *__pyx_vtab;
   PyObject *_cache;
   PyObject *_base_dicts;
   PyObject *_split_cache;
 };
 
 
-/* "pop/pop.data.pyx":68
+/* "data.pyx":68
  *         return any(item in base_dict for base_dict in self._base_dicts)
  * 
  * cdef class ImmutableNamespaceDict:             # <<<<<<<<<<<<<<
  *     cdef readonly dict __data
  * 
  */
-struct __pyx_obj_3pop_4data_ImmutableNamespaceDict {
+struct __pyx_obj_4data_ImmutableNamespaceDict {
   PyObject_HEAD
   PyObject *_ImmutableNamespaceDict__data;
 };
 
 
-/* "pop/pop.data.pyx":65
+/* "data.pyx":65
  *         return iter({k for base_dict in self._base_dicts for k in base_dict})
  * 
  *     def __contains__(self, item):             # <<<<<<<<<<<<<<
  *         return any(item in base_dict for base_dict in self._base_dicts)
  * 
  */
-struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__ {
+struct __pyx_obj_4data___pyx_scope_struct____contains__ {
   PyObject_HEAD
   PyObject *__pyx_v_item;
 };
 
 
-/* "pop/pop.data.pyx":66
+/* "data.pyx":66
  * 
  *     def __contains__(self, item):
  *         return any(item in base_dict for base_dict in self._base_dicts)             # <<<<<<<<<<<<<<
  * 
  * cdef class ImmutableNamespaceDict:
  */
-struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr {
+struct __pyx_obj_4data___pyx_scope_struct_1_genexpr {
   PyObject_HEAD
-  struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__ *__pyx_outer_scope;
+  struct __pyx_obj_4data___pyx_scope_struct____contains__ *__pyx_outer_scope;
   PyObject *__pyx_genexpr_arg_0;
   PyObject *__pyx_v_base_dict;
 };
 
 
-/* "pop/pop.data.pyx":149
+/* "data.pyx":149
  *         return ImmutableNamespaceDict({key: freeze(value) for key, value in data.items()})
  *     elif isinstance(data, list):
  *         return tuple(freeze(value) for value in data)             # <<<<<<<<<<<<<<
  *     elif isinstance(data, set):
  *         return frozenset(freeze(value) for value in data)
  */
-struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr {
+struct __pyx_obj_4data___pyx_scope_struct_2_genexpr {
   PyObject_HEAD
   PyObject *__pyx_genexpr_arg_0;
   PyObject *__pyx_v_value;
   PyObject *__pyx_t_0;
   Py_ssize_t __pyx_t_1;
   PyObject *(*__pyx_t_2)(PyObject *);
 };
 
 
-/* "pop/pop.data.pyx":151
+/* "data.pyx":151
  *         return tuple(freeze(value) for value in data)
  *     elif isinstance(data, set):
  *         return frozenset(freeze(value) for value in data)             # <<<<<<<<<<<<<<
  *     else:
  *         return data
  */
-struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr {
+struct __pyx_obj_4data___pyx_scope_struct_3_genexpr {
   PyObject_HEAD
   PyObject *__pyx_genexpr_arg_0;
   PyObject *__pyx_v_value;
   PyObject *__pyx_t_0;
   Py_ssize_t __pyx_t_1;
   PyObject *(*__pyx_t_2)(PyObject *);
 };
 
 
 
-/* "pop/pop.data.pyx":26
+/* "data.pyx":26
  * 
  * 
  * cdef class MultidictCache:             # <<<<<<<<<<<<<<
  *     cdef dict[str, object] _cache
  *     cdef list[dict[str, object]] _base_dicts
  */
 
-struct __pyx_vtabstruct_3pop_4data_MultidictCache {
-  PyObject *(*_clear)(struct __pyx_obj_3pop_4data_MultidictCache *, int __pyx_skip_dispatch);
+struct __pyx_vtabstruct_4data_MultidictCache {
+  PyObject *(*_clear)(struct __pyx_obj_4data_MultidictCache *, int __pyx_skip_dispatch);
 };
-static struct __pyx_vtabstruct_3pop_4data_MultidictCache *__pyx_vtabptr_3pop_4data_MultidictCache;
+static struct __pyx_vtabstruct_4data_MultidictCache *__pyx_vtabptr_4data_MultidictCache;
 /* #### Code section: utility_code_proto ### */
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
@@ -2667,15 +2667,15 @@
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4real_real(PyComplexObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4imag_imag(PyComplexObject *__pyx_v_self); /* proto*/
-static PyObject *__pyx_f_3pop_4data_14MultidictCache__clear(struct __pyx_obj_3pop_4data_MultidictCache *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
+static PyObject *__pyx_f_4data_14MultidictCache__clear(struct __pyx_obj_4data_MultidictCache *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
 
 /* Module declarations from "cpython.version" */
 
 /* Module declarations from "__builtin__" */
 
 /* Module declarations from "cpython.type" */
 
@@ -2755,27 +2755,27 @@
 
 /* Module declarations from "cpython.pycapsule" */
 
 /* Module declarations from "cpython.contextvars" */
 
 /* Module declarations from "cpython" */
 
-/* Module declarations from "pop.data" */
-static PyObject *__pyx_v_3pop_4data_DICT_ATTRS = 0;
-static PyObject *__pyx_f_3pop_4data_update(PyObject *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_3pop_4data_update *__pyx_optional_args); /*proto*/
-static PyObject *__pyx_f_3pop_4data___pyx_unpickle_NamespaceDict__set_state(struct __pyx_obj_3pop_4data_NamespaceDict *, PyObject *); /*proto*/
-static PyObject *__pyx_f_3pop_4data___pyx_unpickle_MultidictCache__set_state(struct __pyx_obj_3pop_4data_MultidictCache *, PyObject *); /*proto*/
-static PyObject *__pyx_f_3pop_4data___pyx_unpickle_ImmutableNamespaceDict__set_state(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *, PyObject *); /*proto*/
+/* Module declarations from "data" */
+static PyObject *__pyx_v_4data_DICT_ATTRS = 0;
+static PyObject *__pyx_f_4data_update(PyObject *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_4data_update *__pyx_optional_args); /*proto*/
+static PyObject *__pyx_f_4data___pyx_unpickle_NamespaceDict__set_state(struct __pyx_obj_4data_NamespaceDict *, PyObject *); /*proto*/
+static PyObject *__pyx_f_4data___pyx_unpickle_MultidictCache__set_state(struct __pyx_obj_4data_MultidictCache *, PyObject *); /*proto*/
+static PyObject *__pyx_f_4data___pyx_unpickle_ImmutableNamespaceDict__set_state(struct __pyx_obj_4data_ImmutableNamespaceDict *, PyObject *); /*proto*/
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
-#define __Pyx_MODULE_NAME "pop.data"
-extern int __pyx_module_is_main_pop__data;
-int __pyx_module_is_main_pop__data = 0;
+#define __Pyx_MODULE_NAME "data"
+extern int __pyx_module_is_main_data;
+int __pyx_module_is_main_data = 0;
 
-/* Implementation of "pop.data" */
+/* Implementation of "data" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_KeyError;
 static PyObject *__pyx_builtin_AttributeError;
 static PyObject *__pyx_builtin_object;
 static PyObject *__pyx_builtin_TypeError;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_[] = "__";
@@ -2819,41 +2819,40 @@
 static const char __pyx_k_Mapping[] = "Mapping";
 static const char __pyx_k_default[] = "default";
 static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_genexpr[] = "genexpr";
 static const char __pyx_k_setattr[] = "__setattr__";
 static const char __pyx_k_KeyError[] = "KeyError";
 static const char __pyx_k_getstate[] = "__getstate__";
-static const char __pyx_k_pop_data[] = "pop.data";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_unfreeze[] = "unfreeze";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_base_dicts[] = "base_dicts";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_merge_lists[] = "merge_lists";
 static const char __pyx_k_getattribute[] = "__getattribute__";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
+static const char __pyx_k_pop_data_pyx[] = "pop/data.pyx";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "<stringsource>";
 static const char __pyx_k_use_setstate[] = "use_setstate";
 static const char __pyx_k_NamespaceDict[] = "NamespaceDict";
 static const char __pyx_k_class_getitem[] = "__class_getitem__";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_AttributeError[] = "AttributeError";
 static const char __pyx_k_MultidictCache[] = "MultidictCache";
 static const char __pyx_k_collections_abc[] = "collections.abc";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
-static const char __pyx_k_pop_pop_data_pyx[] = "pop/pop.data.pyx";
 static const char __pyx_k_recursive_update[] = "recursive_update";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_MultidictCache__clear[] = "MultidictCache._clear";
 static const char __pyx_k_freeze_locals_genexpr[] = "freeze.<locals>.genexpr";
 static const char __pyx_k_ImmutableNamespaceDict[] = "ImmutableNamespaceDict";
 static const char __pyx_k_object_has_no_attribute[] = "' object has no attribute '";
@@ -2876,61 +2875,61 @@
 static const char __pyx_k_ImmutableNamespaceDict___setstat[] = "ImmutableNamespaceDict.__setstate_cython__";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xe3b0c44, 0xda39a3e, 0xd41d8cd) = ())";
 static const char __pyx_k_MultidictCache___setstate_cython[] = "MultidictCache.__setstate_cython__";
 static const char __pyx_k_ImmutableNamespaceDict_does_not_2[] = "ImmutableNamespaceDict does not support item assignment";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_2[] = "Incompatible checksums (0x%x vs (0x09e6f20, 0xf4b8e03, 0xd271b3e) = (_base_dicts, _cache, _split_cache))";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_3[] = "Incompatible checksums (0x%x vs (0x9077974, 0xccb23f1, 0x45e2a8b) = (_ImmutableNamespaceDict__data))";
 /* #### Code section: decls ### */
-static PyObject *__pyx_pf_3pop_4data_13NamespaceDict___getattr__(struct __pyx_obj_3pop_4data_NamespaceDict *__pyx_v_self, PyObject *__pyx_v_key); /* proto */
-static int __pyx_pf_3pop_4data_13NamespaceDict_2__setattr__(struct __pyx_obj_3pop_4data_NamespaceDict *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value); /* proto */
-static PyObject *__pyx_pf_3pop_4data_13NamespaceDict_4__reduce_cython__(struct __pyx_obj_3pop_4data_NamespaceDict *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_3pop_4data_13NamespaceDict_6__setstate_cython__(struct __pyx_obj_3pop_4data_NamespaceDict *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
-static int __pyx_pf_3pop_4data_14MultidictCache___init__(struct __pyx_obj_3pop_4data_MultidictCache *__pyx_v_self, PyObject *__pyx_v_base_dicts); /* proto */
-static PyObject *__pyx_pf_3pop_4data_14MultidictCache_2_clear(struct __pyx_obj_3pop_4data_MultidictCache *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_3pop_4data_14MultidictCache_4__getitem__(struct __pyx_obj_3pop_4data_MultidictCache *__pyx_v_self, PyObject *__pyx_v_key); /* proto */
-static PyObject *__pyx_pf_3pop_4data_14MultidictCache_6__iter__(struct __pyx_obj_3pop_4data_MultidictCache *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_3pop_4data_14MultidictCache_12__contains___genexpr(PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0); /* proto */
-static int __pyx_pf_3pop_4data_14MultidictCache_8__contains__(struct __pyx_obj_3pop_4data_MultidictCache *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
-static PyObject *__pyx_pf_3pop_4data_14MultidictCache_10__reduce_cython__(struct __pyx_obj_3pop_4data_MultidictCache *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_3pop_4data_14MultidictCache_12__setstate_cython__(struct __pyx_obj_3pop_4data_MultidictCache *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
-static int __pyx_pf_3pop_4data_22ImmutableNamespaceDict___init__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_data); /* proto */
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_2__getitem__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key); /* proto */
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_4__getattr__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key); /* proto */
-static int __pyx_pf_3pop_4data_22ImmutableNamespaceDict_6__setattr__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value); /* proto */
-static int __pyx_pf_3pop_4data_22ImmutableNamespaceDict_8__setitem__(CYTHON_UNUSED struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_key, CYTHON_UNUSED PyObject *__pyx_v_value); /* proto */
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_10__call__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
-static Py_ssize_t __pyx_pf_3pop_4data_22ImmutableNamespaceDict_12__len__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_14__iter__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
-static int __pyx_pf_3pop_4data_22ImmutableNamespaceDict_16__bool__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
-static int __pyx_pf_3pop_4data_22ImmutableNamespaceDict_18__contains__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key); /* proto */
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_20__repr__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_22__eq__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_24__ne__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_26keys(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_28values(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_30items(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_32get(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_default); /* proto */
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_34copy(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_29_ImmutableNamespaceDict__data___get__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_36__reduce_cython__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_38__setstate_cython__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_3pop_4data_6freeze_genexpr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0); /* proto */
-static PyObject *__pyx_pf_3pop_4data_6freeze_3genexpr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0); /* proto */
-static PyObject *__pyx_pf_3pop_4data_freeze(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data); /* proto */
-static PyObject *__pyx_pf_3pop_4data_2unfreeze(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data); /* proto */
-static PyObject *__pyx_pf_3pop_4data_4update(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dest, PyObject *__pyx_v_upd, int __pyx_v_recursive_update, int __pyx_v_merge_lists); /* proto */
-static PyObject *__pyx_pf_3pop_4data_6__pyx_unpickle_NamespaceDict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_3pop_4data_8__pyx_unpickle_MultidictCache(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_3pop_4data_10__pyx_unpickle_ImmutableNamespaceDict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_tp_new_3pop_4data_MultidictCache(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_3pop_4data_ImmutableNamespaceDict(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_3pop_4data___pyx_scope_struct____contains__(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_3pop_4data___pyx_scope_struct_1_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_3pop_4data___pyx_scope_struct_2_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_3pop_4data___pyx_scope_struct_3_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_pf_4data_13NamespaceDict___getattr__(struct __pyx_obj_4data_NamespaceDict *__pyx_v_self, PyObject *__pyx_v_key); /* proto */
+static int __pyx_pf_4data_13NamespaceDict_2__setattr__(struct __pyx_obj_4data_NamespaceDict *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_4data_13NamespaceDict_4__reduce_cython__(struct __pyx_obj_4data_NamespaceDict *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_4data_13NamespaceDict_6__setstate_cython__(struct __pyx_obj_4data_NamespaceDict *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static int __pyx_pf_4data_14MultidictCache___init__(struct __pyx_obj_4data_MultidictCache *__pyx_v_self, PyObject *__pyx_v_base_dicts); /* proto */
+static PyObject *__pyx_pf_4data_14MultidictCache_2_clear(struct __pyx_obj_4data_MultidictCache *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_4data_14MultidictCache_4__getitem__(struct __pyx_obj_4data_MultidictCache *__pyx_v_self, PyObject *__pyx_v_key); /* proto */
+static PyObject *__pyx_pf_4data_14MultidictCache_6__iter__(struct __pyx_obj_4data_MultidictCache *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_4data_14MultidictCache_12__contains___genexpr(PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0); /* proto */
+static int __pyx_pf_4data_14MultidictCache_8__contains__(struct __pyx_obj_4data_MultidictCache *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
+static PyObject *__pyx_pf_4data_14MultidictCache_10__reduce_cython__(struct __pyx_obj_4data_MultidictCache *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_4data_14MultidictCache_12__setstate_cython__(struct __pyx_obj_4data_MultidictCache *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static int __pyx_pf_4data_22ImmutableNamespaceDict___init__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_data); /* proto */
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_2__getitem__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key); /* proto */
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_4__getattr__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key); /* proto */
+static int __pyx_pf_4data_22ImmutableNamespaceDict_6__setattr__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value); /* proto */
+static int __pyx_pf_4data_22ImmutableNamespaceDict_8__setitem__(CYTHON_UNUSED struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_key, CYTHON_UNUSED PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_10__call__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
+static Py_ssize_t __pyx_pf_4data_22ImmutableNamespaceDict_12__len__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_14__iter__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
+static int __pyx_pf_4data_22ImmutableNamespaceDict_16__bool__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
+static int __pyx_pf_4data_22ImmutableNamespaceDict_18__contains__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key); /* proto */
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_20__repr__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_22__eq__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_24__ne__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_26keys(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_28values(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_30items(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_32get(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_default); /* proto */
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_34copy(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_29_ImmutableNamespaceDict__data___get__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_36__reduce_cython__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_38__setstate_cython__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_4data_6freeze_genexpr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0); /* proto */
+static PyObject *__pyx_pf_4data_6freeze_3genexpr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0); /* proto */
+static PyObject *__pyx_pf_4data_freeze(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data); /* proto */
+static PyObject *__pyx_pf_4data_2unfreeze(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data); /* proto */
+static PyObject *__pyx_pf_4data_4update(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dest, PyObject *__pyx_v_upd, int __pyx_v_recursive_update, int __pyx_v_merge_lists); /* proto */
+static PyObject *__pyx_pf_4data_6__pyx_unpickle_NamespaceDict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_4data_8__pyx_unpickle_MultidictCache(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_4data_10__pyx_unpickle_ImmutableNamespaceDict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_tp_new_4data_MultidictCache(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_4data_ImmutableNamespaceDict(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_4data___pyx_scope_struct____contains__(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_4data___pyx_scope_struct_1_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_4data___pyx_scope_struct_2_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_4data___pyx_scope_struct_3_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_get = {0, 0, 0, 0, 0};
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_items = {0, 0, 0, 0, 0};
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_keys = {0, 0, 0, 0, 0};
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_values = {0, 0, 0, 0, 0};
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
@@ -3044,29 +3043,29 @@
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
-  PyObject *__pyx_type_3pop_4data_NamespaceDict;
-  PyObject *__pyx_type_3pop_4data_MultidictCache;
-  PyObject *__pyx_type_3pop_4data_ImmutableNamespaceDict;
-  PyObject *__pyx_type_3pop_4data___pyx_scope_struct____contains__;
-  PyObject *__pyx_type_3pop_4data___pyx_scope_struct_1_genexpr;
-  PyObject *__pyx_type_3pop_4data___pyx_scope_struct_2_genexpr;
-  PyObject *__pyx_type_3pop_4data___pyx_scope_struct_3_genexpr;
-  #endif
-  PyTypeObject *__pyx_ptype_3pop_4data_NamespaceDict;
-  PyTypeObject *__pyx_ptype_3pop_4data_MultidictCache;
-  PyTypeObject *__pyx_ptype_3pop_4data_ImmutableNamespaceDict;
-  PyTypeObject *__pyx_ptype_3pop_4data___pyx_scope_struct____contains__;
-  PyTypeObject *__pyx_ptype_3pop_4data___pyx_scope_struct_1_genexpr;
-  PyTypeObject *__pyx_ptype_3pop_4data___pyx_scope_struct_2_genexpr;
-  PyTypeObject *__pyx_ptype_3pop_4data___pyx_scope_struct_3_genexpr;
+  PyObject *__pyx_type_4data_NamespaceDict;
+  PyObject *__pyx_type_4data_MultidictCache;
+  PyObject *__pyx_type_4data_ImmutableNamespaceDict;
+  PyObject *__pyx_type_4data___pyx_scope_struct____contains__;
+  PyObject *__pyx_type_4data___pyx_scope_struct_1_genexpr;
+  PyObject *__pyx_type_4data___pyx_scope_struct_2_genexpr;
+  PyObject *__pyx_type_4data___pyx_scope_struct_3_genexpr;
+  #endif
+  PyTypeObject *__pyx_ptype_4data_NamespaceDict;
+  PyTypeObject *__pyx_ptype_4data_MultidictCache;
+  PyTypeObject *__pyx_ptype_4data_ImmutableNamespaceDict;
+  PyTypeObject *__pyx_ptype_4data___pyx_scope_struct____contains__;
+  PyTypeObject *__pyx_ptype_4data___pyx_scope_struct_1_genexpr;
+  PyTypeObject *__pyx_ptype_4data___pyx_scope_struct_2_genexpr;
+  PyTypeObject *__pyx_ptype_4data___pyx_scope_struct_3_genexpr;
   PyObject *__pyx_n_u_;
   PyObject *__pyx_n_s_AttributeError;
   PyObject *__pyx_n_s_ImmutableNamespaceDict;
   PyObject *__pyx_n_s_ImmutableNamespaceDict___reduce;
   PyObject *__pyx_n_s_ImmutableNamespaceDict___setstat;
   PyObject *__pyx_n_s_ImmutableNamespaceDict__data;
   PyObject *__pyx_n_u_ImmutableNamespaceDict__data;
@@ -3131,16 +3130,15 @@
   PyObject *__pyx_n_s_merge_lists;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_new;
   PyObject *__pyx_kp_u_not_found_in_any_base_dictionar;
   PyObject *__pyx_n_s_object;
   PyObject *__pyx_kp_u_object_has_no_attribute;
   PyObject *__pyx_n_s_pickle;
-  PyObject *__pyx_n_s_pop_data;
-  PyObject *__pyx_kp_s_pop_pop_data_pyx;
+  PyObject *__pyx_kp_s_pop_data_pyx;
   PyObject *__pyx_n_s_pyx_PickleError;
   PyObject *__pyx_n_s_pyx_checksum;
   PyObject *__pyx_n_s_pyx_result;
   PyObject *__pyx_n_s_pyx_state;
   PyObject *__pyx_n_s_pyx_type;
   PyObject *__pyx_n_s_pyx_unpickle_ImmutableNamespac;
   PyObject *__pyx_n_s_pyx_unpickle_MultidictCache;
@@ -3249,28 +3247,28 @@
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
   Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_4type_type);
   Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_4bool_bool);
   Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_7complex_complex);
-  Py_CLEAR(clear_module_state->__pyx_ptype_3pop_4data_NamespaceDict);
-  Py_CLEAR(clear_module_state->__pyx_type_3pop_4data_NamespaceDict);
-  Py_CLEAR(clear_module_state->__pyx_ptype_3pop_4data_MultidictCache);
-  Py_CLEAR(clear_module_state->__pyx_type_3pop_4data_MultidictCache);
-  Py_CLEAR(clear_module_state->__pyx_ptype_3pop_4data_ImmutableNamespaceDict);
-  Py_CLEAR(clear_module_state->__pyx_type_3pop_4data_ImmutableNamespaceDict);
-  Py_CLEAR(clear_module_state->__pyx_ptype_3pop_4data___pyx_scope_struct____contains__);
-  Py_CLEAR(clear_module_state->__pyx_type_3pop_4data___pyx_scope_struct____contains__);
-  Py_CLEAR(clear_module_state->__pyx_ptype_3pop_4data___pyx_scope_struct_1_genexpr);
-  Py_CLEAR(clear_module_state->__pyx_type_3pop_4data___pyx_scope_struct_1_genexpr);
-  Py_CLEAR(clear_module_state->__pyx_ptype_3pop_4data___pyx_scope_struct_2_genexpr);
-  Py_CLEAR(clear_module_state->__pyx_type_3pop_4data___pyx_scope_struct_2_genexpr);
-  Py_CLEAR(clear_module_state->__pyx_ptype_3pop_4data___pyx_scope_struct_3_genexpr);
-  Py_CLEAR(clear_module_state->__pyx_type_3pop_4data___pyx_scope_struct_3_genexpr);
+  Py_CLEAR(clear_module_state->__pyx_ptype_4data_NamespaceDict);
+  Py_CLEAR(clear_module_state->__pyx_type_4data_NamespaceDict);
+  Py_CLEAR(clear_module_state->__pyx_ptype_4data_MultidictCache);
+  Py_CLEAR(clear_module_state->__pyx_type_4data_MultidictCache);
+  Py_CLEAR(clear_module_state->__pyx_ptype_4data_ImmutableNamespaceDict);
+  Py_CLEAR(clear_module_state->__pyx_type_4data_ImmutableNamespaceDict);
+  Py_CLEAR(clear_module_state->__pyx_ptype_4data___pyx_scope_struct____contains__);
+  Py_CLEAR(clear_module_state->__pyx_type_4data___pyx_scope_struct____contains__);
+  Py_CLEAR(clear_module_state->__pyx_ptype_4data___pyx_scope_struct_1_genexpr);
+  Py_CLEAR(clear_module_state->__pyx_type_4data___pyx_scope_struct_1_genexpr);
+  Py_CLEAR(clear_module_state->__pyx_ptype_4data___pyx_scope_struct_2_genexpr);
+  Py_CLEAR(clear_module_state->__pyx_type_4data___pyx_scope_struct_2_genexpr);
+  Py_CLEAR(clear_module_state->__pyx_ptype_4data___pyx_scope_struct_3_genexpr);
+  Py_CLEAR(clear_module_state->__pyx_type_4data___pyx_scope_struct_3_genexpr);
   Py_CLEAR(clear_module_state->__pyx_n_u_);
   Py_CLEAR(clear_module_state->__pyx_n_s_AttributeError);
   Py_CLEAR(clear_module_state->__pyx_n_s_ImmutableNamespaceDict);
   Py_CLEAR(clear_module_state->__pyx_n_s_ImmutableNamespaceDict___reduce);
   Py_CLEAR(clear_module_state->__pyx_n_s_ImmutableNamespaceDict___setstat);
   Py_CLEAR(clear_module_state->__pyx_n_s_ImmutableNamespaceDict__data);
   Py_CLEAR(clear_module_state->__pyx_n_u_ImmutableNamespaceDict__data);
@@ -3335,16 +3333,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_merge_lists);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_new);
   Py_CLEAR(clear_module_state->__pyx_kp_u_not_found_in_any_base_dictionar);
   Py_CLEAR(clear_module_state->__pyx_n_s_object);
   Py_CLEAR(clear_module_state->__pyx_kp_u_object_has_no_attribute);
   Py_CLEAR(clear_module_state->__pyx_n_s_pickle);
-  Py_CLEAR(clear_module_state->__pyx_n_s_pop_data);
-  Py_CLEAR(clear_module_state->__pyx_kp_s_pop_pop_data_pyx);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_pop_data_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_checksum);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_result);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_unpickle_ImmutableNamespac);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_unpickle_MultidictCache);
@@ -3431,28 +3428,28 @@
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
   Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_4type_type);
   Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_4bool_bool);
   Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_7complex_complex);
-  Py_VISIT(traverse_module_state->__pyx_ptype_3pop_4data_NamespaceDict);
-  Py_VISIT(traverse_module_state->__pyx_type_3pop_4data_NamespaceDict);
-  Py_VISIT(traverse_module_state->__pyx_ptype_3pop_4data_MultidictCache);
-  Py_VISIT(traverse_module_state->__pyx_type_3pop_4data_MultidictCache);
-  Py_VISIT(traverse_module_state->__pyx_ptype_3pop_4data_ImmutableNamespaceDict);
-  Py_VISIT(traverse_module_state->__pyx_type_3pop_4data_ImmutableNamespaceDict);
-  Py_VISIT(traverse_module_state->__pyx_ptype_3pop_4data___pyx_scope_struct____contains__);
-  Py_VISIT(traverse_module_state->__pyx_type_3pop_4data___pyx_scope_struct____contains__);
-  Py_VISIT(traverse_module_state->__pyx_ptype_3pop_4data___pyx_scope_struct_1_genexpr);
-  Py_VISIT(traverse_module_state->__pyx_type_3pop_4data___pyx_scope_struct_1_genexpr);
-  Py_VISIT(traverse_module_state->__pyx_ptype_3pop_4data___pyx_scope_struct_2_genexpr);
-  Py_VISIT(traverse_module_state->__pyx_type_3pop_4data___pyx_scope_struct_2_genexpr);
-  Py_VISIT(traverse_module_state->__pyx_ptype_3pop_4data___pyx_scope_struct_3_genexpr);
-  Py_VISIT(traverse_module_state->__pyx_type_3pop_4data___pyx_scope_struct_3_genexpr);
+  Py_VISIT(traverse_module_state->__pyx_ptype_4data_NamespaceDict);
+  Py_VISIT(traverse_module_state->__pyx_type_4data_NamespaceDict);
+  Py_VISIT(traverse_module_state->__pyx_ptype_4data_MultidictCache);
+  Py_VISIT(traverse_module_state->__pyx_type_4data_MultidictCache);
+  Py_VISIT(traverse_module_state->__pyx_ptype_4data_ImmutableNamespaceDict);
+  Py_VISIT(traverse_module_state->__pyx_type_4data_ImmutableNamespaceDict);
+  Py_VISIT(traverse_module_state->__pyx_ptype_4data___pyx_scope_struct____contains__);
+  Py_VISIT(traverse_module_state->__pyx_type_4data___pyx_scope_struct____contains__);
+  Py_VISIT(traverse_module_state->__pyx_ptype_4data___pyx_scope_struct_1_genexpr);
+  Py_VISIT(traverse_module_state->__pyx_type_4data___pyx_scope_struct_1_genexpr);
+  Py_VISIT(traverse_module_state->__pyx_ptype_4data___pyx_scope_struct_2_genexpr);
+  Py_VISIT(traverse_module_state->__pyx_type_4data___pyx_scope_struct_2_genexpr);
+  Py_VISIT(traverse_module_state->__pyx_ptype_4data___pyx_scope_struct_3_genexpr);
+  Py_VISIT(traverse_module_state->__pyx_type_4data___pyx_scope_struct_3_genexpr);
   Py_VISIT(traverse_module_state->__pyx_n_u_);
   Py_VISIT(traverse_module_state->__pyx_n_s_AttributeError);
   Py_VISIT(traverse_module_state->__pyx_n_s_ImmutableNamespaceDict);
   Py_VISIT(traverse_module_state->__pyx_n_s_ImmutableNamespaceDict___reduce);
   Py_VISIT(traverse_module_state->__pyx_n_s_ImmutableNamespaceDict___setstat);
   Py_VISIT(traverse_module_state->__pyx_n_s_ImmutableNamespaceDict__data);
   Py_VISIT(traverse_module_state->__pyx_n_u_ImmutableNamespaceDict__data);
@@ -3517,16 +3514,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_merge_lists);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_new);
   Py_VISIT(traverse_module_state->__pyx_kp_u_not_found_in_any_base_dictionar);
   Py_VISIT(traverse_module_state->__pyx_n_s_object);
   Py_VISIT(traverse_module_state->__pyx_kp_u_object_has_no_attribute);
   Py_VISIT(traverse_module_state->__pyx_n_s_pickle);
-  Py_VISIT(traverse_module_state->__pyx_n_s_pop_data);
-  Py_VISIT(traverse_module_state->__pyx_kp_s_pop_pop_data_pyx);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_pop_data_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_checksum);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_result);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_unpickle_ImmutableNamespac);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_unpickle_MultidictCache);
@@ -3708,29 +3704,29 @@
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
-#define __pyx_type_3pop_4data_NamespaceDict __pyx_mstate_global->__pyx_type_3pop_4data_NamespaceDict
-#define __pyx_type_3pop_4data_MultidictCache __pyx_mstate_global->__pyx_type_3pop_4data_MultidictCache
-#define __pyx_type_3pop_4data_ImmutableNamespaceDict __pyx_mstate_global->__pyx_type_3pop_4data_ImmutableNamespaceDict
-#define __pyx_type_3pop_4data___pyx_scope_struct____contains__ __pyx_mstate_global->__pyx_type_3pop_4data___pyx_scope_struct____contains__
-#define __pyx_type_3pop_4data___pyx_scope_struct_1_genexpr __pyx_mstate_global->__pyx_type_3pop_4data___pyx_scope_struct_1_genexpr
-#define __pyx_type_3pop_4data___pyx_scope_struct_2_genexpr __pyx_mstate_global->__pyx_type_3pop_4data___pyx_scope_struct_2_genexpr
-#define __pyx_type_3pop_4data___pyx_scope_struct_3_genexpr __pyx_mstate_global->__pyx_type_3pop_4data___pyx_scope_struct_3_genexpr
-#endif
-#define __pyx_ptype_3pop_4data_NamespaceDict __pyx_mstate_global->__pyx_ptype_3pop_4data_NamespaceDict
-#define __pyx_ptype_3pop_4data_MultidictCache __pyx_mstate_global->__pyx_ptype_3pop_4data_MultidictCache
-#define __pyx_ptype_3pop_4data_ImmutableNamespaceDict __pyx_mstate_global->__pyx_ptype_3pop_4data_ImmutableNamespaceDict
-#define __pyx_ptype_3pop_4data___pyx_scope_struct____contains__ __pyx_mstate_global->__pyx_ptype_3pop_4data___pyx_scope_struct____contains__
-#define __pyx_ptype_3pop_4data___pyx_scope_struct_1_genexpr __pyx_mstate_global->__pyx_ptype_3pop_4data___pyx_scope_struct_1_genexpr
-#define __pyx_ptype_3pop_4data___pyx_scope_struct_2_genexpr __pyx_mstate_global->__pyx_ptype_3pop_4data___pyx_scope_struct_2_genexpr
-#define __pyx_ptype_3pop_4data___pyx_scope_struct_3_genexpr __pyx_mstate_global->__pyx_ptype_3pop_4data___pyx_scope_struct_3_genexpr
+#define __pyx_type_4data_NamespaceDict __pyx_mstate_global->__pyx_type_4data_NamespaceDict
+#define __pyx_type_4data_MultidictCache __pyx_mstate_global->__pyx_type_4data_MultidictCache
+#define __pyx_type_4data_ImmutableNamespaceDict __pyx_mstate_global->__pyx_type_4data_ImmutableNamespaceDict
+#define __pyx_type_4data___pyx_scope_struct____contains__ __pyx_mstate_global->__pyx_type_4data___pyx_scope_struct____contains__
+#define __pyx_type_4data___pyx_scope_struct_1_genexpr __pyx_mstate_global->__pyx_type_4data___pyx_scope_struct_1_genexpr
+#define __pyx_type_4data___pyx_scope_struct_2_genexpr __pyx_mstate_global->__pyx_type_4data___pyx_scope_struct_2_genexpr
+#define __pyx_type_4data___pyx_scope_struct_3_genexpr __pyx_mstate_global->__pyx_type_4data___pyx_scope_struct_3_genexpr
+#endif
+#define __pyx_ptype_4data_NamespaceDict __pyx_mstate_global->__pyx_ptype_4data_NamespaceDict
+#define __pyx_ptype_4data_MultidictCache __pyx_mstate_global->__pyx_ptype_4data_MultidictCache
+#define __pyx_ptype_4data_ImmutableNamespaceDict __pyx_mstate_global->__pyx_ptype_4data_ImmutableNamespaceDict
+#define __pyx_ptype_4data___pyx_scope_struct____contains__ __pyx_mstate_global->__pyx_ptype_4data___pyx_scope_struct____contains__
+#define __pyx_ptype_4data___pyx_scope_struct_1_genexpr __pyx_mstate_global->__pyx_ptype_4data___pyx_scope_struct_1_genexpr
+#define __pyx_ptype_4data___pyx_scope_struct_2_genexpr __pyx_mstate_global->__pyx_ptype_4data___pyx_scope_struct_2_genexpr
+#define __pyx_ptype_4data___pyx_scope_struct_3_genexpr __pyx_mstate_global->__pyx_ptype_4data___pyx_scope_struct_3_genexpr
 #define __pyx_n_u_ __pyx_mstate_global->__pyx_n_u_
 #define __pyx_n_s_AttributeError __pyx_mstate_global->__pyx_n_s_AttributeError
 #define __pyx_n_s_ImmutableNamespaceDict __pyx_mstate_global->__pyx_n_s_ImmutableNamespaceDict
 #define __pyx_n_s_ImmutableNamespaceDict___reduce __pyx_mstate_global->__pyx_n_s_ImmutableNamespaceDict___reduce
 #define __pyx_n_s_ImmutableNamespaceDict___setstat __pyx_mstate_global->__pyx_n_s_ImmutableNamespaceDict___setstat
 #define __pyx_n_s_ImmutableNamespaceDict__data __pyx_mstate_global->__pyx_n_s_ImmutableNamespaceDict__data
 #define __pyx_n_u_ImmutableNamespaceDict__data __pyx_mstate_global->__pyx_n_u_ImmutableNamespaceDict__data
@@ -3795,16 +3791,15 @@
 #define __pyx_n_s_merge_lists __pyx_mstate_global->__pyx_n_s_merge_lists
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_new __pyx_mstate_global->__pyx_n_s_new
 #define __pyx_kp_u_not_found_in_any_base_dictionar __pyx_mstate_global->__pyx_kp_u_not_found_in_any_base_dictionar
 #define __pyx_n_s_object __pyx_mstate_global->__pyx_n_s_object
 #define __pyx_kp_u_object_has_no_attribute __pyx_mstate_global->__pyx_kp_u_object_has_no_attribute
 #define __pyx_n_s_pickle __pyx_mstate_global->__pyx_n_s_pickle
-#define __pyx_n_s_pop_data __pyx_mstate_global->__pyx_n_s_pop_data
-#define __pyx_kp_s_pop_pop_data_pyx __pyx_mstate_global->__pyx_kp_s_pop_pop_data_pyx
+#define __pyx_kp_s_pop_data_pyx __pyx_mstate_global->__pyx_kp_s_pop_data_pyx
 #define __pyx_n_s_pyx_PickleError __pyx_mstate_global->__pyx_n_s_pyx_PickleError
 #define __pyx_n_s_pyx_checksum __pyx_mstate_global->__pyx_n_s_pyx_checksum
 #define __pyx_n_s_pyx_result __pyx_mstate_global->__pyx_n_s_pyx_result
 #define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
 #define __pyx_n_s_pyx_type __pyx_mstate_global->__pyx_n_s_pyx_type
 #define __pyx_n_s_pyx_unpickle_ImmutableNamespac __pyx_mstate_global->__pyx_n_s_pyx_unpickle_ImmutableNamespac
 #define __pyx_n_s_pyx_unpickle_MultidictCache __pyx_mstate_global->__pyx_n_s_pyx_unpickle_MultidictCache
@@ -4163,46 +4158,46 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_pyvalue);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":12
+/* "data.pyx":12
  * 
  * cdef class NamespaceDict(dict[str, object]):
  *     def __getattr__(self, key: str):             # <<<<<<<<<<<<<<
  *         if key.startswith("__") and key.endswith("__"):
  *             self.__getattribute__(key)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_13NamespaceDict_1__getattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_key); /*proto*/
-static PyObject *__pyx_pw_3pop_4data_13NamespaceDict_1__getattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_key) {
+static PyObject *__pyx_pw_4data_13NamespaceDict_1__getattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_key); /*proto*/
+static PyObject *__pyx_pw_4data_13NamespaceDict_1__getattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_key) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__getattr__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyUnicode_Type), 0, "key", 1))) __PYX_ERR(0, 12, __pyx_L1_error)
-  __pyx_r = __pyx_pf_3pop_4data_13NamespaceDict___getattr__(((struct __pyx_obj_3pop_4data_NamespaceDict *)__pyx_v_self), ((PyObject*)__pyx_v_key));
+  __pyx_r = __pyx_pf_4data_13NamespaceDict___getattr__(((struct __pyx_obj_4data_NamespaceDict *)__pyx_v_self), ((PyObject*)__pyx_v_key));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_13NamespaceDict___getattr__(struct __pyx_obj_3pop_4data_NamespaceDict *__pyx_v_self, PyObject *__pyx_v_key) {
+static PyObject *__pyx_pf_4data_13NamespaceDict___getattr__(struct __pyx_obj_4data_NamespaceDict *__pyx_v_self, PyObject *__pyx_v_key) {
   PyObject *__pyx_v_e = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -4221,15 +4216,15 @@
   PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getattr__", 1);
 
-  /* "pop/pop.data.pyx":13
+  /* "data.pyx":13
  * cdef class NamespaceDict(dict[str, object]):
  *     def __getattr__(self, key: str):
  *         if key.startswith("__") and key.endswith("__"):             # <<<<<<<<<<<<<<
  *             self.__getattribute__(key)
  *         try:
  */
   __pyx_t_2 = __Pyx_PyUnicode_Tailmatch(__pyx_v_key, __pyx_n_u_, 0, PY_SSIZE_T_MAX, -1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 13, __pyx_L1_error)
@@ -4239,15 +4234,15 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = __Pyx_PyUnicode_Tailmatch(__pyx_v_key, __pyx_n_u_, 0, PY_SSIZE_T_MAX, 1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 13, __pyx_L1_error)
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "pop/pop.data.pyx":14
+    /* "data.pyx":14
  *     def __getattr__(self, key: str):
  *         if key.startswith("__") and key.endswith("__"):
  *             self.__getattribute__(key)             # <<<<<<<<<<<<<<
  *         try:
  *             return self[key]
  */
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_getattribute); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 14, __pyx_L1_error)
@@ -4272,24 +4267,24 @@
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 14, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "pop/pop.data.pyx":13
+    /* "data.pyx":13
  * cdef class NamespaceDict(dict[str, object]):
  *     def __getattr__(self, key: str):
  *         if key.startswith("__") and key.endswith("__"):             # <<<<<<<<<<<<<<
  *             self.__getattribute__(key)
  *         try:
  */
   }
 
-  /* "pop/pop.data.pyx":15
+  /* "data.pyx":15
  *         if key.startswith("__") and key.endswith("__"):
  *             self.__getattribute__(key)
  *         try:             # <<<<<<<<<<<<<<
  *             return self[key]
  *         except KeyError as e:
  */
   {
@@ -4297,74 +4292,74 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9);
     __Pyx_XGOTREF(__pyx_t_7);
     __Pyx_XGOTREF(__pyx_t_8);
     __Pyx_XGOTREF(__pyx_t_9);
     /*try:*/ {
 
-      /* "pop/pop.data.pyx":16
+      /* "data.pyx":16
  *             self.__getattribute__(key)
  *         try:
  *             return self[key]             # <<<<<<<<<<<<<<
  *         except KeyError as e:
  *             raise AttributeError(e)
  */
       __Pyx_XDECREF(__pyx_r);
       __pyx_t_3 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_r = __pyx_t_3;
       __pyx_t_3 = 0;
       goto __pyx_L10_try_return;
 
-      /* "pop/pop.data.pyx":15
+      /* "data.pyx":15
  *         if key.startswith("__") and key.endswith("__"):
  *             self.__getattribute__(key)
  *         try:             # <<<<<<<<<<<<<<
  *             return self[key]
  *         except KeyError as e:
  */
     }
     __pyx_L6_error:;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "pop/pop.data.pyx":17
+    /* "data.pyx":17
  *         try:
  *             return self[key]
  *         except KeyError as e:             # <<<<<<<<<<<<<<
  *             raise AttributeError(e)
  * 
  */
     __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
     if (__pyx_t_6) {
-      __Pyx_AddTraceback("pop.data.NamespaceDict.__getattr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("data.NamespaceDict.__getattr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5) < 0) __PYX_ERR(0, 17, __pyx_L8_except_error)
       __Pyx_XGOTREF(__pyx_t_3);
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_4);
       __pyx_v_e = __pyx_t_4;
       /*try:*/ {
 
-        /* "pop/pop.data.pyx":18
+        /* "data.pyx":18
  *             return self[key]
  *         except KeyError as e:
  *             raise AttributeError(e)             # <<<<<<<<<<<<<<
  * 
  *     def __setattr__(self, key: str, value: object):
  */
         __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_AttributeError, __pyx_v_e); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 18, __pyx_L17_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_Raise(__pyx_t_10, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         __PYX_ERR(0, 18, __pyx_L17_error)
       }
 
-      /* "pop/pop.data.pyx":17
+      /* "data.pyx":17
  *         try:
  *             return self[key]
  *         except KeyError as e:             # <<<<<<<<<<<<<<
  *             raise AttributeError(e)
  * 
  */
       /*finally:*/ {
@@ -4400,15 +4395,15 @@
           __pyx_lineno = __pyx_t_6; __pyx_clineno = __pyx_t_11; __pyx_filename = __pyx_t_12;
           goto __pyx_L8_except_error;
         }
       }
     }
     goto __pyx_L8_except_error;
 
-    /* "pop/pop.data.pyx":15
+    /* "data.pyx":15
  *         if key.startswith("__") and key.endswith("__"):
  *             self.__getattribute__(key)
  *         try:             # <<<<<<<<<<<<<<
  *             return self[key]
  *         except KeyError as e:
  */
     __pyx_L8_except_error:;
@@ -4421,156 +4416,156 @@
     __Pyx_XGIVEREF(__pyx_t_7);
     __Pyx_XGIVEREF(__pyx_t_8);
     __Pyx_XGIVEREF(__pyx_t_9);
     __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_8, __pyx_t_9);
     goto __pyx_L0;
   }
 
-  /* "pop/pop.data.pyx":12
+  /* "data.pyx":12
  * 
  * cdef class NamespaceDict(dict[str, object]):
  *     def __getattr__(self, key: str):             # <<<<<<<<<<<<<<
  *         if key.startswith("__") and key.endswith("__"):
  *             self.__getattribute__(key)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_AddTraceback("pop.data.NamespaceDict.__getattr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.NamespaceDict.__getattr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":20
+/* "data.pyx":20
  *             raise AttributeError(e)
  * 
  *     def __setattr__(self, key: str, value: object):             # <<<<<<<<<<<<<<
  *         if isinstance(value, dict):
  *             value = NamespaceDict(value)
  */
 
 /* Python wrapper */
-static int __pyx_pw_3pop_4data_13NamespaceDict_3__setattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value); /*proto*/
-static int __pyx_pw_3pop_4data_13NamespaceDict_3__setattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value) {
+static int __pyx_pw_4data_13NamespaceDict_3__setattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value); /*proto*/
+static int __pyx_pw_4data_13NamespaceDict_3__setattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setattr__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyUnicode_Type), 0, "key", 1))) __PYX_ERR(0, 20, __pyx_L1_error)
-  __pyx_r = __pyx_pf_3pop_4data_13NamespaceDict_2__setattr__(((struct __pyx_obj_3pop_4data_NamespaceDict *)__pyx_v_self), ((PyObject*)__pyx_v_key), ((PyObject *)__pyx_v_value));
+  __pyx_r = __pyx_pf_4data_13NamespaceDict_2__setattr__(((struct __pyx_obj_4data_NamespaceDict *)__pyx_v_self), ((PyObject*)__pyx_v_key), ((PyObject *)__pyx_v_value));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_3pop_4data_13NamespaceDict_2__setattr__(struct __pyx_obj_3pop_4data_NamespaceDict *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value) {
+static int __pyx_pf_4data_13NamespaceDict_2__setattr__(struct __pyx_obj_4data_NamespaceDict *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setattr__", 0);
   __Pyx_INCREF(__pyx_v_value);
 
-  /* "pop/pop.data.pyx":21
+  /* "data.pyx":21
  * 
  *     def __setattr__(self, key: str, value: object):
  *         if isinstance(value, dict):             # <<<<<<<<<<<<<<
  *             value = NamespaceDict(value)
  *         self[key] = value
  */
   __pyx_t_1 = PyDict_Check(__pyx_v_value); 
   if (__pyx_t_1) {
 
-    /* "pop/pop.data.pyx":22
+    /* "data.pyx":22
  *     def __setattr__(self, key: str, value: object):
  *         if isinstance(value, dict):
  *             value = NamespaceDict(value)             # <<<<<<<<<<<<<<
  *         self[key] = value
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_3pop_4data_NamespaceDict), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4data_NamespaceDict), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "pop/pop.data.pyx":21
+    /* "data.pyx":21
  * 
  *     def __setattr__(self, key: str, value: object):
  *         if isinstance(value, dict):             # <<<<<<<<<<<<<<
  *             value = NamespaceDict(value)
  *         self[key] = value
  */
   }
 
-  /* "pop/pop.data.pyx":23
+  /* "data.pyx":23
  *         if isinstance(value, dict):
  *             value = NamespaceDict(value)
  *         self[key] = value             # <<<<<<<<<<<<<<
  * 
  * 
  */
   if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_self), __pyx_v_key, __pyx_v_value) < 0))) __PYX_ERR(0, 23, __pyx_L1_error)
 
-  /* "pop/pop.data.pyx":20
+  /* "data.pyx":20
  *             raise AttributeError(e)
  * 
  *     def __setattr__(self, key: str, value: object):             # <<<<<<<<<<<<<<
  *         if isinstance(value, dict):
  *             value = NamespaceDict(value)
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("pop.data.NamespaceDict.__setattr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.NamespaceDict.__setattr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_13NamespaceDict_5__reduce_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_4data_13NamespaceDict_5__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_3pop_4data_13NamespaceDict_5__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_13NamespaceDict_5__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_3pop_4data_13NamespaceDict_5__reduce_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_4data_13NamespaceDict_5__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_13NamespaceDict_5__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4data_13NamespaceDict_5__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -4587,22 +4582,22 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  __pyx_r = __pyx_pf_3pop_4data_13NamespaceDict_4__reduce_cython__(((struct __pyx_obj_3pop_4data_NamespaceDict *)__pyx_v_self));
+  __pyx_r = __pyx_pf_4data_13NamespaceDict_4__reduce_cython__(((struct __pyx_obj_4data_NamespaceDict *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_13NamespaceDict_4__reduce_cython__(struct __pyx_obj_3pop_4data_NamespaceDict *__pyx_v_self) {
+static PyObject *__pyx_pf_4data_13NamespaceDict_4__reduce_cython__(struct __pyx_obj_4data_NamespaceDict *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
@@ -4790,15 +4785,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("pop.data.NamespaceDict.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.NamespaceDict.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -4808,23 +4803,23 @@
  *     else:
  *         return __pyx_unpickle_NamespaceDict, (type(self), 0xe3b0c44, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_NamespaceDict__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_13NamespaceDict_7__setstate_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_4data_13NamespaceDict_7__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_3pop_4data_13NamespaceDict_7__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_13NamespaceDict_7__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_3pop_4data_13NamespaceDict_7__setstate_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_4data_13NamespaceDict_7__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_13NamespaceDict_7__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4data_13NamespaceDict_7__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v___pyx_state = 0;
@@ -4886,47 +4881,47 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("pop.data.NamespaceDict.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.NamespaceDict.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_3pop_4data_13NamespaceDict_6__setstate_cython__(((struct __pyx_obj_3pop_4data_NamespaceDict *)__pyx_v_self), __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_4data_13NamespaceDict_6__setstate_cython__(((struct __pyx_obj_4data_NamespaceDict *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_13NamespaceDict_6__setstate_cython__(struct __pyx_obj_3pop_4data_NamespaceDict *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_4data_13NamespaceDict_6__setstate_cython__(struct __pyx_obj_4data_NamespaceDict *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_NamespaceDict, (type(self), 0xe3b0c44, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_NamespaceDict__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
   if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v___pyx_state))) __PYX_ERR(2, 17, __pyx_L1_error)
-  __pyx_t_1 = __pyx_f_3pop_4data___pyx_unpickle_NamespaceDict__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_4data___pyx_unpickle_NamespaceDict__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_NamespaceDict, (type(self), 0xe3b0c44, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
@@ -4934,33 +4929,33 @@
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pop.data.NamespaceDict.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.NamespaceDict.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":31
+/* "data.pyx":31
  *     cdef dict[str, list[str]] _split_cache
  * 
  *     def __init__(self, base_dicts=None):             # <<<<<<<<<<<<<<
  *         if base_dicts is None:
  *             base_dicts = []
  */
 
 /* Python wrapper */
-static int __pyx_pw_3pop_4data_14MultidictCache_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_3pop_4data_14MultidictCache_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_4data_14MultidictCache_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_4data_14MultidictCache_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_base_dicts = 0;
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -5015,77 +5010,77 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("pop.data.MultidictCache.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.MultidictCache.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_3pop_4data_14MultidictCache___init__(((struct __pyx_obj_3pop_4data_MultidictCache *)__pyx_v_self), __pyx_v_base_dicts);
+  __pyx_r = __pyx_pf_4data_14MultidictCache___init__(((struct __pyx_obj_4data_MultidictCache *)__pyx_v_self), __pyx_v_base_dicts);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_3pop_4data_14MultidictCache___init__(struct __pyx_obj_3pop_4data_MultidictCache *__pyx_v_self, PyObject *__pyx_v_base_dicts) {
+static int __pyx_pf_4data_14MultidictCache___init__(struct __pyx_obj_4data_MultidictCache *__pyx_v_self, PyObject *__pyx_v_base_dicts) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
   __Pyx_INCREF(__pyx_v_base_dicts);
 
-  /* "pop/pop.data.pyx":32
+  /* "data.pyx":32
  * 
  *     def __init__(self, base_dicts=None):
  *         if base_dicts is None:             # <<<<<<<<<<<<<<
  *             base_dicts = []
  *         self._base_dicts = base_dicts
  */
   __pyx_t_1 = (__pyx_v_base_dicts == Py_None);
   if (__pyx_t_1) {
 
-    /* "pop/pop.data.pyx":33
+    /* "data.pyx":33
  *     def __init__(self, base_dicts=None):
  *         if base_dicts is None:
  *             base_dicts = []             # <<<<<<<<<<<<<<
  *         self._base_dicts = base_dicts
  *         self._cache = dict[str, object]()
  */
     __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF_SET(__pyx_v_base_dicts, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "pop/pop.data.pyx":32
+    /* "data.pyx":32
  * 
  *     def __init__(self, base_dicts=None):
  *         if base_dicts is None:             # <<<<<<<<<<<<<<
  *             base_dicts = []
  *         self._base_dicts = base_dicts
  */
   }
 
-  /* "pop/pop.data.pyx":34
+  /* "data.pyx":34
  *         if base_dicts is None:
  *             base_dicts = []
  *         self._base_dicts = base_dicts             # <<<<<<<<<<<<<<
  *         self._cache = dict[str, object]()
  *         self._split_cache = dict[str, list[str]]()
  */
   if (!(likely(PyList_CheckExact(__pyx_v_base_dicts))||((__pyx_v_base_dicts) == Py_None) || __Pyx_RaiseUnexpectedTypeError("list", __pyx_v_base_dicts))) __PYX_ERR(0, 34, __pyx_L1_error)
@@ -5093,15 +5088,15 @@
   __Pyx_INCREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->_base_dicts);
   __Pyx_DECREF(__pyx_v_self->_base_dicts);
   __pyx_v_self->_base_dicts = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pop/pop.data.pyx":35
+  /* "data.pyx":35
  *             base_dicts = []
  *         self._base_dicts = base_dicts
  *         self._cache = dict[str, object]()             # <<<<<<<<<<<<<<
  *         self._split_cache = dict[str, list[str]]()
  * 
  */
   __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error)
@@ -5140,15 +5135,15 @@
   if (!(likely(PyDict_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_2))) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->_cache);
   __Pyx_DECREF(__pyx_v_self->_cache);
   __pyx_v_self->_cache = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pop/pop.data.pyx":36
+  /* "data.pyx":36
  *         self._base_dicts = base_dicts
  *         self._cache = dict[str, object]()
  *         self._split_cache = dict[str, list[str]]()             # <<<<<<<<<<<<<<
  * 
  *     cpdef _clear(self):
  */
   __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)(&PyList_Type)), ((PyObject *)(&PyUnicode_Type))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 36, __pyx_L1_error)
@@ -5189,53 +5184,53 @@
   if (!(likely(PyDict_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_2))) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->_split_cache);
   __Pyx_DECREF(__pyx_v_self->_split_cache);
   __pyx_v_self->_split_cache = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pop/pop.data.pyx":31
+  /* "data.pyx":31
  *     cdef dict[str, list[str]] _split_cache
  * 
  *     def __init__(self, base_dicts=None):             # <<<<<<<<<<<<<<
  *         if base_dicts is None:
  *             base_dicts = []
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("pop.data.MultidictCache.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.MultidictCache.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_base_dicts);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":38
+/* "data.pyx":38
  *         self._split_cache = dict[str, list[str]]()
  * 
  *     cpdef _clear(self):             # <<<<<<<<<<<<<<
  *         self._cache.clear()
  *         self._split_cache.clear()
  */
 
-static PyObject *__pyx_pw_3pop_4data_14MultidictCache_3_clear(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_4data_14MultidictCache_3_clear(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyObject *__pyx_f_3pop_4data_14MultidictCache__clear(struct __pyx_obj_3pop_4data_MultidictCache *__pyx_v_self, int __pyx_skip_dispatch) {
+static PyObject *__pyx_f_4data_14MultidictCache__clear(struct __pyx_obj_4data_MultidictCache *__pyx_v_self, int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
@@ -5251,15 +5246,15 @@
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
       __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_clear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_3pop_4data_14MultidictCache_3_clear)) {
+      if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_4data_14MultidictCache_3_clear)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         __pyx_t_5 = 0;
         #if CYTHON_UNPACK_METHODS
         if (unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -5294,41 +5289,41 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "pop/pop.data.pyx":39
+  /* "data.pyx":39
  * 
  *     cpdef _clear(self):
  *         self._cache.clear()             # <<<<<<<<<<<<<<
  *         self._split_cache.clear()
  * 
  */
   if (unlikely(__pyx_v_self->_cache == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "clear");
     __PYX_ERR(0, 39, __pyx_L1_error)
   }
   __pyx_t_6 = __Pyx_PyDict_Clear(__pyx_v_self->_cache); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 39, __pyx_L1_error)
 
-  /* "pop/pop.data.pyx":40
+  /* "data.pyx":40
  *     cpdef _clear(self):
  *         self._cache.clear()
  *         self._split_cache.clear()             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, key:str):
  */
   if (unlikely(__pyx_v_self->_split_cache == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "clear");
     __PYX_ERR(0, 40, __pyx_L1_error)
   }
   __pyx_t_6 = __Pyx_PyDict_Clear(__pyx_v_self->_split_cache); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 40, __pyx_L1_error)
 
-  /* "pop/pop.data.pyx":38
+  /* "data.pyx":38
  *         self._split_cache = dict[str, list[str]]()
  * 
  *     cpdef _clear(self):             # <<<<<<<<<<<<<<
  *         self._cache.clear()
  *         self._split_cache.clear()
  */
 
@@ -5336,32 +5331,32 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("pop.data.MultidictCache._clear", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.MultidictCache._clear", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_14MultidictCache_3_clear(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_4data_14MultidictCache_3_clear(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_3pop_4data_14MultidictCache_3_clear = {"_clear", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_14MultidictCache_3_clear, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_3pop_4data_14MultidictCache_3_clear(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_4data_14MultidictCache_3_clear = {"_clear", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_14MultidictCache_3_clear, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4data_14MultidictCache_3_clear(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -5378,79 +5373,79 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("_clear", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "_clear", 0))) return NULL;
-  __pyx_r = __pyx_pf_3pop_4data_14MultidictCache_2_clear(((struct __pyx_obj_3pop_4data_MultidictCache *)__pyx_v_self));
+  __pyx_r = __pyx_pf_4data_14MultidictCache_2_clear(((struct __pyx_obj_4data_MultidictCache *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_14MultidictCache_2_clear(struct __pyx_obj_3pop_4data_MultidictCache *__pyx_v_self) {
+static PyObject *__pyx_pf_4data_14MultidictCache_2_clear(struct __pyx_obj_4data_MultidictCache *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_clear", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_3pop_4data_14MultidictCache__clear(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_4data_14MultidictCache__clear(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pop.data.MultidictCache._clear", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.MultidictCache._clear", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":42
+/* "data.pyx":42
  *         self._split_cache.clear()
  * 
  *     def __getitem__(self, key:str):             # <<<<<<<<<<<<<<
  *         if key in self._cache:
  *             return self._cache[key]
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_14MultidictCache_5__getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_key); /*proto*/
-static PyObject *__pyx_pw_3pop_4data_14MultidictCache_5__getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_key) {
+static PyObject *__pyx_pw_4data_14MultidictCache_5__getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_key); /*proto*/
+static PyObject *__pyx_pw_4data_14MultidictCache_5__getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_key) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__getitem__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyUnicode_Type), 0, "key", 1))) __PYX_ERR(0, 42, __pyx_L1_error)
-  __pyx_r = __pyx_pf_3pop_4data_14MultidictCache_4__getitem__(((struct __pyx_obj_3pop_4data_MultidictCache *)__pyx_v_self), ((PyObject*)__pyx_v_key));
+  __pyx_r = __pyx_pf_4data_14MultidictCache_4__getitem__(((struct __pyx_obj_4data_MultidictCache *)__pyx_v_self), ((PyObject*)__pyx_v_key));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_14MultidictCache_4__getitem__(struct __pyx_obj_3pop_4data_MultidictCache *__pyx_v_self, PyObject *__pyx_v_key) {
+static PyObject *__pyx_pf_4data_14MultidictCache_4__getitem__(struct __pyx_obj_4data_MultidictCache *__pyx_v_self, PyObject *__pyx_v_key) {
   PyObject *__pyx_v_parts = NULL;
   PyObject *__pyx_v_base_dict = NULL;
   PyObject *__pyx_v_finder = NULL;
   PyObject *__pyx_v_part = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
@@ -5467,29 +5462,29 @@
   PyObject *__pyx_t_12 = NULL;
   Py_UCS4 __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 1);
 
-  /* "pop/pop.data.pyx":43
+  /* "data.pyx":43
  * 
  *     def __getitem__(self, key:str):
  *         if key in self._cache:             # <<<<<<<<<<<<<<
  *             return self._cache[key]
  * 
  */
   if (unlikely(__pyx_v_self->_cache == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
     __PYX_ERR(0, 43, __pyx_L1_error)
   }
   __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_key, __pyx_v_self->_cache, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 43, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "pop/pop.data.pyx":44
+    /* "data.pyx":44
  *     def __getitem__(self, key:str):
  *         if key in self._cache:
  *             return self._cache[key]             # <<<<<<<<<<<<<<
  * 
  *         if key not in self._split_cache:
  */
     __Pyx_XDECREF(__pyx_r);
@@ -5499,38 +5494,38 @@
     }
     __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_self->_cache, __pyx_v_key); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "pop/pop.data.pyx":43
+    /* "data.pyx":43
  * 
  *     def __getitem__(self, key:str):
  *         if key in self._cache:             # <<<<<<<<<<<<<<
  *             return self._cache[key]
  * 
  */
   }
 
-  /* "pop/pop.data.pyx":46
+  /* "data.pyx":46
  *             return self._cache[key]
  * 
  *         if key not in self._split_cache:             # <<<<<<<<<<<<<<
  *             self._split_cache[key] = key.split('.')
  * 
  */
   if (unlikely(__pyx_v_self->_split_cache == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
     __PYX_ERR(0, 46, __pyx_L1_error)
   }
   __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_key, __pyx_v_self->_split_cache, Py_NE)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 46, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "pop/pop.data.pyx":47
+    /* "data.pyx":47
  * 
  *         if key not in self._split_cache:
  *             self._split_cache[key] = key.split('.')             # <<<<<<<<<<<<<<
  * 
  *         parts = self._split_cache[key]
  */
     __pyx_t_2 = PyUnicode_Split(__pyx_v_key, __Pyx_NoneAsNull(__pyx_kp_u__2), -1L); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
@@ -5538,24 +5533,24 @@
     if (unlikely(__pyx_v_self->_split_cache == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
       __PYX_ERR(0, 47, __pyx_L1_error)
     }
     if (unlikely((PyDict_SetItem(__pyx_v_self->_split_cache, __pyx_v_key, __pyx_t_2) < 0))) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pop/pop.data.pyx":46
+    /* "data.pyx":46
  *             return self._cache[key]
  * 
  *         if key not in self._split_cache:             # <<<<<<<<<<<<<<
  *             self._split_cache[key] = key.split('.')
  * 
  */
   }
 
-  /* "pop/pop.data.pyx":49
+  /* "data.pyx":49
  *             self._split_cache[key] = key.split('.')
  * 
  *         parts = self._split_cache[key]             # <<<<<<<<<<<<<<
  *         for base_dict in self._base_dicts:
  *             finder = base_dict
  */
   if (unlikely(__pyx_v_self->_split_cache == Py_None)) {
@@ -5563,15 +5558,15 @@
     __PYX_ERR(0, 49, __pyx_L1_error)
   }
   __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_self->_split_cache, __pyx_v_key); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_parts = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pop/pop.data.pyx":50
+  /* "data.pyx":50
  * 
  *         parts = self._split_cache[key]
  *         for base_dict in self._base_dicts:             # <<<<<<<<<<<<<<
  *             finder = base_dict
  *             try:
  */
   if (unlikely(__pyx_v_self->_base_dicts == Py_None)) {
@@ -5593,25 +5588,25 @@
     #else
     __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 50, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_base_dict, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "pop/pop.data.pyx":51
+    /* "data.pyx":51
  *         parts = self._split_cache[key]
  *         for base_dict in self._base_dicts:
  *             finder = base_dict             # <<<<<<<<<<<<<<
  *             try:
  *                 for part in parts:
  */
     __Pyx_INCREF(__pyx_v_base_dict);
     __Pyx_XDECREF_SET(__pyx_v_finder, __pyx_v_base_dict);
 
-    /* "pop/pop.data.pyx":52
+    /* "data.pyx":52
  *         for base_dict in self._base_dicts:
  *             finder = base_dict
  *             try:             # <<<<<<<<<<<<<<
  *                 for part in parts:
  *                     finder = finder[part]
  */
     {
@@ -5619,15 +5614,15 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7);
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
       /*try:*/ {
 
-        /* "pop/pop.data.pyx":53
+        /* "data.pyx":53
  *             finder = base_dict
  *             try:
  *                 for part in parts:             # <<<<<<<<<<<<<<
  *                     finder = finder[part]
  *                 self._cache[key] = finder
  */
         if (likely(PyList_CheckExact(__pyx_v_parts)) || PyTuple_CheckExact(__pyx_v_parts)) {
@@ -5681,90 +5676,90 @@
               break;
             }
             __Pyx_GOTREF(__pyx_t_10);
           }
           __Pyx_XDECREF_SET(__pyx_v_part, __pyx_t_10);
           __pyx_t_10 = 0;
 
-          /* "pop/pop.data.pyx":54
+          /* "data.pyx":54
  *             try:
  *                 for part in parts:
  *                     finder = finder[part]             # <<<<<<<<<<<<<<
  *                 self._cache[key] = finder
  *                 return finder
  */
           __pyx_t_10 = __Pyx_PyObject_GetItem(__pyx_v_finder, __pyx_v_part); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 54, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_10);
           __Pyx_DECREF_SET(__pyx_v_finder, __pyx_t_10);
           __pyx_t_10 = 0;
 
-          /* "pop/pop.data.pyx":53
+          /* "data.pyx":53
  *             finder = base_dict
  *             try:
  *                 for part in parts:             # <<<<<<<<<<<<<<
  *                     finder = finder[part]
  *                 self._cache[key] = finder
  */
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "pop/pop.data.pyx":55
+        /* "data.pyx":55
  *                 for part in parts:
  *                     finder = finder[part]
  *                 self._cache[key] = finder             # <<<<<<<<<<<<<<
  *                 return finder
  *             except KeyError:
  */
         if (unlikely(__pyx_v_self->_cache == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
           __PYX_ERR(0, 55, __pyx_L7_error)
         }
         if (unlikely((PyDict_SetItem(__pyx_v_self->_cache, __pyx_v_key, __pyx_v_finder) < 0))) __PYX_ERR(0, 55, __pyx_L7_error)
 
-        /* "pop/pop.data.pyx":56
+        /* "data.pyx":56
  *                     finder = finder[part]
  *                 self._cache[key] = finder
  *                 return finder             # <<<<<<<<<<<<<<
  *             except KeyError:
  *                 continue
  */
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_v_finder);
         __pyx_r = __pyx_v_finder;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         goto __pyx_L11_try_return;
 
-        /* "pop/pop.data.pyx":52
+        /* "data.pyx":52
  *         for base_dict in self._base_dicts:
  *             finder = base_dict
  *             try:             # <<<<<<<<<<<<<<
  *                 for part in parts:
  *                     finder = finder[part]
  */
       }
       __pyx_L7_error:;
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "pop/pop.data.pyx":57
+      /* "data.pyx":57
  *                 self._cache[key] = finder
  *                 return finder
  *             except KeyError:             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
       __pyx_t_11 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
       if (__pyx_t_11) {
-        __Pyx_AddTraceback("pop.data.MultidictCache.__getitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+        __Pyx_AddTraceback("data.MultidictCache.__getitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
         if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_10, &__pyx_t_12) < 0) __PYX_ERR(0, 57, __pyx_L9_except_error)
         __Pyx_XGOTREF(__pyx_t_4);
         __Pyx_XGOTREF(__pyx_t_10);
         __Pyx_XGOTREF(__pyx_t_12);
 
-        /* "pop/pop.data.pyx":58
+        /* "data.pyx":58
  *                 return finder
  *             except KeyError:
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *         raise KeyError(f"Item '{key}' not found in any base dictionary")
  */
         goto __pyx_L18_except_continue;
@@ -5772,15 +5767,15 @@
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         goto __pyx_L13_try_continue;
       }
       goto __pyx_L9_except_error;
 
-      /* "pop/pop.data.pyx":52
+      /* "data.pyx":52
  *         for base_dict in self._base_dicts:
  *             finder = base_dict
  *             try:             # <<<<<<<<<<<<<<
  *                 for part in parts:
  *                     finder = finder[part]
  */
       __pyx_L9_except_error:;
@@ -5799,26 +5794,26 @@
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_XGIVEREF(__pyx_t_6);
       __Pyx_XGIVEREF(__pyx_t_7);
       __Pyx_ExceptionReset(__pyx_t_5, __pyx_t_6, __pyx_t_7);
       goto __pyx_L0;
     }
 
-    /* "pop/pop.data.pyx":50
+    /* "data.pyx":50
  * 
  *         parts = self._split_cache[key]
  *         for base_dict in self._base_dicts:             # <<<<<<<<<<<<<<
  *             finder = base_dict
  *             try:
  */
     __pyx_L5_continue:;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pop/pop.data.pyx":60
+  /* "data.pyx":60
  *                 continue
  * 
  *         raise KeyError(f"Item '{key}' not found in any base dictionary")             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
@@ -5844,64 +5839,64 @@
   __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_KeyError, __pyx_t_12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __Pyx_Raise(__pyx_t_2, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __PYX_ERR(0, 60, __pyx_L1_error)
 
-  /* "pop/pop.data.pyx":42
+  /* "data.pyx":42
  *         self._split_cache.clear()
  * 
  *     def __getitem__(self, key:str):             # <<<<<<<<<<<<<<
  *         if key in self._cache:
  *             return self._cache[key]
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_12);
-  __Pyx_AddTraceback("pop.data.MultidictCache.__getitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.MultidictCache.__getitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_parts);
   __Pyx_XDECREF(__pyx_v_base_dict);
   __Pyx_XDECREF(__pyx_v_finder);
   __Pyx_XDECREF(__pyx_v_part);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":62
+/* "data.pyx":62
  *         raise KeyError(f"Item '{key}' not found in any base dictionary")
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return iter({k for base_dict in self._base_dicts for k in base_dict})
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_14MultidictCache_7__iter__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_3pop_4data_14MultidictCache_7__iter__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_4data_14MultidictCache_7__iter__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_4data_14MultidictCache_7__iter__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__iter__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  __pyx_r = __pyx_pf_3pop_4data_14MultidictCache_6__iter__(((struct __pyx_obj_3pop_4data_MultidictCache *)__pyx_v_self));
+  __pyx_r = __pyx_pf_4data_14MultidictCache_6__iter__(((struct __pyx_obj_4data_MultidictCache *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_14MultidictCache_6__iter__(struct __pyx_obj_3pop_4data_MultidictCache *__pyx_v_self) {
+static PyObject *__pyx_pf_4data_14MultidictCache_6__iter__(struct __pyx_obj_4data_MultidictCache *__pyx_v_self) {
   PyObject *__pyx_7genexpr__pyx_v_base_dict = NULL;
   PyObject *__pyx_7genexpr__pyx_v_k = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
@@ -5910,15 +5905,15 @@
   PyObject *(*__pyx_t_6)(PyObject *);
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iter__", 1);
 
-  /* "pop/pop.data.pyx":63
+  /* "data.pyx":63
  * 
  *     def __iter__(self):
  *         return iter({k for base_dict in self._base_dicts for k in base_dict})             # <<<<<<<<<<<<<<
  * 
  *     def __contains__(self, item):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -6018,112 +6013,112 @@
   __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pop/pop.data.pyx":62
+  /* "data.pyx":62
  *         raise KeyError(f"Item '{key}' not found in any base dictionary")
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return iter({k for base_dict in self._base_dicts for k in base_dict})
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("pop.data.MultidictCache.__iter__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.MultidictCache.__iter__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_base_dict);
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_k);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":65
+/* "data.pyx":65
  *         return iter({k for base_dict in self._base_dicts for k in base_dict})
  * 
  *     def __contains__(self, item):             # <<<<<<<<<<<<<<
  *         return any(item in base_dict for base_dict in self._base_dicts)
  * 
  */
 
 /* Python wrapper */
-static int __pyx_pw_3pop_4data_14MultidictCache_9__contains__(PyObject *__pyx_v_self, PyObject *__pyx_v_item); /*proto*/
-static int __pyx_pw_3pop_4data_14MultidictCache_9__contains__(PyObject *__pyx_v_self, PyObject *__pyx_v_item) {
+static int __pyx_pw_4data_14MultidictCache_9__contains__(PyObject *__pyx_v_self, PyObject *__pyx_v_item); /*proto*/
+static int __pyx_pw_4data_14MultidictCache_9__contains__(PyObject *__pyx_v_self, PyObject *__pyx_v_item) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__contains__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  __pyx_r = __pyx_pf_3pop_4data_14MultidictCache_8__contains__(((struct __pyx_obj_3pop_4data_MultidictCache *)__pyx_v_self), ((PyObject *)__pyx_v_item));
+  __pyx_r = __pyx_pf_4data_14MultidictCache_8__contains__(((struct __pyx_obj_4data_MultidictCache *)__pyx_v_self), ((PyObject *)__pyx_v_item));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static PyObject *__pyx_gb_3pop_4data_14MultidictCache_12__contains___2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+static PyObject *__pyx_gb_4data_14MultidictCache_12__contains___2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "pop/pop.data.pyx":66
+/* "data.pyx":66
  * 
  *     def __contains__(self, item):
  *         return any(item in base_dict for base_dict in self._base_dicts)             # <<<<<<<<<<<<<<
  * 
  * cdef class ImmutableNamespaceDict:
  */
 
-static PyObject *__pyx_pf_3pop_4data_14MultidictCache_12__contains___genexpr(PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0) {
-  struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr *__pyx_cur_scope;
+static PyObject *__pyx_pf_4data_14MultidictCache_12__contains___genexpr(PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0) {
+  struct __pyx_obj_4data___pyx_scope_struct_1_genexpr *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
-  __pyx_cur_scope = (struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr *)__pyx_tp_new_3pop_4data___pyx_scope_struct_1_genexpr(__pyx_ptype_3pop_4data___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
+  __pyx_cur_scope = (struct __pyx_obj_4data___pyx_scope_struct_1_genexpr *)__pyx_tp_new_4data___pyx_scope_struct_1_genexpr(__pyx_ptype_4data___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr *)Py_None);
+    __pyx_cur_scope = ((struct __pyx_obj_4data___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 66, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
-  __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__ *) __pyx_self;
+  __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_4data___pyx_scope_struct____contains__ *) __pyx_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_outer_scope);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_outer_scope);
   __pyx_cur_scope->__pyx_genexpr_arg_0 = __pyx_genexpr_arg_0;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_3pop_4data_14MultidictCache_12__contains___2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_contains___locals_genexpr, __pyx_n_s_pop_data); if (unlikely(!gen)) __PYX_ERR(0, 66, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_4data_14MultidictCache_12__contains___2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_contains___locals_genexpr, __pyx_n_s_data); if (unlikely(!gen)) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_AddTraceback("pop.data.MultidictCache.__contains__.genexpr", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.MultidictCache.__contains__.genexpr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_DECREF((PyObject *)__pyx_cur_scope);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_3pop_4data_14MultidictCache_12__contains___2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_4data_14MultidictCache_12__contains___2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
-  struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr *__pyx_cur_scope = ((struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr *)__pyx_generator->closure);
+  struct __pyx_obj_4data___pyx_scope_struct_1_genexpr *__pyx_cur_scope = ((struct __pyx_obj_4data___pyx_scope_struct_1_genexpr *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -6196,100 +6191,100 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":65
+/* "data.pyx":65
  *         return iter({k for base_dict in self._base_dicts for k in base_dict})
  * 
  *     def __contains__(self, item):             # <<<<<<<<<<<<<<
  *         return any(item in base_dict for base_dict in self._base_dicts)
  * 
  */
 
-static int __pyx_pf_3pop_4data_14MultidictCache_8__contains__(struct __pyx_obj_3pop_4data_MultidictCache *__pyx_v_self, PyObject *__pyx_v_item) {
-  struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__ *__pyx_cur_scope;
-  PyObject *__pyx_gb_3pop_4data_14MultidictCache_12__contains___2generator = 0;
+static int __pyx_pf_4data_14MultidictCache_8__contains__(struct __pyx_obj_4data_MultidictCache *__pyx_v_self, PyObject *__pyx_v_item) {
+  struct __pyx_obj_4data___pyx_scope_struct____contains__ *__pyx_cur_scope;
+  PyObject *__pyx_gb_4data_14MultidictCache_12__contains___2generator = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__contains__", 0);
-  __pyx_cur_scope = (struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__ *)__pyx_tp_new_3pop_4data___pyx_scope_struct____contains__(__pyx_ptype_3pop_4data___pyx_scope_struct____contains__, __pyx_empty_tuple, NULL);
+  __pyx_cur_scope = (struct __pyx_obj_4data___pyx_scope_struct____contains__ *)__pyx_tp_new_4data___pyx_scope_struct____contains__(__pyx_ptype_4data___pyx_scope_struct____contains__, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__ *)Py_None);
+    __pyx_cur_scope = ((struct __pyx_obj_4data___pyx_scope_struct____contains__ *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 65, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_item = __pyx_v_item;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_item);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_item);
 
-  /* "pop/pop.data.pyx":66
+  /* "data.pyx":66
  * 
  *     def __contains__(self, item):
  *         return any(item in base_dict for base_dict in self._base_dicts)             # <<<<<<<<<<<<<<
  * 
  * cdef class ImmutableNamespaceDict:
  */
-  __pyx_t_1 = __pyx_pf_3pop_4data_14MultidictCache_12__contains___genexpr(((PyObject*)__pyx_cur_scope), __pyx_v_self->_base_dicts); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_1 = __pyx_pf_4data_14MultidictCache_12__contains___genexpr(((PyObject*)__pyx_cur_scope), __pyx_v_self->_base_dicts); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_Generator_Next(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   goto __pyx_L0;
 
-  /* "pop/pop.data.pyx":65
+  /* "data.pyx":65
  *         return iter({k for base_dict in self._base_dicts for k in base_dict})
  * 
  *     def __contains__(self, item):             # <<<<<<<<<<<<<<
  *         return any(item in base_dict for base_dict in self._base_dicts)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("pop.data.MultidictCache.__contains__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.MultidictCache.__contains__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_gb_3pop_4data_14MultidictCache_12__contains___2generator);
+  __Pyx_XDECREF(__pyx_gb_4data_14MultidictCache_12__contains___2generator);
   __Pyx_DECREF((PyObject *)__pyx_cur_scope);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_14MultidictCache_11__reduce_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_4data_14MultidictCache_11__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_3pop_4data_14MultidictCache_11__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_14MultidictCache_11__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_3pop_4data_14MultidictCache_11__reduce_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_4data_14MultidictCache_11__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_14MultidictCache_11__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4data_14MultidictCache_11__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -6306,22 +6301,22 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  __pyx_r = __pyx_pf_3pop_4data_14MultidictCache_10__reduce_cython__(((struct __pyx_obj_3pop_4data_MultidictCache *)__pyx_v_self));
+  __pyx_r = __pyx_pf_4data_14MultidictCache_10__reduce_cython__(((struct __pyx_obj_4data_MultidictCache *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_14MultidictCache_10__reduce_cython__(struct __pyx_obj_3pop_4data_MultidictCache *__pyx_v_self) {
+static PyObject *__pyx_pf_4data_14MultidictCache_10__reduce_cython__(struct __pyx_obj_4data_MultidictCache *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
@@ -6536,15 +6531,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("pop.data.MultidictCache.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.MultidictCache.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -6554,23 +6549,23 @@
  *     else:
  *         return __pyx_unpickle_MultidictCache, (type(self), 0x09e6f20, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_MultidictCache__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_14MultidictCache_13__setstate_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_4data_14MultidictCache_13__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_3pop_4data_14MultidictCache_13__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_14MultidictCache_13__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_3pop_4data_14MultidictCache_13__setstate_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_4data_14MultidictCache_13__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_14MultidictCache_13__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4data_14MultidictCache_13__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v___pyx_state = 0;
@@ -6632,47 +6627,47 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("pop.data.MultidictCache.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.MultidictCache.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_3pop_4data_14MultidictCache_12__setstate_cython__(((struct __pyx_obj_3pop_4data_MultidictCache *)__pyx_v_self), __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_4data_14MultidictCache_12__setstate_cython__(((struct __pyx_obj_4data_MultidictCache *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_14MultidictCache_12__setstate_cython__(struct __pyx_obj_3pop_4data_MultidictCache *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_4data_14MultidictCache_12__setstate_cython__(struct __pyx_obj_4data_MultidictCache *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_MultidictCache, (type(self), 0x09e6f20, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_MultidictCache__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
   if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v___pyx_state))) __PYX_ERR(2, 17, __pyx_L1_error)
-  __pyx_t_1 = __pyx_f_3pop_4data___pyx_unpickle_MultidictCache__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_4data___pyx_unpickle_MultidictCache__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_MultidictCache, (type(self), 0x09e6f20, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
@@ -6680,33 +6675,33 @@
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pop.data.MultidictCache.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.MultidictCache.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":71
+/* "data.pyx":71
  *     cdef readonly dict __data
  * 
  *     def __init__(self, data=None):             # <<<<<<<<<<<<<<
  *         if isinstance(data, ImmutableNamespaceDict):
  *             self.__data = data.__data
  */
 
 /* Python wrapper */
-static int __pyx_pw_3pop_4data_22ImmutableNamespaceDict_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_3pop_4data_22ImmutableNamespaceDict_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_4data_22ImmutableNamespaceDict_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_4data_22ImmutableNamespaceDict_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_data = 0;
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -6761,32 +6756,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict___init__(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self), __pyx_v_data);
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict___init__(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self), __pyx_v_data);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_3pop_4data_22ImmutableNamespaceDict___init__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_data) {
+static int __pyx_pf_4data_22ImmutableNamespaceDict___init__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_data) {
   PyObject *__pyx_8genexpr2__pyx_v_key = NULL;
   PyObject *__pyx_8genexpr2__pyx_v_value = NULL;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -6798,25 +6793,25 @@
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
 
-  /* "pop/pop.data.pyx":72
+  /* "data.pyx":72
  * 
  *     def __init__(self, data=None):
  *         if isinstance(data, ImmutableNamespaceDict):             # <<<<<<<<<<<<<<
  *             self.__data = data.__data
  *         elif isinstance(data, dict):
  */
-  __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_data, __pyx_ptype_3pop_4data_ImmutableNamespaceDict); 
+  __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_data, __pyx_ptype_4data_ImmutableNamespaceDict); 
   if (__pyx_t_1) {
 
-    /* "pop/pop.data.pyx":73
+    /* "data.pyx":73
  *     def __init__(self, data=None):
  *         if isinstance(data, ImmutableNamespaceDict):
  *             self.__data = data.__data             # <<<<<<<<<<<<<<
  *         elif isinstance(data, dict):
  *             self.__data = {key: freeze(value) for key, value in data.items()}
  */
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_ImmutableNamespaceDict__data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
@@ -6824,35 +6819,35 @@
     if (!(likely(PyDict_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_2))) __PYX_ERR(0, 73, __pyx_L1_error)
     __Pyx_GIVEREF(__pyx_t_2);
     __Pyx_GOTREF(__pyx_v_self->_ImmutableNamespaceDict__data);
     __Pyx_DECREF(__pyx_v_self->_ImmutableNamespaceDict__data);
     __pyx_v_self->_ImmutableNamespaceDict__data = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "pop/pop.data.pyx":72
+    /* "data.pyx":72
  * 
  *     def __init__(self, data=None):
  *         if isinstance(data, ImmutableNamespaceDict):             # <<<<<<<<<<<<<<
  *             self.__data = data.__data
  *         elif isinstance(data, dict):
  */
     goto __pyx_L3;
   }
 
-  /* "pop/pop.data.pyx":74
+  /* "data.pyx":74
  *         if isinstance(data, ImmutableNamespaceDict):
  *             self.__data = data.__data
  *         elif isinstance(data, dict):             # <<<<<<<<<<<<<<
  *             self.__data = {key: freeze(value) for key, value in data.items()}
  *         else:
  */
   __pyx_t_1 = PyDict_Check(__pyx_v_data); 
   if (__pyx_t_1) {
 
-    /* "pop/pop.data.pyx":75
+    /* "data.pyx":75
  *             self.__data = data.__data
  *         elif isinstance(data, dict):
  *             self.__data = {key: freeze(value) for key, value in data.items()}             # <<<<<<<<<<<<<<
  *         else:
  *             self.__data = {}
  */
     { /* enter inner scope */
@@ -6917,25 +6912,25 @@
     } /* exit inner scope */
     __Pyx_GIVEREF(__pyx_t_2);
     __Pyx_GOTREF(__pyx_v_self->_ImmutableNamespaceDict__data);
     __Pyx_DECREF(__pyx_v_self->_ImmutableNamespaceDict__data);
     __pyx_v_self->_ImmutableNamespaceDict__data = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "pop/pop.data.pyx":74
+    /* "data.pyx":74
  *         if isinstance(data, ImmutableNamespaceDict):
  *             self.__data = data.__data
  *         elif isinstance(data, dict):             # <<<<<<<<<<<<<<
  *             self.__data = {key: freeze(value) for key, value in data.items()}
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "pop/pop.data.pyx":77
+  /* "data.pyx":77
  *             self.__data = {key: freeze(value) for key, value in data.items()}
  *         else:
  *             self.__data = {}             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, key):
  */
   /*else*/ {
@@ -6945,15 +6940,15 @@
     __Pyx_GOTREF(__pyx_v_self->_ImmutableNamespaceDict__data);
     __Pyx_DECREF(__pyx_v_self->_ImmutableNamespaceDict__data);
     __pyx_v_self->_ImmutableNamespaceDict__data = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
   }
   __pyx_L3:;
 
-  /* "pop/pop.data.pyx":71
+  /* "data.pyx":71
  *     cdef readonly dict __data
  * 
  *     def __init__(self, data=None):             # <<<<<<<<<<<<<<
  *         if isinstance(data, ImmutableNamespaceDict):
  *             self.__data = data.__data
  */
 
@@ -6962,47 +6957,47 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_key);
   __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_value);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":79
+/* "data.pyx":79
  *             self.__data = {}
  * 
  *     def __getitem__(self, key):             # <<<<<<<<<<<<<<
  *         try:
  *             return self.__data[key]
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_3__getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_key); /*proto*/
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_3__getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_key) {
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_3__getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_key); /*proto*/
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_3__getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_key) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__getitem__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_2__getitem__(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self), ((PyObject *)__pyx_v_key));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_2__getitem__(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self), ((PyObject *)__pyx_v_key));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_2__getitem__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key) {
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_2__getitem__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
@@ -7010,15 +7005,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 1);
 
-  /* "pop/pop.data.pyx":80
+  /* "data.pyx":80
  * 
  *     def __getitem__(self, key):
  *         try:             # <<<<<<<<<<<<<<
  *             return self.__data[key]
  *         except KeyError:
  */
   {
@@ -7026,15 +7021,15 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "pop/pop.data.pyx":81
+      /* "data.pyx":81
  *     def __getitem__(self, key):
  *         try:
  *             return self.__data[key]             # <<<<<<<<<<<<<<
  *         except KeyError:
  *             return ImmutableNamespaceDict()
  */
       __Pyx_XDECREF(__pyx_r);
@@ -7044,60 +7039,60 @@
       }
       __pyx_t_4 = __Pyx_PyDict_GetItem(__pyx_v_self->_ImmutableNamespaceDict__data, __pyx_v_key); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_r = __pyx_t_4;
       __pyx_t_4 = 0;
       goto __pyx_L7_try_return;
 
-      /* "pop/pop.data.pyx":80
+      /* "data.pyx":80
  * 
  *     def __getitem__(self, key):
  *         try:             # <<<<<<<<<<<<<<
  *             return self.__data[key]
  *         except KeyError:
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pop/pop.data.pyx":82
+    /* "data.pyx":82
  *         try:
  *             return self.__data[key]
  *         except KeyError:             # <<<<<<<<<<<<<<
  *             return ImmutableNamespaceDict()
  * 
  */
     __pyx_t_5 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
     if (__pyx_t_5) {
-      __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__getitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("data.ImmutableNamespaceDict.__getitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 82, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "pop/pop.data.pyx":83
+      /* "data.pyx":83
  *             return self.__data[key]
  *         except KeyError:
  *             return ImmutableNamespaceDict()             # <<<<<<<<<<<<<<
  * 
  *     def __getattr__(self, key):
  */
       __Pyx_XDECREF(__pyx_r);
-      __pyx_t_8 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_3pop_4data_ImmutableNamespaceDict)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 83, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_4data_ImmutableNamespaceDict)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 83, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_r = __pyx_t_8;
       __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       goto __pyx_L6_except_return;
     }
     goto __pyx_L5_except_error;
 
-    /* "pop/pop.data.pyx":80
+    /* "data.pyx":80
  * 
  *     def __getitem__(self, key):
  *         try:             # <<<<<<<<<<<<<<
  *             return self.__data[key]
  *         except KeyError:
  */
     __pyx_L5_except_error:;
@@ -7116,88 +7111,88 @@
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L0;
   }
 
-  /* "pop/pop.data.pyx":79
+  /* "data.pyx":79
  *             self.__data = {}
  * 
  *     def __getitem__(self, key):             # <<<<<<<<<<<<<<
  *         try:
  *             return self.__data[key]
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__getitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.__getitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":85
+/* "data.pyx":85
  *             return ImmutableNamespaceDict()
  * 
  *     def __getattr__(self, key):             # <<<<<<<<<<<<<<
  *         if key in self.__data:
  *             return self.__data[key]
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_5__getattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_key); /*proto*/
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_5__getattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_key) {
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_5__getattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_key); /*proto*/
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_5__getattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_key) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__getattr__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_4__getattr__(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self), ((PyObject *)__pyx_v_key));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_4__getattr__(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self), ((PyObject *)__pyx_v_key));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_4__getattr__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key) {
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_4__getattr__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   Py_UCS4 __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getattr__", 1);
 
-  /* "pop/pop.data.pyx":86
+  /* "data.pyx":86
  * 
  *     def __getattr__(self, key):
  *         if key in self.__data:             # <<<<<<<<<<<<<<
  *             return self.__data[key]
  *         raise AttributeError(f"'{type(self).__name__}' object has no attribute '{key}'")
  */
   if (unlikely(__pyx_v_self->_ImmutableNamespaceDict__data == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
     __PYX_ERR(0, 86, __pyx_L1_error)
   }
   __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_key, __pyx_v_self->_ImmutableNamespaceDict__data, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 86, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "pop/pop.data.pyx":87
+    /* "data.pyx":87
  *     def __getattr__(self, key):
  *         if key in self.__data:
  *             return self.__data[key]             # <<<<<<<<<<<<<<
  *         raise AttributeError(f"'{type(self).__name__}' object has no attribute '{key}'")
  * 
  */
     __Pyx_XDECREF(__pyx_r);
@@ -7207,24 +7202,24 @@
     }
     __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_self->_ImmutableNamespaceDict__data, __pyx_v_key); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "pop/pop.data.pyx":86
+    /* "data.pyx":86
  * 
  *     def __getattr__(self, key):
  *         if key in self.__data:             # <<<<<<<<<<<<<<
  *             return self.__data[key]
  *         raise AttributeError(f"'{type(self).__name__}' object has no attribute '{key}'")
  */
   }
 
-  /* "pop/pop.data.pyx":88
+  /* "data.pyx":88
  *         if key in self.__data:
  *             return self.__data[key]
  *         raise AttributeError(f"'{type(self).__name__}' object has no attribute '{key}'")             # <<<<<<<<<<<<<<
  * 
  *     def __setattr__(self, key, value):
  */
   __pyx_t_2 = PyTuple_New(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
@@ -7266,82 +7261,82 @@
   __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_AttributeError, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_Raise(__pyx_t_2, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __PYX_ERR(0, 88, __pyx_L1_error)
 
-  /* "pop/pop.data.pyx":85
+  /* "data.pyx":85
  *             return ImmutableNamespaceDict()
  * 
  *     def __getattr__(self, key):             # <<<<<<<<<<<<<<
  *         if key in self.__data:
  *             return self.__data[key]
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__getattr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.__getattr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":90
+/* "data.pyx":90
  *         raise AttributeError(f"'{type(self).__name__}' object has no attribute '{key}'")
  * 
  *     def __setattr__(self, key, value):             # <<<<<<<<<<<<<<
  *         if key == '_ImmutableNamespaceDict__data':
  *             object.__setattr__(self, key, value)
  */
 
 /* Python wrapper */
-static int __pyx_pw_3pop_4data_22ImmutableNamespaceDict_7__setattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value); /*proto*/
-static int __pyx_pw_3pop_4data_22ImmutableNamespaceDict_7__setattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value) {
+static int __pyx_pw_4data_22ImmutableNamespaceDict_7__setattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value); /*proto*/
+static int __pyx_pw_4data_22ImmutableNamespaceDict_7__setattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setattr__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_6__setattr__(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self), ((PyObject *)__pyx_v_key), ((PyObject *)__pyx_v_value));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_6__setattr__(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self), ((PyObject *)__pyx_v_key), ((PyObject *)__pyx_v_value));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_3pop_4data_22ImmutableNamespaceDict_6__setattr__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value) {
+static int __pyx_pf_4data_22ImmutableNamespaceDict_6__setattr__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setattr__", 1);
 
-  /* "pop/pop.data.pyx":91
+  /* "data.pyx":91
  * 
  *     def __setattr__(self, key, value):
  *         if key == '_ImmutableNamespaceDict__data':             # <<<<<<<<<<<<<<
  *             object.__setattr__(self, key, value)
  *         else:
  */
   __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_key, __pyx_n_u_ImmutableNamespaceDict__data, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 91, __pyx_L1_error)
   if (likely(__pyx_t_1)) {
 
-    /* "pop/pop.data.pyx":92
+    /* "data.pyx":92
  *     def __setattr__(self, key, value):
  *         if key == '_ImmutableNamespaceDict__data':
  *             object.__setattr__(self, key, value)             # <<<<<<<<<<<<<<
  *         else:
  *             raise TypeError("ImmutableNamespaceDict does not support attribute assignment")
  */
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_builtin_object, __pyx_n_s_setattr); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
@@ -7366,25 +7361,25 @@
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pop/pop.data.pyx":91
+    /* "data.pyx":91
  * 
  *     def __setattr__(self, key, value):
  *         if key == '_ImmutableNamespaceDict__data':             # <<<<<<<<<<<<<<
  *             object.__setattr__(self, key, value)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "pop/pop.data.pyx":94
+  /* "data.pyx":94
  *             object.__setattr__(self, key, value)
  *         else:
  *             raise TypeError("ImmutableNamespaceDict does not support attribute assignment")             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(self, key, value):
  */
   /*else*/ {
@@ -7392,143 +7387,143 @@
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 94, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "pop/pop.data.pyx":90
+  /* "data.pyx":90
  *         raise AttributeError(f"'{type(self).__name__}' object has no attribute '{key}'")
  * 
  *     def __setattr__(self, key, value):             # <<<<<<<<<<<<<<
  *         if key == '_ImmutableNamespaceDict__data':
  *             object.__setattr__(self, key, value)
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__setattr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.__setattr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":96
+/* "data.pyx":96
  *             raise TypeError("ImmutableNamespaceDict does not support attribute assignment")
  * 
  *     def __setitem__(self, key, value):             # <<<<<<<<<<<<<<
  *         raise TypeError("ImmutableNamespaceDict does not support item assignment")
  * 
  */
 
 /* Python wrapper */
-static int __pyx_pw_3pop_4data_22ImmutableNamespaceDict_9__setitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value); /*proto*/
-static int __pyx_pw_3pop_4data_22ImmutableNamespaceDict_9__setitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value) {
+static int __pyx_pw_4data_22ImmutableNamespaceDict_9__setitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value); /*proto*/
+static int __pyx_pw_4data_22ImmutableNamespaceDict_9__setitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_value) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setitem__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_8__setitem__(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self), ((PyObject *)__pyx_v_key), ((PyObject *)__pyx_v_value));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_8__setitem__(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self), ((PyObject *)__pyx_v_key), ((PyObject *)__pyx_v_value));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_3pop_4data_22ImmutableNamespaceDict_8__setitem__(CYTHON_UNUSED struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_key, CYTHON_UNUSED PyObject *__pyx_v_value) {
+static int __pyx_pf_4data_22ImmutableNamespaceDict_8__setitem__(CYTHON_UNUSED struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_key, CYTHON_UNUSED PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setitem__", 1);
 
-  /* "pop/pop.data.pyx":97
+  /* "data.pyx":97
  * 
  *     def __setitem__(self, key, value):
  *         raise TypeError("ImmutableNamespaceDict does not support item assignment")             # <<<<<<<<<<<<<<
  * 
  *     def __call__(self):
  */
   __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 97, __pyx_L1_error)
 
-  /* "pop/pop.data.pyx":96
+  /* "data.pyx":96
  *             raise TypeError("ImmutableNamespaceDict does not support attribute assignment")
  * 
  *     def __setitem__(self, key, value):             # <<<<<<<<<<<<<<
  *         raise TypeError("ImmutableNamespaceDict does not support item assignment")
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__setitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.__setitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":99
+/* "data.pyx":99
  *         raise TypeError("ImmutableNamespaceDict does not support item assignment")
  * 
  *     def __call__(self):             # <<<<<<<<<<<<<<
  *         return unfreeze(self.__data)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_11__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_11__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_11__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_11__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__call__ (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__call__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_VARARGS(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__call__", 0))) return NULL;
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_10__call__(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_10__call__(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_10__call__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self) {
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_10__call__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 1);
 
-  /* "pop/pop.data.pyx":100
+  /* "data.pyx":100
  * 
  *     def __call__(self):
  *         return unfreeze(self.__data)             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -7556,69 +7551,69 @@
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pop/pop.data.pyx":99
+  /* "data.pyx":99
  *         raise TypeError("ImmutableNamespaceDict does not support item assignment")
  * 
  *     def __call__(self):             # <<<<<<<<<<<<<<
  *         return unfreeze(self.__data)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":102
+/* "data.pyx":102
  *         return unfreeze(self.__data)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self.__data)
  * 
  */
 
 /* Python wrapper */
-static Py_ssize_t __pyx_pw_3pop_4data_22ImmutableNamespaceDict_13__len__(PyObject *__pyx_v_self); /*proto*/
-static Py_ssize_t __pyx_pw_3pop_4data_22ImmutableNamespaceDict_13__len__(PyObject *__pyx_v_self) {
+static Py_ssize_t __pyx_pw_4data_22ImmutableNamespaceDict_13__len__(PyObject *__pyx_v_self); /*proto*/
+static Py_ssize_t __pyx_pw_4data_22ImmutableNamespaceDict_13__len__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__len__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_12__len__(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_12__len__(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static Py_ssize_t __pyx_pf_3pop_4data_22ImmutableNamespaceDict_12__len__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self) {
+static Py_ssize_t __pyx_pf_4data_22ImmutableNamespaceDict_12__len__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self) {
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__len__", 1);
 
-  /* "pop/pop.data.pyx":103
+  /* "data.pyx":103
  * 
  *     def __len__(self):
  *         return len(self.__data)             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __pyx_t_1 = __pyx_v_self->_ImmutableNamespaceDict__data;
@@ -7628,66 +7623,66 @@
     __PYX_ERR(0, 103, __pyx_L1_error)
   }
   __pyx_t_2 = PyDict_Size(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   goto __pyx_L0;
 
-  /* "pop/pop.data.pyx":102
+  /* "data.pyx":102
  *         return unfreeze(self.__data)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self.__data)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__len__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.__len__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":105
+/* "data.pyx":105
  *         return len(self.__data)
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return iter(self.__data)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_15__iter__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_15__iter__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_15__iter__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_15__iter__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__iter__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_14__iter__(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_14__iter__(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_14__iter__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self) {
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_14__iter__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iter__", 1);
 
-  /* "pop/pop.data.pyx":106
+  /* "data.pyx":106
  * 
  *     def __iter__(self):
  *         return iter(self.__data)             # <<<<<<<<<<<<<<
  * 
  *     def __bool__(self):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -7696,262 +7691,262 @@
   __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pop/pop.data.pyx":105
+  /* "data.pyx":105
  *         return len(self.__data)
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return iter(self.__data)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__iter__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.__iter__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":108
+/* "data.pyx":108
  *         return iter(self.__data)
  * 
  *     def __bool__(self):             # <<<<<<<<<<<<<<
  *         return bool(self.__data)
  * 
  */
 
 /* Python wrapper */
-static int __pyx_pw_3pop_4data_22ImmutableNamespaceDict_17__bool__(PyObject *__pyx_v_self); /*proto*/
-static int __pyx_pw_3pop_4data_22ImmutableNamespaceDict_17__bool__(PyObject *__pyx_v_self) {
+static int __pyx_pw_4data_22ImmutableNamespaceDict_17__bool__(PyObject *__pyx_v_self); /*proto*/
+static int __pyx_pw_4data_22ImmutableNamespaceDict_17__bool__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__bool__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_16__bool__(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_16__bool__(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_3pop_4data_22ImmutableNamespaceDict_16__bool__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self) {
+static int __pyx_pf_4data_22ImmutableNamespaceDict_16__bool__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self) {
   int __pyx_r;
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "pop/pop.data.pyx":109
+  /* "data.pyx":109
  * 
  *     def __bool__(self):
  *         return bool(self.__data)             # <<<<<<<<<<<<<<
  * 
  *     def __contains__(self, key):
  */
   __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->_ImmutableNamespaceDict__data); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 109, __pyx_L1_error)
   __pyx_r = (!(!__pyx_t_1));
   goto __pyx_L0;
 
-  /* "pop/pop.data.pyx":108
+  /* "data.pyx":108
  *         return iter(self.__data)
  * 
  *     def __bool__(self):             # <<<<<<<<<<<<<<
  *         return bool(self.__data)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__bool__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.__bool__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":111
+/* "data.pyx":111
  *         return bool(self.__data)
  * 
  *     def __contains__(self, key):             # <<<<<<<<<<<<<<
  *         return key in self.__data
  * 
  */
 
 /* Python wrapper */
-static int __pyx_pw_3pop_4data_22ImmutableNamespaceDict_19__contains__(PyObject *__pyx_v_self, PyObject *__pyx_v_key); /*proto*/
-static int __pyx_pw_3pop_4data_22ImmutableNamespaceDict_19__contains__(PyObject *__pyx_v_self, PyObject *__pyx_v_key) {
+static int __pyx_pw_4data_22ImmutableNamespaceDict_19__contains__(PyObject *__pyx_v_self, PyObject *__pyx_v_key); /*proto*/
+static int __pyx_pw_4data_22ImmutableNamespaceDict_19__contains__(PyObject *__pyx_v_self, PyObject *__pyx_v_key) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__contains__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_18__contains__(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self), ((PyObject *)__pyx_v_key));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_18__contains__(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self), ((PyObject *)__pyx_v_key));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_3pop_4data_22ImmutableNamespaceDict_18__contains__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key) {
+static int __pyx_pf_4data_22ImmutableNamespaceDict_18__contains__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key) {
   int __pyx_r;
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "pop/pop.data.pyx":112
+  /* "data.pyx":112
  * 
  *     def __contains__(self, key):
  *         return key in self.__data             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   if (unlikely(__pyx_v_self->_ImmutableNamespaceDict__data == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
     __PYX_ERR(0, 112, __pyx_L1_error)
   }
   __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_key, __pyx_v_self->_ImmutableNamespaceDict__data, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 112, __pyx_L1_error)
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
-  /* "pop/pop.data.pyx":111
+  /* "data.pyx":111
  *         return bool(self.__data)
  * 
  *     def __contains__(self, key):             # <<<<<<<<<<<<<<
  *         return key in self.__data
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__contains__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.__contains__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":114
+/* "data.pyx":114
  *         return key in self.__data
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f"{self.__data}"
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_21__repr__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_21__repr__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_21__repr__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_21__repr__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__repr__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_20__repr__(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_20__repr__(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_20__repr__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self) {
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_20__repr__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 1);
 
-  /* "pop/pop.data.pyx":115
+  /* "data.pyx":115
  * 
  *     def __repr__(self):
  *         return f"{self.__data}"             # <<<<<<<<<<<<<<
  * 
  *     def __eq__(self, other):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_self->_ImmutableNamespaceDict__data, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pop/pop.data.pyx":114
+  /* "data.pyx":114
  *         return key in self.__data
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f"{self.__data}"
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":117
+/* "data.pyx":117
  *         return f"{self.__data}"
  * 
  *     def __eq__(self, other):             # <<<<<<<<<<<<<<
  *         if isinstance(other, ImmutableNamespaceDict):
  *             return self.__data == other.__data
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_23__eq__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_23__eq__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_23__eq__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_23__eq__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__eq__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_22__eq__(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self), ((PyObject *)__pyx_v_other));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_22__eq__(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self), ((PyObject *)__pyx_v_other));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_22__eq__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_22__eq__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__eq__", 1);
 
-  /* "pop/pop.data.pyx":118
+  /* "data.pyx":118
  * 
  *     def __eq__(self, other):
  *         if isinstance(other, ImmutableNamespaceDict):             # <<<<<<<<<<<<<<
  *             return self.__data == other.__data
  *         elif isinstance(other, dict):
  */
-  __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_other, __pyx_ptype_3pop_4data_ImmutableNamespaceDict); 
+  __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_other, __pyx_ptype_4data_ImmutableNamespaceDict); 
   if (__pyx_t_1) {
 
-    /* "pop/pop.data.pyx":119
+    /* "data.pyx":119
  *     def __eq__(self, other):
  *         if isinstance(other, ImmutableNamespaceDict):
  *             return self.__data == other.__data             # <<<<<<<<<<<<<<
  *         elif isinstance(other, dict):
  *             return self.__data == other
  */
     __Pyx_XDECREF(__pyx_r);
@@ -7959,124 +7954,124 @@
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = PyObject_RichCompare(__pyx_v_self->_ImmutableNamespaceDict__data, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "pop/pop.data.pyx":118
+    /* "data.pyx":118
  * 
  *     def __eq__(self, other):
  *         if isinstance(other, ImmutableNamespaceDict):             # <<<<<<<<<<<<<<
  *             return self.__data == other.__data
  *         elif isinstance(other, dict):
  */
   }
 
-  /* "pop/pop.data.pyx":120
+  /* "data.pyx":120
  *         if isinstance(other, ImmutableNamespaceDict):
  *             return self.__data == other.__data
  *         elif isinstance(other, dict):             # <<<<<<<<<<<<<<
  *             return self.__data == other
  *         return False
  */
   __pyx_t_1 = PyDict_Check(__pyx_v_other); 
   if (__pyx_t_1) {
 
-    /* "pop/pop.data.pyx":121
+    /* "data.pyx":121
  *             return self.__data == other.__data
  *         elif isinstance(other, dict):
  *             return self.__data == other             # <<<<<<<<<<<<<<
  *         return False
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_3 = PyObject_RichCompare(__pyx_v_self->_ImmutableNamespaceDict__data, __pyx_v_other, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "pop/pop.data.pyx":120
+    /* "data.pyx":120
  *         if isinstance(other, ImmutableNamespaceDict):
  *             return self.__data == other.__data
  *         elif isinstance(other, dict):             # <<<<<<<<<<<<<<
  *             return self.__data == other
  *         return False
  */
   }
 
-  /* "pop/pop.data.pyx":122
+  /* "data.pyx":122
  *         elif isinstance(other, dict):
  *             return self.__data == other
  *         return False             # <<<<<<<<<<<<<<
  * 
  *     def __ne__(self, other):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(Py_False);
   __pyx_r = Py_False;
   goto __pyx_L0;
 
-  /* "pop/pop.data.pyx":117
+  /* "data.pyx":117
  *         return f"{self.__data}"
  * 
  *     def __eq__(self, other):             # <<<<<<<<<<<<<<
  *         if isinstance(other, ImmutableNamespaceDict):
  *             return self.__data == other.__data
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__eq__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.__eq__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":124
+/* "data.pyx":124
  *         return False
  * 
  *     def __ne__(self, other):             # <<<<<<<<<<<<<<
  *         return not self.__eq__(other)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_25__ne__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_25__ne__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_25__ne__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_25__ne__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__ne__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_24__ne__(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self), ((PyObject *)__pyx_v_other));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_24__ne__(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self), ((PyObject *)__pyx_v_other));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_24__ne__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_24__ne__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__ne__", 1);
 
-  /* "pop/pop.data.pyx":125
+  /* "data.pyx":125
  * 
  *     def __ne__(self, other):
  *         return not self.__eq__(other)             # <<<<<<<<<<<<<<
  * 
  *     def keys(self):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -8108,53 +8103,53 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_PyBool_FromLong((!__pyx_t_5)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pop/pop.data.pyx":124
+  /* "data.pyx":124
  *         return False
  * 
  *     def __ne__(self, other):             # <<<<<<<<<<<<<<
  *         return not self.__eq__(other)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__ne__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.__ne__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":127
+/* "data.pyx":127
  *         return not self.__eq__(other)
  * 
  *     def keys(self):             # <<<<<<<<<<<<<<
  *         return self.__data.keys()
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_27keys(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_27keys(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_3pop_4data_22ImmutableNamespaceDict_27keys = {"keys", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_27keys, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_27keys(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_4data_22ImmutableNamespaceDict_27keys = {"keys", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_22ImmutableNamespaceDict_27keys, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_27keys(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -8171,31 +8166,31 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("keys", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "keys", 0))) return NULL;
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_26keys(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_26keys(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_26keys(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self) {
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_26keys(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("keys", 1);
 
-  /* "pop/pop.data.pyx":128
+  /* "data.pyx":128
  * 
  *     def keys(self):
  *         return self.__data.keys()             # <<<<<<<<<<<<<<
  * 
  *     def values(self):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -8205,51 +8200,51 @@
   }
   __pyx_t_1 = __Pyx_PyDict_Keys(__pyx_v_self->_ImmutableNamespaceDict__data); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pop/pop.data.pyx":127
+  /* "data.pyx":127
  *         return not self.__eq__(other)
  * 
  *     def keys(self):             # <<<<<<<<<<<<<<
  *         return self.__data.keys()
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.keys", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.keys", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":130
+/* "data.pyx":130
  *         return self.__data.keys()
  * 
  *     def values(self):             # <<<<<<<<<<<<<<
  *         return self.__data.values()
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_29values(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_29values(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_3pop_4data_22ImmutableNamespaceDict_29values = {"values", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_29values, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_29values(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_4data_22ImmutableNamespaceDict_29values = {"values", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_22ImmutableNamespaceDict_29values, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_29values(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -8266,31 +8261,31 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("values", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "values", 0))) return NULL;
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_28values(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_28values(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_28values(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self) {
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_28values(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("values", 1);
 
-  /* "pop/pop.data.pyx":131
+  /* "data.pyx":131
  * 
  *     def values(self):
  *         return self.__data.values()             # <<<<<<<<<<<<<<
  * 
  *     def items(self):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -8300,51 +8295,51 @@
   }
   __pyx_t_1 = __Pyx_PyDict_Values(__pyx_v_self->_ImmutableNamespaceDict__data); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pop/pop.data.pyx":130
+  /* "data.pyx":130
  *         return self.__data.keys()
  * 
  *     def values(self):             # <<<<<<<<<<<<<<
  *         return self.__data.values()
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.values", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.values", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":133
+/* "data.pyx":133
  *         return self.__data.values()
  * 
  *     def items(self):             # <<<<<<<<<<<<<<
  *         return self.__data.items()
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_31items(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_31items(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_3pop_4data_22ImmutableNamespaceDict_31items = {"items", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_31items, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_31items(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_4data_22ImmutableNamespaceDict_31items = {"items", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_22ImmutableNamespaceDict_31items, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_31items(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -8361,31 +8356,31 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("items", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "items", 0))) return NULL;
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_30items(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_30items(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_30items(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self) {
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_30items(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("items", 1);
 
-  /* "pop/pop.data.pyx":134
+  /* "data.pyx":134
  * 
  *     def items(self):
  *         return self.__data.items()             # <<<<<<<<<<<<<<
  * 
  *     def get(self, key, default=None):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -8395,51 +8390,51 @@
   }
   __pyx_t_1 = __Pyx_PyDict_Items(__pyx_v_self->_ImmutableNamespaceDict__data); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pop/pop.data.pyx":133
+  /* "data.pyx":133
  *         return self.__data.values()
  * 
  *     def items(self):             # <<<<<<<<<<<<<<
  *         return self.__data.items()
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.items", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.items", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":136
+/* "data.pyx":136
  *         return self.__data.items()
  * 
  *     def get(self, key, default=None):             # <<<<<<<<<<<<<<
  *         return self.__data.get(key, default)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_33get(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_33get(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_3pop_4data_22ImmutableNamespaceDict_33get = {"get", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_33get, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_33get(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_4data_22ImmutableNamespaceDict_33get = {"get", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_22ImmutableNamespaceDict_33get, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_33get(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_key = 0;
@@ -8517,41 +8512,41 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.get", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.get", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_32get(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self), __pyx_v_key, __pyx_v_default);
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_32get(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self), __pyx_v_key, __pyx_v_default);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_32get(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_default) {
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_32get(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v_key, PyObject *__pyx_v_default) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get", 1);
 
-  /* "pop/pop.data.pyx":137
+  /* "data.pyx":137
  * 
  *     def get(self, key, default=None):
  *         return self.__data.get(key, default)             # <<<<<<<<<<<<<<
  * 
  *     def copy(self):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -8561,51 +8556,51 @@
   }
   __pyx_t_1 = __Pyx_PyDict_GetItemDefault(__pyx_v_self->_ImmutableNamespaceDict__data, __pyx_v_key, __pyx_v_default); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pop/pop.data.pyx":136
+  /* "data.pyx":136
  *         return self.__data.items()
  * 
  *     def get(self, key, default=None):             # <<<<<<<<<<<<<<
  *         return self.__data.get(key, default)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.get", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.get", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":139
+/* "data.pyx":139
  *         return self.__data.get(key, default)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         return unfreeze(self.__data)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_35copy(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_35copy(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_3pop_4data_22ImmutableNamespaceDict_35copy = {"copy", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_35copy, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_35copy(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_4data_22ImmutableNamespaceDict_35copy = {"copy", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_22ImmutableNamespaceDict_35copy, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_35copy(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -8622,34 +8617,34 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("copy", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "copy", 0))) return NULL;
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_34copy(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_34copy(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_34copy(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self) {
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_34copy(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy", 1);
 
-  /* "pop/pop.data.pyx":140
+  /* "data.pyx":140
  * 
  *     def copy(self):
  *         return unfreeze(self.__data)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
@@ -8677,59 +8672,59 @@
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pop/pop.data.pyx":139
+  /* "data.pyx":139
  *         return self.__data.get(key, default)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         return unfreeze(self.__data)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.copy", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.copy", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":69
+/* "data.pyx":69
  * 
  * cdef class ImmutableNamespaceDict:
  *     cdef readonly dict __data             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, data=None):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_29_ImmutableNamespaceDict__data_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_29_ImmutableNamespaceDict__data_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_29_ImmutableNamespaceDict__data_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_29_ImmutableNamespaceDict__data_1__get__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_29_ImmutableNamespaceDict__data___get__(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_29_ImmutableNamespaceDict__data___get__(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_29_ImmutableNamespaceDict__data___get__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self) {
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_29_ImmutableNamespaceDict__data___get__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_ImmutableNamespaceDict__data);
   __pyx_r = __pyx_v_self->_ImmutableNamespaceDict__data;
   goto __pyx_L0;
@@ -8744,23 +8739,23 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_37__reduce_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_37__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_3pop_4data_22ImmutableNamespaceDict_37__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_37__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_37__reduce_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_4data_22ImmutableNamespaceDict_37__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_22ImmutableNamespaceDict_37__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_37__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -8777,22 +8772,22 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_36__reduce_cython__(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self));
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_36__reduce_cython__(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_36__reduce_cython__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self) {
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_36__reduce_cython__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
@@ -8986,15 +8981,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -9004,23 +8999,23 @@
  *     else:
  *         return __pyx_unpickle_ImmutableNamespaceDict, (type(self), 0x9077974, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_ImmutableNamespaceDict__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_39__setstate_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_39__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_3pop_4data_22ImmutableNamespaceDict_39__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_39__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_3pop_4data_22ImmutableNamespaceDict_39__setstate_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_4data_22ImmutableNamespaceDict_39__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_22ImmutableNamespaceDict_39__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4data_22ImmutableNamespaceDict_39__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v___pyx_state = 0;
@@ -9082,47 +9077,47 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_3pop_4data_22ImmutableNamespaceDict_38__setstate_cython__(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v_self), __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_4data_22ImmutableNamespaceDict_38__setstate_cython__(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_22ImmutableNamespaceDict_38__setstate_cython__(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_4data_22ImmutableNamespaceDict_38__setstate_cython__(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_ImmutableNamespaceDict, (type(self), 0x9077974, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_ImmutableNamespaceDict__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
   if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v___pyx_state))) __PYX_ERR(2, 17, __pyx_L1_error)
-  __pyx_t_1 = __pyx_f_3pop_4data___pyx_unpickle_ImmutableNamespaceDict__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_4data___pyx_unpickle_ImmutableNamespaceDict__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_ImmutableNamespaceDict, (type(self), 0x9077974, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
@@ -9130,40 +9125,40 @@
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pop.data.ImmutableNamespaceDict.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.ImmutableNamespaceDict.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":143
+/* "data.pyx":143
  * 
  * 
  * def freeze(data):             # <<<<<<<<<<<<<<
  *     if isinstance(data, ImmutableNamespaceDict):
  *         return data
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_1freeze(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_4data_1freeze(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_3pop_4data_1freeze = {"freeze", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_1freeze, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_3pop_4data_1freeze(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_4data_1freeze = {"freeze", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_1freeze, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4data_1freeze(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_data = 0;
@@ -9225,79 +9220,79 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("pop.data.freeze", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.freeze", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_3pop_4data_freeze(__pyx_self, __pyx_v_data);
+  __pyx_r = __pyx_pf_4data_freeze(__pyx_self, __pyx_v_data);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static PyObject *__pyx_gb_3pop_4data_6freeze_2generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+static PyObject *__pyx_gb_4data_6freeze_2generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "pop/pop.data.pyx":149
+/* "data.pyx":149
  *         return ImmutableNamespaceDict({key: freeze(value) for key, value in data.items()})
  *     elif isinstance(data, list):
  *         return tuple(freeze(value) for value in data)             # <<<<<<<<<<<<<<
  *     elif isinstance(data, set):
  *         return frozenset(freeze(value) for value in data)
  */
 
-static PyObject *__pyx_pf_3pop_4data_6freeze_genexpr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0) {
-  struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr *__pyx_cur_scope;
+static PyObject *__pyx_pf_4data_6freeze_genexpr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0) {
+  struct __pyx_obj_4data___pyx_scope_struct_2_genexpr *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
-  __pyx_cur_scope = (struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr *)__pyx_tp_new_3pop_4data___pyx_scope_struct_2_genexpr(__pyx_ptype_3pop_4data___pyx_scope_struct_2_genexpr, __pyx_empty_tuple, NULL);
+  __pyx_cur_scope = (struct __pyx_obj_4data___pyx_scope_struct_2_genexpr *)__pyx_tp_new_4data___pyx_scope_struct_2_genexpr(__pyx_ptype_4data___pyx_scope_struct_2_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr *)Py_None);
+    __pyx_cur_scope = ((struct __pyx_obj_4data___pyx_scope_struct_2_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 149, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_genexpr_arg_0 = __pyx_genexpr_arg_0;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_3pop_4data_6freeze_2generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_freeze_locals_genexpr, __pyx_n_s_pop_data); if (unlikely(!gen)) __PYX_ERR(0, 149, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_4data_6freeze_2generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_freeze_locals_genexpr, __pyx_n_s_data); if (unlikely(!gen)) __PYX_ERR(0, 149, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_AddTraceback("pop.data.freeze.genexpr", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.freeze.genexpr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_DECREF((PyObject *)__pyx_cur_scope);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_3pop_4data_6freeze_2generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_4data_6freeze_2generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
-  struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr *__pyx_cur_scope = ((struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr *)__pyx_generator->closure);
+  struct __pyx_obj_4data___pyx_scope_struct_2_genexpr *__pyx_cur_scope = ((struct __pyx_obj_4data___pyx_scope_struct_2_genexpr *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   PyObject *(*__pyx_t_3)(PyObject *);
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
@@ -9436,63 +9431,63 @@
   __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static PyObject *__pyx_gb_3pop_4data_6freeze_5generator2(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+static PyObject *__pyx_gb_4data_6freeze_5generator2(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "pop/pop.data.pyx":151
+/* "data.pyx":151
  *         return tuple(freeze(value) for value in data)
  *     elif isinstance(data, set):
  *         return frozenset(freeze(value) for value in data)             # <<<<<<<<<<<<<<
  *     else:
  *         return data
  */
 
-static PyObject *__pyx_pf_3pop_4data_6freeze_3genexpr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0) {
-  struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr *__pyx_cur_scope;
+static PyObject *__pyx_pf_4data_6freeze_3genexpr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0) {
+  struct __pyx_obj_4data___pyx_scope_struct_3_genexpr *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
-  __pyx_cur_scope = (struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr *)__pyx_tp_new_3pop_4data___pyx_scope_struct_3_genexpr(__pyx_ptype_3pop_4data___pyx_scope_struct_3_genexpr, __pyx_empty_tuple, NULL);
+  __pyx_cur_scope = (struct __pyx_obj_4data___pyx_scope_struct_3_genexpr *)__pyx_tp_new_4data___pyx_scope_struct_3_genexpr(__pyx_ptype_4data___pyx_scope_struct_3_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr *)Py_None);
+    __pyx_cur_scope = ((struct __pyx_obj_4data___pyx_scope_struct_3_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 151, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_genexpr_arg_0 = __pyx_genexpr_arg_0;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_3pop_4data_6freeze_5generator2, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_freeze_locals_genexpr, __pyx_n_s_pop_data); if (unlikely(!gen)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_4data_6freeze_5generator2, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_freeze_locals_genexpr, __pyx_n_s_data); if (unlikely(!gen)) __PYX_ERR(0, 151, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_AddTraceback("pop.data.freeze.genexpr", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.freeze.genexpr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_DECREF((PyObject *)__pyx_cur_scope);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_3pop_4data_6freeze_5generator2(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_4data_6freeze_5generator2(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
-  struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr *__pyx_cur_scope = ((struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr *)__pyx_generator->closure);
+  struct __pyx_obj_4data___pyx_scope_struct_3_genexpr *__pyx_cur_scope = ((struct __pyx_obj_4data___pyx_scope_struct_3_genexpr *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   PyObject *(*__pyx_t_3)(PyObject *);
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
@@ -9632,27 +9627,27 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":143
+/* "data.pyx":143
  * 
  * 
  * def freeze(data):             # <<<<<<<<<<<<<<
  *     if isinstance(data, ImmutableNamespaceDict):
  *         return data
  */
 
-static PyObject *__pyx_pf_3pop_4data_freeze(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data) {
+static PyObject *__pyx_pf_4data_freeze(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data) {
   PyObject *__pyx_8genexpr3__pyx_v_key = NULL;
   PyObject *__pyx_8genexpr3__pyx_v_value = NULL;
-  PyObject *__pyx_gb_3pop_4data_6freeze_2generator1 = 0;
-  PyObject *__pyx_gb_3pop_4data_6freeze_5generator2 = 0;
+  PyObject *__pyx_gb_4data_6freeze_2generator1 = 0;
+  PyObject *__pyx_gb_4data_6freeze_5generator2 = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
@@ -9662,56 +9657,56 @@
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("freeze", 1);
 
-  /* "pop/pop.data.pyx":144
+  /* "data.pyx":144
  * 
  * def freeze(data):
  *     if isinstance(data, ImmutableNamespaceDict):             # <<<<<<<<<<<<<<
  *         return data
  *     elif isinstance(data, dict):
  */
-  __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_data, __pyx_ptype_3pop_4data_ImmutableNamespaceDict); 
+  __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_data, __pyx_ptype_4data_ImmutableNamespaceDict); 
   if (__pyx_t_1) {
 
-    /* "pop/pop.data.pyx":145
+    /* "data.pyx":145
  * def freeze(data):
  *     if isinstance(data, ImmutableNamespaceDict):
  *         return data             # <<<<<<<<<<<<<<
  *     elif isinstance(data, dict):
  *         return ImmutableNamespaceDict({key: freeze(value) for key, value in data.items()})
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_data);
     __pyx_r = __pyx_v_data;
     goto __pyx_L0;
 
-    /* "pop/pop.data.pyx":144
+    /* "data.pyx":144
  * 
  * def freeze(data):
  *     if isinstance(data, ImmutableNamespaceDict):             # <<<<<<<<<<<<<<
  *         return data
  *     elif isinstance(data, dict):
  */
   }
 
-  /* "pop/pop.data.pyx":146
+  /* "data.pyx":146
  *     if isinstance(data, ImmutableNamespaceDict):
  *         return data
  *     elif isinstance(data, dict):             # <<<<<<<<<<<<<<
  *         return ImmutableNamespaceDict({key: freeze(value) for key, value in data.items()})
  *     elif isinstance(data, list):
  */
   __pyx_t_1 = PyDict_Check(__pyx_v_data); 
   if (__pyx_t_1) {
 
-    /* "pop/pop.data.pyx":147
+    /* "data.pyx":147
  *         return data
  *     elif isinstance(data, dict):
  *         return ImmutableNamespaceDict({key: freeze(value) for key, value in data.items()})             # <<<<<<<<<<<<<<
  *     elif isinstance(data, list):
  *         return tuple(freeze(value) for value in data)
  */
     __Pyx_XDECREF(__pyx_r);
@@ -9771,161 +9766,161 @@
       goto __pyx_L9_exit_scope;
       __pyx_L6_error:;
       __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_key); __pyx_8genexpr3__pyx_v_key = 0;
       __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_value); __pyx_8genexpr3__pyx_v_value = 0;
       goto __pyx_L1_error;
       __pyx_L9_exit_scope:;
     } /* exit inner scope */
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_3pop_4data_ImmutableNamespaceDict), __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4data_ImmutableNamespaceDict), __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "pop/pop.data.pyx":146
+    /* "data.pyx":146
  *     if isinstance(data, ImmutableNamespaceDict):
  *         return data
  *     elif isinstance(data, dict):             # <<<<<<<<<<<<<<
  *         return ImmutableNamespaceDict({key: freeze(value) for key, value in data.items()})
  *     elif isinstance(data, list):
  */
   }
 
-  /* "pop/pop.data.pyx":148
+  /* "data.pyx":148
  *     elif isinstance(data, dict):
  *         return ImmutableNamespaceDict({key: freeze(value) for key, value in data.items()})
  *     elif isinstance(data, list):             # <<<<<<<<<<<<<<
  *         return tuple(freeze(value) for value in data)
  *     elif isinstance(data, set):
  */
   __pyx_t_1 = PyList_Check(__pyx_v_data); 
   if (__pyx_t_1) {
 
-    /* "pop/pop.data.pyx":149
+    /* "data.pyx":149
  *         return ImmutableNamespaceDict({key: freeze(value) for key, value in data.items()})
  *     elif isinstance(data, list):
  *         return tuple(freeze(value) for value in data)             # <<<<<<<<<<<<<<
  *     elif isinstance(data, set):
  *         return frozenset(freeze(value) for value in data)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __pyx_pf_3pop_4data_6freeze_genexpr(NULL, __pyx_v_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
+    __pyx_t_3 = __pyx_pf_4data_6freeze_genexpr(NULL, __pyx_v_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_2 = __Pyx_PySequence_Tuple(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "pop/pop.data.pyx":148
+    /* "data.pyx":148
  *     elif isinstance(data, dict):
  *         return ImmutableNamespaceDict({key: freeze(value) for key, value in data.items()})
  *     elif isinstance(data, list):             # <<<<<<<<<<<<<<
  *         return tuple(freeze(value) for value in data)
  *     elif isinstance(data, set):
  */
   }
 
-  /* "pop/pop.data.pyx":150
+  /* "data.pyx":150
  *     elif isinstance(data, list):
  *         return tuple(freeze(value) for value in data)
  *     elif isinstance(data, set):             # <<<<<<<<<<<<<<
  *         return frozenset(freeze(value) for value in data)
  *     else:
  */
   __pyx_t_1 = PySet_Check(__pyx_v_data); 
   if (__pyx_t_1) {
 
-    /* "pop/pop.data.pyx":151
+    /* "data.pyx":151
  *         return tuple(freeze(value) for value in data)
  *     elif isinstance(data, set):
  *         return frozenset(freeze(value) for value in data)             # <<<<<<<<<<<<<<
  *     else:
  *         return data
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __pyx_pf_3pop_4data_6freeze_3genexpr(NULL, __pyx_v_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_2 = __pyx_pf_4data_6freeze_3genexpr(NULL, __pyx_v_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 151, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = __Pyx_PyFrozenSet_New(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 151, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "pop/pop.data.pyx":150
+    /* "data.pyx":150
  *     elif isinstance(data, list):
  *         return tuple(freeze(value) for value in data)
  *     elif isinstance(data, set):             # <<<<<<<<<<<<<<
  *         return frozenset(freeze(value) for value in data)
  *     else:
  */
   }
 
-  /* "pop/pop.data.pyx":153
+  /* "data.pyx":153
  *         return frozenset(freeze(value) for value in data)
  *     else:
  *         return data             # <<<<<<<<<<<<<<
  * 
  * def unfreeze(data):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_data);
     __pyx_r = __pyx_v_data;
     goto __pyx_L0;
   }
 
-  /* "pop/pop.data.pyx":143
+  /* "data.pyx":143
  * 
  * 
  * def freeze(data):             # <<<<<<<<<<<<<<
  *     if isinstance(data, ImmutableNamespaceDict):
  *         return data
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_AddTraceback("pop.data.freeze", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.freeze", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_key);
   __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_value);
-  __Pyx_XDECREF(__pyx_gb_3pop_4data_6freeze_2generator1);
-  __Pyx_XDECREF(__pyx_gb_3pop_4data_6freeze_5generator2);
+  __Pyx_XDECREF(__pyx_gb_4data_6freeze_2generator1);
+  __Pyx_XDECREF(__pyx_gb_4data_6freeze_5generator2);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":155
+/* "data.pyx":155
  *         return data
  * 
  * def unfreeze(data):             # <<<<<<<<<<<<<<
  *     if isinstance(data, ImmutableNamespaceDict):
  *         return {key: unfreeze(value) for key, value in data.items()}
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_3unfreeze(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_4data_3unfreeze(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_3pop_4data_3unfreeze = {"unfreeze", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_3unfreeze, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_3pop_4data_3unfreeze(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_4data_3unfreeze = {"unfreeze", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_3unfreeze, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4data_3unfreeze(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_data = 0;
@@ -9987,32 +9982,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("pop.data.unfreeze", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.unfreeze", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_3pop_4data_2unfreeze(__pyx_self, __pyx_v_data);
+  __pyx_r = __pyx_pf_4data_2unfreeze(__pyx_self, __pyx_v_data);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_2unfreeze(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data) {
+static PyObject *__pyx_pf_4data_2unfreeze(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data) {
   PyObject *__pyx_8genexpr6__pyx_v_key = NULL;
   PyObject *__pyx_8genexpr6__pyx_v_value = NULL;
   PyObject *__pyx_8genexpr7__pyx_v_value = NULL;
   PyObject *__pyx_8genexpr8__pyx_v_value = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
@@ -10027,25 +10022,25 @@
   PyObject *__pyx_t_10 = NULL;
   PyObject *(*__pyx_t_11)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("unfreeze", 1);
 
-  /* "pop/pop.data.pyx":156
+  /* "data.pyx":156
  * 
  * def unfreeze(data):
  *     if isinstance(data, ImmutableNamespaceDict):             # <<<<<<<<<<<<<<
  *         return {key: unfreeze(value) for key, value in data.items()}
  *     elif isinstance(data, frozenset):
  */
-  __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_data, __pyx_ptype_3pop_4data_ImmutableNamespaceDict); 
+  __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_data, __pyx_ptype_4data_ImmutableNamespaceDict); 
   if (__pyx_t_1) {
 
-    /* "pop/pop.data.pyx":157
+    /* "data.pyx":157
  * def unfreeze(data):
  *     if isinstance(data, ImmutableNamespaceDict):
  *         return {key: unfreeze(value) for key, value in data.items()}             # <<<<<<<<<<<<<<
  *     elif isinstance(data, frozenset):
  *         return {unfreeze(value) for value in data}
  */
     __Pyx_XDECREF(__pyx_r);
@@ -10109,34 +10104,34 @@
       goto __pyx_L1_error;
       __pyx_L9_exit_scope:;
     } /* exit inner scope */
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "pop/pop.data.pyx":156
+    /* "data.pyx":156
  * 
  * def unfreeze(data):
  *     if isinstance(data, ImmutableNamespaceDict):             # <<<<<<<<<<<<<<
  *         return {key: unfreeze(value) for key, value in data.items()}
  *     elif isinstance(data, frozenset):
  */
   }
 
-  /* "pop/pop.data.pyx":158
+  /* "data.pyx":158
  *     if isinstance(data, ImmutableNamespaceDict):
  *         return {key: unfreeze(value) for key, value in data.items()}
  *     elif isinstance(data, frozenset):             # <<<<<<<<<<<<<<
  *         return {unfreeze(value) for value in data}
  *     elif isinstance(data, tuple):
  */
   __pyx_t_1 = PyFrozenSet_Check(__pyx_v_data); 
   if (__pyx_t_1) {
 
-    /* "pop/pop.data.pyx":159
+    /* "data.pyx":159
  *         return {key: unfreeze(value) for key, value in data.items()}
  *     elif isinstance(data, frozenset):
  *         return {unfreeze(value) for value in data}             # <<<<<<<<<<<<<<
  *     elif isinstance(data, tuple):
  *         return [unfreeze(value) for value in data]
  */
     __Pyx_XDECREF(__pyx_r);
@@ -10232,34 +10227,34 @@
       goto __pyx_L1_error;
       __pyx_L16_exit_scope:;
     } /* exit inner scope */
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "pop/pop.data.pyx":158
+    /* "data.pyx":158
  *     if isinstance(data, ImmutableNamespaceDict):
  *         return {key: unfreeze(value) for key, value in data.items()}
  *     elif isinstance(data, frozenset):             # <<<<<<<<<<<<<<
  *         return {unfreeze(value) for value in data}
  *     elif isinstance(data, tuple):
  */
   }
 
-  /* "pop/pop.data.pyx":160
+  /* "data.pyx":160
  *     elif isinstance(data, frozenset):
  *         return {unfreeze(value) for value in data}
  *     elif isinstance(data, tuple):             # <<<<<<<<<<<<<<
  *         return [unfreeze(value) for value in data]
  *     else:
  */
   __pyx_t_1 = PyTuple_Check(__pyx_v_data); 
   if (__pyx_t_1) {
 
-    /* "pop/pop.data.pyx":161
+    /* "data.pyx":161
  *         return {unfreeze(value) for value in data}
  *     elif isinstance(data, tuple):
  *         return [unfreeze(value) for value in data]             # <<<<<<<<<<<<<<
  *     else:
  *         return data
  */
     __Pyx_XDECREF(__pyx_r);
@@ -10355,80 +10350,80 @@
       goto __pyx_L1_error;
       __pyx_L23_exit_scope:;
     } /* exit inner scope */
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "pop/pop.data.pyx":160
+    /* "data.pyx":160
  *     elif isinstance(data, frozenset):
  *         return {unfreeze(value) for value in data}
  *     elif isinstance(data, tuple):             # <<<<<<<<<<<<<<
  *         return [unfreeze(value) for value in data]
  *     else:
  */
   }
 
-  /* "pop/pop.data.pyx":163
+  /* "data.pyx":163
  *         return [unfreeze(value) for value in data]
  *     else:
  *         return data             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_data);
     __pyx_r = __pyx_v_data;
     goto __pyx_L0;
   }
 
-  /* "pop/pop.data.pyx":155
+  /* "data.pyx":155
  *         return data
  * 
  * def unfreeze(data):             # <<<<<<<<<<<<<<
  *     if isinstance(data, ImmutableNamespaceDict):
  *         return {key: unfreeze(value) for key, value in data.items()}
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_AddTraceback("pop.data.unfreeze", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.unfreeze", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_key);
   __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_value);
   __Pyx_XDECREF(__pyx_8genexpr7__pyx_v_value);
   __Pyx_XDECREF(__pyx_8genexpr8__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pop/pop.data.pyx":166
+/* "data.pyx":166
  * 
  * 
  * cpdef update(dest, upd, bint recursive_update=True, bint merge_lists=False):             # <<<<<<<<<<<<<<
  *     """
  *     Recursive version of the default dict.update
  */
 
-static PyObject *__pyx_pw_3pop_4data_5update(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_4data_5update(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyObject *__pyx_f_3pop_4data_update(PyObject *__pyx_v_dest, PyObject *__pyx_v_upd, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_3pop_4data_update *__pyx_optional_args) {
+static PyObject *__pyx_f_4data_update(PyObject *__pyx_v_dest, PyObject *__pyx_v_upd, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_4data_update *__pyx_optional_args) {
   int __pyx_v_recursive_update = ((int)1);
   int __pyx_v_merge_lists = ((int)0);
   PyObject *__pyx_v_keys = 0;
   PyObject *__pyx_v_key = 0;
   PyObject *__pyx_v_val = 0;
   PyObject *__pyx_v_dest_subkey = 0;
   PyObject *__pyx_v_ret = NULL;
@@ -10457,15 +10452,15 @@
       __pyx_v_recursive_update = __pyx_optional_args->recursive_update;
       if (__pyx_optional_args->__pyx_n > 1) {
         __pyx_v_merge_lists = __pyx_optional_args->merge_lists;
       }
     }
   }
 
-  /* "pop/pop.data.pyx":181
+  /* "data.pyx":181
  *     """
  *     cdef:
  *         list keys = list(upd.keys())             # <<<<<<<<<<<<<<
  *         object key, val, dest_subkey
  * 
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_upd, __pyx_n_s_keys); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
@@ -10494,24 +10489,24 @@
   }
   __pyx_t_2 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_keys = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pop/pop.data.pyx":184
+  /* "data.pyx":184
  *         object key, val, dest_subkey
  * 
  *     if recursive_update:             # <<<<<<<<<<<<<<
  *         for key in keys:
  *             val = upd[key]
  */
   if (__pyx_v_recursive_update) {
 
-    /* "pop/pop.data.pyx":185
+    /* "data.pyx":185
  * 
  *     if recursive_update:
  *         for key in keys:             # <<<<<<<<<<<<<<
  *             val = upd[key]
  *             dest_subkey = dest.get(key, None)
  */
     __pyx_t_2 = __pyx_v_keys; __Pyx_INCREF(__pyx_t_2);
@@ -10529,27 +10524,27 @@
       #else
       __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #endif
       __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "pop/pop.data.pyx":186
+      /* "data.pyx":186
  *     if recursive_update:
  *         for key in keys:
  *             val = upd[key]             # <<<<<<<<<<<<<<
  *             dest_subkey = dest.get(key, None)
  *             if isinstance(dest_subkey, Mapping) and isinstance(val, Mapping):
  */
       __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_upd, __pyx_v_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_val, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "pop/pop.data.pyx":187
+      /* "data.pyx":187
  *         for key in keys:
  *             val = upd[key]
  *             dest_subkey = dest.get(key, None)             # <<<<<<<<<<<<<<
  *             if isinstance(dest_subkey, Mapping) and isinstance(val, Mapping):
  *                 ret = update(dest_subkey, val, merge_lists=merge_lists)
  */
       __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_dest, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 187, __pyx_L1_error)
@@ -10575,15 +10570,15 @@
         if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
       __Pyx_XDECREF_SET(__pyx_v_dest_subkey, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "pop/pop.data.pyx":188
+      /* "data.pyx":188
  *             val = upd[key]
  *             dest_subkey = dest.get(key, None)
  *             if isinstance(dest_subkey, Mapping) and isinstance(val, Mapping):             # <<<<<<<<<<<<<<
  *                 ret = update(dest_subkey, val, merge_lists=merge_lists)
  *                 dest[key] = ret
  */
       __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Mapping); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
@@ -10599,15 +10594,15 @@
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_8 = PyObject_IsInstance(__pyx_v_val, __pyx_t_1); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 188, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_7 = __pyx_t_8;
       __pyx_L7_bool_binop_done:;
       if (__pyx_t_7) {
 
-        /* "pop/pop.data.pyx":189
+        /* "data.pyx":189
  *             dest_subkey = dest.get(key, None)
  *             if isinstance(dest_subkey, Mapping) and isinstance(val, Mapping):
  *                 ret = update(dest_subkey, val, merge_lists=merge_lists)             # <<<<<<<<<<<<<<
  *                 dest[key] = ret
  *             elif isinstance(dest_subkey, list) and isinstance(val, list) and merge_lists:
  */
         __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_update); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
@@ -10630,34 +10625,34 @@
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_XDECREF_SET(__pyx_v_ret, __pyx_t_9);
         __pyx_t_9 = 0;
 
-        /* "pop/pop.data.pyx":190
+        /* "data.pyx":190
  *             if isinstance(dest_subkey, Mapping) and isinstance(val, Mapping):
  *                 ret = update(dest_subkey, val, merge_lists=merge_lists)
  *                 dest[key] = ret             # <<<<<<<<<<<<<<
  *             elif isinstance(dest_subkey, list) and isinstance(val, list) and merge_lists:
  *                 merged = dest_subkey[:]
  */
         if (unlikely((PyObject_SetItem(__pyx_v_dest, __pyx_v_key, __pyx_v_ret) < 0))) __PYX_ERR(0, 190, __pyx_L1_error)
 
-        /* "pop/pop.data.pyx":188
+        /* "data.pyx":188
  *             val = upd[key]
  *             dest_subkey = dest.get(key, None)
  *             if isinstance(dest_subkey, Mapping) and isinstance(val, Mapping):             # <<<<<<<<<<<<<<
  *                 ret = update(dest_subkey, val, merge_lists=merge_lists)
  *                 dest[key] = ret
  */
         goto __pyx_L6;
       }
 
-      /* "pop/pop.data.pyx":191
+      /* "data.pyx":191
  *                 ret = update(dest_subkey, val, merge_lists=merge_lists)
  *                 dest[key] = ret
  *             elif isinstance(dest_subkey, list) and isinstance(val, list) and merge_lists:             # <<<<<<<<<<<<<<
  *                 merged = dest_subkey[:]
  *                 merged.extend([x for x in val if x not in merged])
  */
       __pyx_t_8 = PyList_Check(__pyx_v_dest_subkey); 
@@ -10672,27 +10667,27 @@
         __pyx_t_7 = __pyx_t_8;
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_7 = __pyx_v_merge_lists;
       __pyx_L9_bool_binop_done:;
       if (__pyx_t_7) {
 
-        /* "pop/pop.data.pyx":192
+        /* "data.pyx":192
  *                 dest[key] = ret
  *             elif isinstance(dest_subkey, list) and isinstance(val, list) and merge_lists:
  *                 merged = dest_subkey[:]             # <<<<<<<<<<<<<<
  *                 merged.extend([x for x in val if x not in merged])
  *                 dest[key] = merged
  */
         __pyx_t_9 = __Pyx_PyObject_GetSlice(__pyx_v_dest_subkey, 0, 0, NULL, NULL, &__pyx_slice__6, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 192, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_XDECREF_SET(__pyx_v_merged, __pyx_t_9);
         __pyx_t_9 = 0;
 
-        /* "pop/pop.data.pyx":193
+        /* "data.pyx":193
  *             elif isinstance(dest_subkey, list) and isinstance(val, list) and merge_lists:
  *                 merged = dest_subkey[:]
  *                 merged.extend([x for x in val if x not in merged])             # <<<<<<<<<<<<<<
  *                 dest[key] = merged
  *             else:
  */
         __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_merged, __pyx_n_s_extend); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 193, __pyx_L1_error)
@@ -10788,69 +10783,69 @@
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 193, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-        /* "pop/pop.data.pyx":194
+        /* "data.pyx":194
  *                 merged = dest_subkey[:]
  *                 merged.extend([x for x in val if x not in merged])
  *                 dest[key] = merged             # <<<<<<<<<<<<<<
  *             else:
  *                 dest[key] = upd[key]
  */
         if (unlikely((PyObject_SetItem(__pyx_v_dest, __pyx_v_key, __pyx_v_merged) < 0))) __PYX_ERR(0, 194, __pyx_L1_error)
 
-        /* "pop/pop.data.pyx":191
+        /* "data.pyx":191
  *                 ret = update(dest_subkey, val, merge_lists=merge_lists)
  *                 dest[key] = ret
  *             elif isinstance(dest_subkey, list) and isinstance(val, list) and merge_lists:             # <<<<<<<<<<<<<<
  *                 merged = dest_subkey[:]
  *                 merged.extend([x for x in val if x not in merged])
  */
         goto __pyx_L6;
       }
 
-      /* "pop/pop.data.pyx":196
+      /* "data.pyx":196
  *                 dest[key] = merged
  *             else:
  *                 dest[key] = upd[key]             # <<<<<<<<<<<<<<
  *     else:
  *         for key in keys:
  */
       /*else*/ {
         __pyx_t_9 = __Pyx_PyObject_GetItem(__pyx_v_upd, __pyx_v_key); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 196, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         if (unlikely((PyObject_SetItem(__pyx_v_dest, __pyx_v_key, __pyx_t_9) < 0))) __PYX_ERR(0, 196, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
       __pyx_L6:;
 
-      /* "pop/pop.data.pyx":185
+      /* "data.pyx":185
  * 
  *     if recursive_update:
  *         for key in keys:             # <<<<<<<<<<<<<<
  *             val = upd[key]
  *             dest_subkey = dest.get(key, None)
  */
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pop/pop.data.pyx":184
+    /* "data.pyx":184
  *         object key, val, dest_subkey
  * 
  *     if recursive_update:             # <<<<<<<<<<<<<<
  *         for key in keys:
  *             val = upd[key]
  */
     goto __pyx_L3;
   }
 
-  /* "pop/pop.data.pyx":198
+  /* "data.pyx":198
  *                 dest[key] = upd[key]
  *     else:
  *         for key in keys:             # <<<<<<<<<<<<<<
  *             dest[key] = upd[key]
  *     return dest
  */
   /*else*/ {
@@ -10869,48 +10864,48 @@
       #else
       __pyx_t_9 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       #endif
       __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_9);
       __pyx_t_9 = 0;
 
-      /* "pop/pop.data.pyx":199
+      /* "data.pyx":199
  *     else:
  *         for key in keys:
  *             dest[key] = upd[key]             # <<<<<<<<<<<<<<
  *     return dest
  */
       __pyx_t_9 = __Pyx_PyObject_GetItem(__pyx_v_upd, __pyx_v_key); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 199, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       if (unlikely((PyObject_SetItem(__pyx_v_dest, __pyx_v_key, __pyx_t_9) < 0))) __PYX_ERR(0, 199, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-      /* "pop/pop.data.pyx":198
+      /* "data.pyx":198
  *                 dest[key] = upd[key]
  *     else:
  *         for key in keys:             # <<<<<<<<<<<<<<
  *             dest[key] = upd[key]
  *     return dest
  */
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_L3:;
 
-  /* "pop/pop.data.pyx":200
+  /* "data.pyx":200
  *         for key in keys:
  *             dest[key] = upd[key]
  *     return dest             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_dest);
   __pyx_r = __pyx_v_dest;
   goto __pyx_L0;
 
-  /* "pop/pop.data.pyx":166
+  /* "data.pyx":166
  * 
  * 
  * cpdef update(dest, upd, bint recursive_update=True, bint merge_lists=False):             # <<<<<<<<<<<<<<
  *     """
  *     Recursive version of the default dict.update
  */
 
@@ -10918,15 +10913,15 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_12);
-  __Pyx_AddTraceback("pop.data.update", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.update", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_keys);
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XDECREF(__pyx_v_val);
   __Pyx_XDECREF(__pyx_v_dest_subkey);
   __Pyx_XDECREF(__pyx_v_ret);
@@ -10934,24 +10929,24 @@
   __Pyx_XDECREF(__pyx_8genexpr9__pyx_v_x);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_5update(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_4data_5update(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_3pop_4data_4update, "\n    Recursive version of the default dict.update\n\n    Merges upd recursively into dest\n\n    If recursive_update=False, will use the classic dict.update, or fall back\n    on a manual merge (helpful for non-dict types like FunctionWrapper)\n\n    If merge_lists=True, will aggregate list object types instead of replace.\n    The list in ``upd`` is added to the list in ``dest``, so the resulting list\n    is ``dest[key] + upd[key]``. This behavior is only activated when\n    recursive_update=True. By default merge_lists=False.\n    ");
-static PyMethodDef __pyx_mdef_3pop_4data_5update = {"update", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_5update, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_3pop_4data_4update};
-static PyObject *__pyx_pw_3pop_4data_5update(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_4data_4update, "\n    Recursive version of the default dict.update\n\n    Merges upd recursively into dest\n\n    If recursive_update=False, will use the classic dict.update, or fall back\n    on a manual merge (helpful for non-dict types like FunctionWrapper)\n\n    If merge_lists=True, will aggregate list object types instead of replace.\n    The list in ``upd`` is added to the list in ``dest``, so the resulting list\n    is ``dest[key] + upd[key]``. This behavior is only activated when\n    recursive_update=True. By default merge_lists=False.\n    ");
+static PyMethodDef __pyx_mdef_4data_5update = {"update", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_5update, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_4data_4update};
+static PyObject *__pyx_pw_4data_5update(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_dest = 0;
@@ -11064,77 +11059,77 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("pop.data.update", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.update", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_3pop_4data_4update(__pyx_self, __pyx_v_dest, __pyx_v_upd, __pyx_v_recursive_update, __pyx_v_merge_lists);
+  __pyx_r = __pyx_pf_4data_4update(__pyx_self, __pyx_v_dest, __pyx_v_upd, __pyx_v_recursive_update, __pyx_v_merge_lists);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_4update(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dest, PyObject *__pyx_v_upd, int __pyx_v_recursive_update, int __pyx_v_merge_lists) {
+static PyObject *__pyx_pf_4data_4update(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dest, PyObject *__pyx_v_upd, int __pyx_v_recursive_update, int __pyx_v_merge_lists) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  struct __pyx_opt_args_3pop_4data_update __pyx_t_2;
+  struct __pyx_opt_args_4data_update __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("update", 1);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.recursive_update = __pyx_v_recursive_update;
   __pyx_t_2.merge_lists = __pyx_v_merge_lists;
-  __pyx_t_1 = __pyx_f_3pop_4data_update(__pyx_v_dest, __pyx_v_upd, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_4data_update(__pyx_v_dest, __pyx_v_upd, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pop.data.update", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.update", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __pyx_unpickle_NamespaceDict(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_7__pyx_unpickle_NamespaceDict(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_4data_7__pyx_unpickle_NamespaceDict(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_3pop_4data_7__pyx_unpickle_NamespaceDict = {"__pyx_unpickle_NamespaceDict", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_7__pyx_unpickle_NamespaceDict, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_3pop_4data_7__pyx_unpickle_NamespaceDict(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_4data_7__pyx_unpickle_NamespaceDict = {"__pyx_unpickle_NamespaceDict", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_7__pyx_unpickle_NamespaceDict, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4data_7__pyx_unpickle_NamespaceDict(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v___pyx_type = 0;
@@ -11226,32 +11221,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("pop.data.__pyx_unpickle_NamespaceDict", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.__pyx_unpickle_NamespaceDict", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_3pop_4data_6__pyx_unpickle_NamespaceDict(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_4data_6__pyx_unpickle_NamespaceDict(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_6__pyx_unpickle_NamespaceDict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_4data_6__pyx_unpickle_NamespaceDict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
@@ -11325,15 +11320,15 @@
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0xe3b0c44, 0xda39a3e, 0xd41d8cd) = ())" % __pyx_checksum
  *     __pyx_result = NamespaceDict.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_NamespaceDict__set_state(<NamespaceDict> __pyx_result, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_3pop_4data_NamespaceDict), __pyx_n_s_new); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 7, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_4data_NamespaceDict), __pyx_n_s_new); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -11370,15 +11365,15 @@
  *     __pyx_result = NamespaceDict.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_NamespaceDict__set_state(<NamespaceDict> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_NamespaceDict__set_state(NamespaceDict __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v___pyx_state))) __PYX_ERR(2, 9, __pyx_L1_error)
-    __pyx_t_1 = __pyx_f_3pop_4data___pyx_unpickle_NamespaceDict__set_state(((struct __pyx_obj_3pop_4data_NamespaceDict *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_4data___pyx_unpickle_NamespaceDict__set_state(((struct __pyx_obj_4data_NamespaceDict *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0xe3b0c44, 0xda39a3e, 0xd41d8cd) = ())" % __pyx_checksum
  *     __pyx_result = NamespaceDict.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
@@ -11406,15 +11401,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("pop.data.__pyx_unpickle_NamespaceDict", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.__pyx_unpickle_NamespaceDict", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -11424,15 +11419,15 @@
  *         __pyx_unpickle_NamespaceDict__set_state(<NamespaceDict> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_NamespaceDict__set_state(NamespaceDict __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     if len(__pyx_state) > 0 and hasattr(__pyx_result, '__dict__'):
  *         __pyx_result.__dict__.update(__pyx_state[0])
  */
 
-static PyObject *__pyx_f_3pop_4data___pyx_unpickle_NamespaceDict__set_state(struct __pyx_obj_3pop_4data_NamespaceDict *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_f_4data___pyx_unpickle_NamespaceDict__set_state(struct __pyx_obj_4data_NamespaceDict *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -11527,38 +11522,38 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("pop.data.__pyx_unpickle_NamespaceDict__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.__pyx_unpickle_NamespaceDict__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __pyx_unpickle_MultidictCache(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_9__pyx_unpickle_MultidictCache(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_4data_9__pyx_unpickle_MultidictCache(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_3pop_4data_9__pyx_unpickle_MultidictCache = {"__pyx_unpickle_MultidictCache", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_9__pyx_unpickle_MultidictCache, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_3pop_4data_9__pyx_unpickle_MultidictCache(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_4data_9__pyx_unpickle_MultidictCache = {"__pyx_unpickle_MultidictCache", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_9__pyx_unpickle_MultidictCache, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4data_9__pyx_unpickle_MultidictCache(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v___pyx_type = 0;
@@ -11650,32 +11645,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("pop.data.__pyx_unpickle_MultidictCache", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.__pyx_unpickle_MultidictCache", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_3pop_4data_8__pyx_unpickle_MultidictCache(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_4data_8__pyx_unpickle_MultidictCache(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_8__pyx_unpickle_MultidictCache(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_4data_8__pyx_unpickle_MultidictCache(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
@@ -11749,15 +11744,15 @@
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x09e6f20, 0xf4b8e03, 0xd271b3e) = (_base_dicts, _cache, _split_cache))" % __pyx_checksum
  *     __pyx_result = MultidictCache.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_MultidictCache__set_state(<MultidictCache> __pyx_result, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_3pop_4data_MultidictCache), __pyx_n_s_new); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 7, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_4data_MultidictCache), __pyx_n_s_new); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -11794,15 +11789,15 @@
  *     __pyx_result = MultidictCache.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_MultidictCache__set_state(<MultidictCache> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_MultidictCache__set_state(MultidictCache __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v___pyx_state))) __PYX_ERR(2, 9, __pyx_L1_error)
-    __pyx_t_1 = __pyx_f_3pop_4data___pyx_unpickle_MultidictCache__set_state(((struct __pyx_obj_3pop_4data_MultidictCache *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_4data___pyx_unpickle_MultidictCache__set_state(((struct __pyx_obj_4data_MultidictCache *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x09e6f20, 0xf4b8e03, 0xd271b3e) = (_base_dicts, _cache, _split_cache))" % __pyx_checksum
  *     __pyx_result = MultidictCache.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
@@ -11830,15 +11825,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("pop.data.__pyx_unpickle_MultidictCache", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.__pyx_unpickle_MultidictCache", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -11848,15 +11843,15 @@
  *         __pyx_unpickle_MultidictCache__set_state(<MultidictCache> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_MultidictCache__set_state(MultidictCache __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result._base_dicts = __pyx_state[0]; __pyx_result._cache = __pyx_state[1]; __pyx_result._split_cache = __pyx_state[2]
  *     if len(__pyx_state) > 3 and hasattr(__pyx_result, '__dict__'):
  */
 
-static PyObject *__pyx_f_3pop_4data___pyx_unpickle_MultidictCache__set_state(struct __pyx_obj_3pop_4data_MultidictCache *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_f_4data___pyx_unpickle_MultidictCache__set_state(struct __pyx_obj_4data_MultidictCache *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
@@ -11995,38 +11990,38 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("pop.data.__pyx_unpickle_MultidictCache__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.__pyx_unpickle_MultidictCache__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __pyx_unpickle_ImmutableNamespaceDict(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_3pop_4data_11__pyx_unpickle_ImmutableNamespaceDict(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_4data_11__pyx_unpickle_ImmutableNamespaceDict(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_3pop_4data_11__pyx_unpickle_ImmutableNamespaceDict = {"__pyx_unpickle_ImmutableNamespaceDict", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_11__pyx_unpickle_ImmutableNamespaceDict, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_3pop_4data_11__pyx_unpickle_ImmutableNamespaceDict(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_4data_11__pyx_unpickle_ImmutableNamespaceDict = {"__pyx_unpickle_ImmutableNamespaceDict", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_11__pyx_unpickle_ImmutableNamespaceDict, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4data_11__pyx_unpickle_ImmutableNamespaceDict(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v___pyx_type = 0;
@@ -12118,32 +12113,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("pop.data.__pyx_unpickle_ImmutableNamespaceDict", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.__pyx_unpickle_ImmutableNamespaceDict", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_3pop_4data_10__pyx_unpickle_ImmutableNamespaceDict(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_4data_10__pyx_unpickle_ImmutableNamespaceDict(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_3pop_4data_10__pyx_unpickle_ImmutableNamespaceDict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_4data_10__pyx_unpickle_ImmutableNamespaceDict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
@@ -12217,15 +12212,15 @@
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x9077974, 0xccb23f1, 0x45e2a8b) = (_ImmutableNamespaceDict__data))" % __pyx_checksum
  *     __pyx_result = ImmutableNamespaceDict.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_ImmutableNamespaceDict__set_state(<ImmutableNamespaceDict> __pyx_result, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_3pop_4data_ImmutableNamespaceDict), __pyx_n_s_new); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 7, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_4data_ImmutableNamespaceDict), __pyx_n_s_new); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -12262,15 +12257,15 @@
  *     __pyx_result = ImmutableNamespaceDict.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_ImmutableNamespaceDict__set_state(<ImmutableNamespaceDict> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_ImmutableNamespaceDict__set_state(ImmutableNamespaceDict __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v___pyx_state))) __PYX_ERR(2, 9, __pyx_L1_error)
-    __pyx_t_1 = __pyx_f_3pop_4data___pyx_unpickle_ImmutableNamespaceDict__set_state(((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_4data___pyx_unpickle_ImmutableNamespaceDict__set_state(((struct __pyx_obj_4data_ImmutableNamespaceDict *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x9077974, 0xccb23f1, 0x45e2a8b) = (_ImmutableNamespaceDict__data))" % __pyx_checksum
  *     __pyx_result = ImmutableNamespaceDict.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
@@ -12298,15 +12293,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("pop.data.__pyx_unpickle_ImmutableNamespaceDict", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.__pyx_unpickle_ImmutableNamespaceDict", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -12316,15 +12311,15 @@
  *         __pyx_unpickle_ImmutableNamespaceDict__set_state(<ImmutableNamespaceDict> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_ImmutableNamespaceDict__set_state(ImmutableNamespaceDict __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result._ImmutableNamespaceDict__data = __pyx_state[0]
  *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
  */
 
-static PyObject *__pyx_f_3pop_4data___pyx_unpickle_ImmutableNamespaceDict__set_state(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_f_4data___pyx_unpickle_ImmutableNamespaceDict__set_state(struct __pyx_obj_4data_ImmutableNamespaceDict *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
@@ -12439,81 +12434,81 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("pop.data.__pyx_unpickle_ImmutableNamespaceDict__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("data.__pyx_unpickle_ImmutableNamespaceDict__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_tp_traverse_3pop_4data_NamespaceDict(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_4data_NamespaceDict(PyObject *o, visitproc v, void *a) {
   int e;
   if (!(&PyDict_Type)->tp_traverse); else { e = (&PyDict_Type)->tp_traverse(o,v,a); if (e) return e; }
   return 0;
 }
 
-static int __pyx_tp_clear_3pop_4data_NamespaceDict(PyObject *o) {
+static int __pyx_tp_clear_4data_NamespaceDict(PyObject *o) {
   if (!(&PyDict_Type)->tp_clear); else (&PyDict_Type)->tp_clear(o);
   return 0;
 }
 
-static PyObject *__pyx_tp_getattro_3pop_4data_NamespaceDict(PyObject *o, PyObject *n) {
+static PyObject *__pyx_tp_getattro_4data_NamespaceDict(PyObject *o, PyObject *n) {
   PyObject *v = __Pyx_PyObject_GenericGetAttr(o, n);
   if (!v && PyErr_ExceptionMatches(PyExc_AttributeError)) {
     PyErr_Clear();
-    v = __pyx_pw_3pop_4data_13NamespaceDict_1__getattr__(o, n);
+    v = __pyx_pw_4data_13NamespaceDict_1__getattr__(o, n);
   }
   return v;
 }
 
-static int __pyx_tp_setattro_3pop_4data_NamespaceDict(PyObject *o, PyObject *n, PyObject *v) {
+static int __pyx_tp_setattro_4data_NamespaceDict(PyObject *o, PyObject *n, PyObject *v) {
   if (v) {
-    return __pyx_pw_3pop_4data_13NamespaceDict_3__setattr__(o, n, v);
+    return __pyx_pw_4data_13NamespaceDict_3__setattr__(o, n, v);
   }
   else {
     if ((&PyDict_Type)->tp_setattro)
       return (&PyDict_Type)->tp_setattro(o, n, v);
     return PyObject_GenericSetAttr(o, n, 0);
   }
 }
 
-static PyMethodDef __pyx_methods_3pop_4data_NamespaceDict[] = {
-  {"__getattr__", (PyCFunction)__pyx_pw_3pop_4data_13NamespaceDict_1__getattr__, METH_O|METH_COEXIST, 0},
-  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_13NamespaceDict_5__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_13NamespaceDict_7__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+static PyMethodDef __pyx_methods_4data_NamespaceDict[] = {
+  {"__getattr__", (PyCFunction)__pyx_pw_4data_13NamespaceDict_1__getattr__, METH_O|METH_COEXIST, 0},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_13NamespaceDict_5__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_13NamespaceDict_7__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
 #if CYTHON_USE_TYPE_SPECS
-static PyType_Slot __pyx_type_3pop_4data_NamespaceDict_slots[] = {
-  {Py_tp_getattro, (void *)__pyx_tp_getattro_3pop_4data_NamespaceDict},
-  {Py_tp_setattro, (void *)__pyx_tp_setattro_3pop_4data_NamespaceDict},
-  {Py_tp_traverse, (void *)__pyx_tp_traverse_3pop_4data_NamespaceDict},
-  {Py_tp_clear, (void *)__pyx_tp_clear_3pop_4data_NamespaceDict},
-  {Py_tp_methods, (void *)__pyx_methods_3pop_4data_NamespaceDict},
+static PyType_Slot __pyx_type_4data_NamespaceDict_slots[] = {
+  {Py_tp_getattro, (void *)__pyx_tp_getattro_4data_NamespaceDict},
+  {Py_tp_setattro, (void *)__pyx_tp_setattro_4data_NamespaceDict},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_4data_NamespaceDict},
+  {Py_tp_clear, (void *)__pyx_tp_clear_4data_NamespaceDict},
+  {Py_tp_methods, (void *)__pyx_methods_4data_NamespaceDict},
   {0, 0},
 };
-static PyType_Spec __pyx_type_3pop_4data_NamespaceDict_spec = {
-  "pop.data.NamespaceDict",
-  sizeof(struct __pyx_obj_3pop_4data_NamespaceDict),
+static PyType_Spec __pyx_type_4data_NamespaceDict_spec = {
+  "data.NamespaceDict",
+  sizeof(struct __pyx_obj_4data_NamespaceDict),
   0,
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE,
-  __pyx_type_3pop_4data_NamespaceDict_slots,
+  __pyx_type_4data_NamespaceDict_slots,
 };
 #else
 
-static PyTypeObject __pyx_type_3pop_4data_NamespaceDict = {
+static PyTypeObject __pyx_type_4data_NamespaceDict = {
   PyVarObject_HEAD_INIT(0, 0)
-  "pop.data.""NamespaceDict", /*tp_name*/
-  sizeof(struct __pyx_obj_3pop_4data_NamespaceDict), /*tp_basicsize*/
+  "data.""NamespaceDict", /*tp_name*/
+  sizeof(struct __pyx_obj_4data_NamespaceDict), /*tp_basicsize*/
   0, /*tp_itemsize*/
   0, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
@@ -12529,26 +12524,26 @@
   0, /*tp_repr*/
   0, /*tp_as_number*/
   0, /*tp_as_sequence*/
   0, /*tp_as_mapping*/
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
-  __pyx_tp_getattro_3pop_4data_NamespaceDict, /*tp_getattro*/
-  __pyx_tp_setattro_3pop_4data_NamespaceDict, /*tp_setattro*/
+  __pyx_tp_getattro_4data_NamespaceDict, /*tp_getattro*/
+  __pyx_tp_setattro_4data_NamespaceDict, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_3pop_4data_NamespaceDict, /*tp_traverse*/
-  __pyx_tp_clear_3pop_4data_NamespaceDict, /*tp_clear*/
+  __pyx_tp_traverse_4data_NamespaceDict, /*tp_traverse*/
+  __pyx_tp_clear_4data_NamespaceDict, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_3pop_4data_NamespaceDict, /*tp_methods*/
+  __pyx_methods_4data_NamespaceDict, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   #if !CYTHON_USE_TYPE_SPECS
@@ -12583,43 +12578,43 @@
   0, /*tp_watched*/
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
-static struct __pyx_vtabstruct_3pop_4data_MultidictCache __pyx_vtable_3pop_4data_MultidictCache;
+static struct __pyx_vtabstruct_4data_MultidictCache __pyx_vtable_4data_MultidictCache;
 
-static PyObject *__pyx_tp_new_3pop_4data_MultidictCache(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
-  struct __pyx_obj_3pop_4data_MultidictCache *p;
+static PyObject *__pyx_tp_new_4data_MultidictCache(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  struct __pyx_obj_4data_MultidictCache *p;
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
   if (likely(!__Pyx_PyType_HasFeature(t, Py_TPFLAGS_IS_ABSTRACT))) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
   #endif
-  p = ((struct __pyx_obj_3pop_4data_MultidictCache *)o);
-  p->__pyx_vtab = __pyx_vtabptr_3pop_4data_MultidictCache;
+  p = ((struct __pyx_obj_4data_MultidictCache *)o);
+  p->__pyx_vtab = __pyx_vtabptr_4data_MultidictCache;
   p->_cache = ((PyObject*)Py_None); Py_INCREF(Py_None);
   p->_base_dicts = ((PyObject*)Py_None); Py_INCREF(Py_None);
   p->_split_cache = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
-static void __pyx_tp_dealloc_3pop_4data_MultidictCache(PyObject *o) {
-  struct __pyx_obj_3pop_4data_MultidictCache *p = (struct __pyx_obj_3pop_4data_MultidictCache *)o;
+static void __pyx_tp_dealloc_4data_MultidictCache(PyObject *o) {
+  struct __pyx_obj_4data_MultidictCache *p = (struct __pyx_obj_4data_MultidictCache *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
-    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_3pop_4data_MultidictCache) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_4data_MultidictCache) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->_cache);
   Py_CLEAR(p->_base_dicts);
@@ -12630,104 +12625,104 @@
   {
     freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
     if (tp_free) tp_free(o);
   }
   #endif
 }
 
-static int __pyx_tp_traverse_3pop_4data_MultidictCache(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_4data_MultidictCache(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_3pop_4data_MultidictCache *p = (struct __pyx_obj_3pop_4data_MultidictCache *)o;
+  struct __pyx_obj_4data_MultidictCache *p = (struct __pyx_obj_4data_MultidictCache *)o;
   if (p->_cache) {
     e = (*v)(p->_cache, a); if (e) return e;
   }
   if (p->_base_dicts) {
     e = (*v)(p->_base_dicts, a); if (e) return e;
   }
   if (p->_split_cache) {
     e = (*v)(p->_split_cache, a); if (e) return e;
   }
   return 0;
 }
 
-static int __pyx_tp_clear_3pop_4data_MultidictCache(PyObject *o) {
+static int __pyx_tp_clear_4data_MultidictCache(PyObject *o) {
   PyObject* tmp;
-  struct __pyx_obj_3pop_4data_MultidictCache *p = (struct __pyx_obj_3pop_4data_MultidictCache *)o;
+  struct __pyx_obj_4data_MultidictCache *p = (struct __pyx_obj_4data_MultidictCache *)o;
   tmp = ((PyObject*)p->_cache);
   p->_cache = ((PyObject*)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->_base_dicts);
   p->_base_dicts = ((PyObject*)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->_split_cache);
   p->_split_cache = ((PyObject*)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
-static PyObject *__pyx_sq_item_3pop_4data_MultidictCache(PyObject *o, Py_ssize_t i) {
+static PyObject *__pyx_sq_item_4data_MultidictCache(PyObject *o, Py_ssize_t i) {
   PyObject *r;
   PyObject *x = PyInt_FromSsize_t(i); if(!x) return 0;
   r = Py_TYPE(o)->tp_as_mapping->mp_subscript(o, x);
   Py_DECREF(x);
   return r;
 }
 
-static PyMethodDef __pyx_methods_3pop_4data_MultidictCache[] = {
-  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_14MultidictCache_11__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_14MultidictCache_13__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+static PyMethodDef __pyx_methods_4data_MultidictCache[] = {
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_14MultidictCache_11__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_14MultidictCache_13__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
 #if CYTHON_USE_TYPE_SPECS
-static PyType_Slot __pyx_type_3pop_4data_MultidictCache_slots[] = {
-  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_3pop_4data_MultidictCache},
-  {Py_sq_item, (void *)__pyx_sq_item_3pop_4data_MultidictCache},
-  {Py_sq_contains, (void *)__pyx_pw_3pop_4data_14MultidictCache_9__contains__},
-  {Py_mp_subscript, (void *)__pyx_pw_3pop_4data_14MultidictCache_5__getitem__},
-  {Py_tp_traverse, (void *)__pyx_tp_traverse_3pop_4data_MultidictCache},
-  {Py_tp_clear, (void *)__pyx_tp_clear_3pop_4data_MultidictCache},
-  {Py_tp_iter, (void *)__pyx_pw_3pop_4data_14MultidictCache_7__iter__},
-  {Py_tp_methods, (void *)__pyx_methods_3pop_4data_MultidictCache},
-  {Py_tp_init, (void *)__pyx_pw_3pop_4data_14MultidictCache_1__init__},
-  {Py_tp_new, (void *)__pyx_tp_new_3pop_4data_MultidictCache},
+static PyType_Slot __pyx_type_4data_MultidictCache_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_4data_MultidictCache},
+  {Py_sq_item, (void *)__pyx_sq_item_4data_MultidictCache},
+  {Py_sq_contains, (void *)__pyx_pw_4data_14MultidictCache_9__contains__},
+  {Py_mp_subscript, (void *)__pyx_pw_4data_14MultidictCache_5__getitem__},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_4data_MultidictCache},
+  {Py_tp_clear, (void *)__pyx_tp_clear_4data_MultidictCache},
+  {Py_tp_iter, (void *)__pyx_pw_4data_14MultidictCache_7__iter__},
+  {Py_tp_methods, (void *)__pyx_methods_4data_MultidictCache},
+  {Py_tp_init, (void *)__pyx_pw_4data_14MultidictCache_1__init__},
+  {Py_tp_new, (void *)__pyx_tp_new_4data_MultidictCache},
   {0, 0},
 };
-static PyType_Spec __pyx_type_3pop_4data_MultidictCache_spec = {
-  "pop.data.MultidictCache",
-  sizeof(struct __pyx_obj_3pop_4data_MultidictCache),
+static PyType_Spec __pyx_type_4data_MultidictCache_spec = {
+  "data.MultidictCache",
+  sizeof(struct __pyx_obj_4data_MultidictCache),
   0,
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC,
-  __pyx_type_3pop_4data_MultidictCache_slots,
+  __pyx_type_4data_MultidictCache_slots,
 };
 #else
 
 static PySequenceMethods __pyx_tp_as_sequence_MultidictCache = {
   0, /*sq_length*/
   0, /*sq_concat*/
   0, /*sq_repeat*/
-  __pyx_sq_item_3pop_4data_MultidictCache, /*sq_item*/
+  __pyx_sq_item_4data_MultidictCache, /*sq_item*/
   0, /*sq_slice*/
   0, /*sq_ass_item*/
   0, /*sq_ass_slice*/
-  __pyx_pw_3pop_4data_14MultidictCache_9__contains__, /*sq_contains*/
+  __pyx_pw_4data_14MultidictCache_9__contains__, /*sq_contains*/
   0, /*sq_inplace_concat*/
   0, /*sq_inplace_repeat*/
 };
 
 static PyMappingMethods __pyx_tp_as_mapping_MultidictCache = {
   0, /*mp_length*/
-  __pyx_pw_3pop_4data_14MultidictCache_5__getitem__, /*mp_subscript*/
+  __pyx_pw_4data_14MultidictCache_5__getitem__, /*mp_subscript*/
   0, /*mp_ass_subscript*/
 };
 
-static PyTypeObject __pyx_type_3pop_4data_MultidictCache = {
+static PyTypeObject __pyx_type_4data_MultidictCache = {
   PyVarObject_HEAD_INIT(0, 0)
-  "pop.data.""MultidictCache", /*tp_name*/
-  sizeof(struct __pyx_obj_3pop_4data_MultidictCache), /*tp_basicsize*/
+  "data.""MultidictCache", /*tp_name*/
+  sizeof(struct __pyx_obj_4data_MultidictCache), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_3pop_4data_MultidictCache, /*tp_dealloc*/
+  __pyx_tp_dealloc_4data_MultidictCache, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -12746,33 +12741,33 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_3pop_4data_MultidictCache, /*tp_traverse*/
-  __pyx_tp_clear_3pop_4data_MultidictCache, /*tp_clear*/
+  __pyx_tp_traverse_4data_MultidictCache, /*tp_traverse*/
+  __pyx_tp_clear_4data_MultidictCache, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
-  __pyx_pw_3pop_4data_14MultidictCache_7__iter__, /*tp_iter*/
+  __pyx_pw_4data_14MultidictCache_7__iter__, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_3pop_4data_MultidictCache, /*tp_methods*/
+  __pyx_methods_4data_MultidictCache, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
   #endif
-  __pyx_pw_3pop_4data_14MultidictCache_1__init__, /*tp_init*/
+  __pyx_pw_4data_14MultidictCache_1__init__, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_3pop_4data_MultidictCache, /*tp_new*/
+  __pyx_tp_new_4data_MultidictCache, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -12796,38 +12791,38 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
-static PyObject *__pyx_tp_new_3pop_4data_ImmutableNamespaceDict(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
-  struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *p;
+static PyObject *__pyx_tp_new_4data_ImmutableNamespaceDict(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  struct __pyx_obj_4data_ImmutableNamespaceDict *p;
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
   if (likely(!__Pyx_PyType_HasFeature(t, Py_TPFLAGS_IS_ABSTRACT))) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
   #endif
-  p = ((struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)o);
+  p = ((struct __pyx_obj_4data_ImmutableNamespaceDict *)o);
   p->_ImmutableNamespaceDict__data = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
-static void __pyx_tp_dealloc_3pop_4data_ImmutableNamespaceDict(PyObject *o) {
-  struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *p = (struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)o;
+static void __pyx_tp_dealloc_4data_ImmutableNamespaceDict(PyObject *o) {
+  struct __pyx_obj_4data_ImmutableNamespaceDict *p = (struct __pyx_obj_4data_ImmutableNamespaceDict *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
-    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_3pop_4data_ImmutableNamespaceDict) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_4data_ImmutableNamespaceDict) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->_ImmutableNamespaceDict__data);
   #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
@@ -12836,140 +12831,140 @@
   {
     freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
     if (tp_free) tp_free(o);
   }
   #endif
 }
 
-static int __pyx_tp_traverse_3pop_4data_ImmutableNamespaceDict(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_4data_ImmutableNamespaceDict(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *p = (struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)o;
+  struct __pyx_obj_4data_ImmutableNamespaceDict *p = (struct __pyx_obj_4data_ImmutableNamespaceDict *)o;
   if (p->_ImmutableNamespaceDict__data) {
     e = (*v)(p->_ImmutableNamespaceDict__data, a); if (e) return e;
   }
   return 0;
 }
 
-static int __pyx_tp_clear_3pop_4data_ImmutableNamespaceDict(PyObject *o) {
+static int __pyx_tp_clear_4data_ImmutableNamespaceDict(PyObject *o) {
   PyObject* tmp;
-  struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *p = (struct __pyx_obj_3pop_4data_ImmutableNamespaceDict *)o;
+  struct __pyx_obj_4data_ImmutableNamespaceDict *p = (struct __pyx_obj_4data_ImmutableNamespaceDict *)o;
   tmp = ((PyObject*)p->_ImmutableNamespaceDict__data);
   p->_ImmutableNamespaceDict__data = ((PyObject*)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
-static PyObject *__pyx_sq_item_3pop_4data_ImmutableNamespaceDict(PyObject *o, Py_ssize_t i) {
+static PyObject *__pyx_sq_item_4data_ImmutableNamespaceDict(PyObject *o, Py_ssize_t i) {
   PyObject *r;
   PyObject *x = PyInt_FromSsize_t(i); if(!x) return 0;
   r = Py_TYPE(o)->tp_as_mapping->mp_subscript(o, x);
   Py_DECREF(x);
   return r;
 }
 
-static int __pyx_mp_ass_subscript_3pop_4data_ImmutableNamespaceDict(PyObject *o, PyObject *i, PyObject *v) {
+static int __pyx_mp_ass_subscript_4data_ImmutableNamespaceDict(PyObject *o, PyObject *i, PyObject *v) {
   if (v) {
-    return __pyx_pw_3pop_4data_22ImmutableNamespaceDict_9__setitem__(o, i, v);
+    return __pyx_pw_4data_22ImmutableNamespaceDict_9__setitem__(o, i, v);
   }
   else {
     __Pyx_TypeName o_type_name;
     o_type_name = __Pyx_PyType_GetName(Py_TYPE(o));
     PyErr_Format(PyExc_NotImplementedError,
       "Subscript deletion not supported by " __Pyx_FMT_TYPENAME, o_type_name);
     __Pyx_DECREF_TypeName(o_type_name);
     return -1;
   }
 }
 
-static PyObject *__pyx_tp_getattro_3pop_4data_ImmutableNamespaceDict(PyObject *o, PyObject *n) {
+static PyObject *__pyx_tp_getattro_4data_ImmutableNamespaceDict(PyObject *o, PyObject *n) {
   PyObject *v = __Pyx_PyObject_GenericGetAttr(o, n);
   if (!v && PyErr_ExceptionMatches(PyExc_AttributeError)) {
     PyErr_Clear();
-    v = __pyx_pw_3pop_4data_22ImmutableNamespaceDict_5__getattr__(o, n);
+    v = __pyx_pw_4data_22ImmutableNamespaceDict_5__getattr__(o, n);
   }
   return v;
 }
 
-static int __pyx_tp_setattro_3pop_4data_ImmutableNamespaceDict(PyObject *o, PyObject *n, PyObject *v) {
+static int __pyx_tp_setattro_4data_ImmutableNamespaceDict(PyObject *o, PyObject *n, PyObject *v) {
   if (v) {
-    return __pyx_pw_3pop_4data_22ImmutableNamespaceDict_7__setattr__(o, n, v);
+    return __pyx_pw_4data_22ImmutableNamespaceDict_7__setattr__(o, n, v);
   }
   else {
     return PyObject_GenericSetAttr(o, n, 0);
   }
 }
 
-static PyObject *__pyx_tp_richcompare_3pop_4data_ImmutableNamespaceDict(PyObject *o1, PyObject *o2, int op) {
+static PyObject *__pyx_tp_richcompare_4data_ImmutableNamespaceDict(PyObject *o1, PyObject *o2, int op) {
   switch (op) {
     case Py_EQ: {
-      return __pyx_pw_3pop_4data_22ImmutableNamespaceDict_23__eq__(o1, o2);
+      return __pyx_pw_4data_22ImmutableNamespaceDict_23__eq__(o1, o2);
     }
     case Py_NE: {
-      return __pyx_pw_3pop_4data_22ImmutableNamespaceDict_25__ne__(o1, o2);
+      return __pyx_pw_4data_22ImmutableNamespaceDict_25__ne__(o1, o2);
     }
     default: {
       return __Pyx_NewRef(Py_NotImplemented);
     }
   }
 }
 
-static PyObject *__pyx_getprop_3pop_4data_22ImmutableNamespaceDict__ImmutableNamespaceDict__data(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_3pop_4data_22ImmutableNamespaceDict_29_ImmutableNamespaceDict__data_1__get__(o);
+static PyObject *__pyx_getprop_4data_22ImmutableNamespaceDict__ImmutableNamespaceDict__data(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_4data_22ImmutableNamespaceDict_29_ImmutableNamespaceDict__data_1__get__(o);
 }
 
-static PyObject *__pyx_specialmethod___pyx_pw_3pop_4data_22ImmutableNamespaceDict_21__repr__(PyObject *self, CYTHON_UNUSED PyObject *arg) {
-  return __pyx_pw_3pop_4data_22ImmutableNamespaceDict_21__repr__(self);
+static PyObject *__pyx_specialmethod___pyx_pw_4data_22ImmutableNamespaceDict_21__repr__(PyObject *self, CYTHON_UNUSED PyObject *arg) {
+  return __pyx_pw_4data_22ImmutableNamespaceDict_21__repr__(self);
 }
 
-static PyMethodDef __pyx_methods_3pop_4data_ImmutableNamespaceDict[] = {
-  {"__getattr__", (PyCFunction)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_5__getattr__, METH_O|METH_COEXIST, 0},
-  {"__repr__", (PyCFunction)__pyx_specialmethod___pyx_pw_3pop_4data_22ImmutableNamespaceDict_21__repr__, METH_NOARGS|METH_COEXIST, 0},
-  {"keys", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_27keys, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"values", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_29values, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"items", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_31items, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"get", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_33get, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"copy", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_35copy, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_37__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_39__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+static PyMethodDef __pyx_methods_4data_ImmutableNamespaceDict[] = {
+  {"__getattr__", (PyCFunction)__pyx_pw_4data_22ImmutableNamespaceDict_5__getattr__, METH_O|METH_COEXIST, 0},
+  {"__repr__", (PyCFunction)__pyx_specialmethod___pyx_pw_4data_22ImmutableNamespaceDict_21__repr__, METH_NOARGS|METH_COEXIST, 0},
+  {"keys", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_22ImmutableNamespaceDict_27keys, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"values", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_22ImmutableNamespaceDict_29values, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"items", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_22ImmutableNamespaceDict_31items, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"get", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_22ImmutableNamespaceDict_33get, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"copy", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_22ImmutableNamespaceDict_35copy, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_22ImmutableNamespaceDict_37__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4data_22ImmutableNamespaceDict_39__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
 
-static struct PyGetSetDef __pyx_getsets_3pop_4data_ImmutableNamespaceDict[] = {
-  {(char *)"_ImmutableNamespaceDict__data", __pyx_getprop_3pop_4data_22ImmutableNamespaceDict__ImmutableNamespaceDict__data, 0, (char *)0, 0},
+static struct PyGetSetDef __pyx_getsets_4data_ImmutableNamespaceDict[] = {
+  {(char *)"_ImmutableNamespaceDict__data", __pyx_getprop_4data_22ImmutableNamespaceDict__ImmutableNamespaceDict__data, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 #if CYTHON_USE_TYPE_SPECS
-static PyType_Slot __pyx_type_3pop_4data_ImmutableNamespaceDict_slots[] = {
-  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_3pop_4data_ImmutableNamespaceDict},
-  {Py_tp_repr, (void *)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_21__repr__},
-  {Py_nb_bool, (void *)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_17__bool__},
-  {Py_sq_length, (void *)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_13__len__},
-  {Py_sq_item, (void *)__pyx_sq_item_3pop_4data_ImmutableNamespaceDict},
-  {Py_sq_contains, (void *)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_19__contains__},
-  {Py_mp_length, (void *)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_13__len__},
-  {Py_mp_subscript, (void *)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_3__getitem__},
-  {Py_mp_ass_subscript, (void *)__pyx_mp_ass_subscript_3pop_4data_ImmutableNamespaceDict},
-  {Py_tp_call, (void *)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_11__call__},
-  {Py_tp_getattro, (void *)__pyx_tp_getattro_3pop_4data_ImmutableNamespaceDict},
-  {Py_tp_setattro, (void *)__pyx_tp_setattro_3pop_4data_ImmutableNamespaceDict},
-  {Py_tp_traverse, (void *)__pyx_tp_traverse_3pop_4data_ImmutableNamespaceDict},
-  {Py_tp_clear, (void *)__pyx_tp_clear_3pop_4data_ImmutableNamespaceDict},
-  {Py_tp_richcompare, (void *)__pyx_tp_richcompare_3pop_4data_ImmutableNamespaceDict},
-  {Py_tp_iter, (void *)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_15__iter__},
-  {Py_tp_methods, (void *)__pyx_methods_3pop_4data_ImmutableNamespaceDict},
-  {Py_tp_getset, (void *)__pyx_getsets_3pop_4data_ImmutableNamespaceDict},
-  {Py_tp_init, (void *)__pyx_pw_3pop_4data_22ImmutableNamespaceDict_1__init__},
-  {Py_tp_new, (void *)__pyx_tp_new_3pop_4data_ImmutableNamespaceDict},
+static PyType_Slot __pyx_type_4data_ImmutableNamespaceDict_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_4data_ImmutableNamespaceDict},
+  {Py_tp_repr, (void *)__pyx_pw_4data_22ImmutableNamespaceDict_21__repr__},
+  {Py_nb_bool, (void *)__pyx_pw_4data_22ImmutableNamespaceDict_17__bool__},
+  {Py_sq_length, (void *)__pyx_pw_4data_22ImmutableNamespaceDict_13__len__},
+  {Py_sq_item, (void *)__pyx_sq_item_4data_ImmutableNamespaceDict},
+  {Py_sq_contains, (void *)__pyx_pw_4data_22ImmutableNamespaceDict_19__contains__},
+  {Py_mp_length, (void *)__pyx_pw_4data_22ImmutableNamespaceDict_13__len__},
+  {Py_mp_subscript, (void *)__pyx_pw_4data_22ImmutableNamespaceDict_3__getitem__},
+  {Py_mp_ass_subscript, (void *)__pyx_mp_ass_subscript_4data_ImmutableNamespaceDict},
+  {Py_tp_call, (void *)__pyx_pw_4data_22ImmutableNamespaceDict_11__call__},
+  {Py_tp_getattro, (void *)__pyx_tp_getattro_4data_ImmutableNamespaceDict},
+  {Py_tp_setattro, (void *)__pyx_tp_setattro_4data_ImmutableNamespaceDict},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_4data_ImmutableNamespaceDict},
+  {Py_tp_clear, (void *)__pyx_tp_clear_4data_ImmutableNamespaceDict},
+  {Py_tp_richcompare, (void *)__pyx_tp_richcompare_4data_ImmutableNamespaceDict},
+  {Py_tp_iter, (void *)__pyx_pw_4data_22ImmutableNamespaceDict_15__iter__},
+  {Py_tp_methods, (void *)__pyx_methods_4data_ImmutableNamespaceDict},
+  {Py_tp_getset, (void *)__pyx_getsets_4data_ImmutableNamespaceDict},
+  {Py_tp_init, (void *)__pyx_pw_4data_22ImmutableNamespaceDict_1__init__},
+  {Py_tp_new, (void *)__pyx_tp_new_4data_ImmutableNamespaceDict},
   {0, 0},
 };
-static PyType_Spec __pyx_type_3pop_4data_ImmutableNamespaceDict_spec = {
-  "pop.data.ImmutableNamespaceDict",
-  sizeof(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict),
+static PyType_Spec __pyx_type_4data_ImmutableNamespaceDict_spec = {
+  "data.ImmutableNamespaceDict",
+  sizeof(struct __pyx_obj_4data_ImmutableNamespaceDict),
   0,
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC,
-  __pyx_type_3pop_4data_ImmutableNamespaceDict_slots,
+  __pyx_type_4data_ImmutableNamespaceDict_slots,
 };
 #else
 
 static PyNumberMethods __pyx_tp_as_number_ImmutableNamespaceDict = {
   0, /*nb_add*/
   0, /*nb_subtract*/
   0, /*nb_multiply*/
@@ -12978,15 +12973,15 @@
   #endif
   0, /*nb_remainder*/
   0, /*nb_divmod*/
   0, /*nb_power*/
   0, /*nb_negative*/
   0, /*nb_positive*/
   0, /*nb_absolute*/
-  __pyx_pw_3pop_4data_22ImmutableNamespaceDict_17__bool__, /*nb_bool*/
+  __pyx_pw_4data_22ImmutableNamespaceDict_17__bool__, /*nb_bool*/
   0, /*nb_invert*/
   0, /*nb_lshift*/
   0, /*nb_rshift*/
   0, /*nb_and*/
   0, /*nb_xor*/
   0, /*nb_or*/
   #if PY_MAJOR_VERSION < 3 || (CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x03050000)
@@ -13028,83 +13023,83 @@
   #endif
   #if PY_VERSION_HEX >= 0x03050000
   0, /*nb_inplace_matrix_multiply*/
   #endif
 };
 
 static PySequenceMethods __pyx_tp_as_sequence_ImmutableNamespaceDict = {
-  __pyx_pw_3pop_4data_22ImmutableNamespaceDict_13__len__, /*sq_length*/
+  __pyx_pw_4data_22ImmutableNamespaceDict_13__len__, /*sq_length*/
   0, /*sq_concat*/
   0, /*sq_repeat*/
-  __pyx_sq_item_3pop_4data_ImmutableNamespaceDict, /*sq_item*/
+  __pyx_sq_item_4data_ImmutableNamespaceDict, /*sq_item*/
   0, /*sq_slice*/
   0, /*sq_ass_item*/
   0, /*sq_ass_slice*/
-  __pyx_pw_3pop_4data_22ImmutableNamespaceDict_19__contains__, /*sq_contains*/
+  __pyx_pw_4data_22ImmutableNamespaceDict_19__contains__, /*sq_contains*/
   0, /*sq_inplace_concat*/
   0, /*sq_inplace_repeat*/
 };
 
 static PyMappingMethods __pyx_tp_as_mapping_ImmutableNamespaceDict = {
-  __pyx_pw_3pop_4data_22ImmutableNamespaceDict_13__len__, /*mp_length*/
-  __pyx_pw_3pop_4data_22ImmutableNamespaceDict_3__getitem__, /*mp_subscript*/
-  __pyx_mp_ass_subscript_3pop_4data_ImmutableNamespaceDict, /*mp_ass_subscript*/
+  __pyx_pw_4data_22ImmutableNamespaceDict_13__len__, /*mp_length*/
+  __pyx_pw_4data_22ImmutableNamespaceDict_3__getitem__, /*mp_subscript*/
+  __pyx_mp_ass_subscript_4data_ImmutableNamespaceDict, /*mp_ass_subscript*/
 };
 
-static PyTypeObject __pyx_type_3pop_4data_ImmutableNamespaceDict = {
+static PyTypeObject __pyx_type_4data_ImmutableNamespaceDict = {
   PyVarObject_HEAD_INIT(0, 0)
-  "pop.data.""ImmutableNamespaceDict", /*tp_name*/
-  sizeof(struct __pyx_obj_3pop_4data_ImmutableNamespaceDict), /*tp_basicsize*/
+  "data.""ImmutableNamespaceDict", /*tp_name*/
+  sizeof(struct __pyx_obj_4data_ImmutableNamespaceDict), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_3pop_4data_ImmutableNamespaceDict, /*tp_dealloc*/
+  __pyx_tp_dealloc_4data_ImmutableNamespaceDict, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
   #endif
-  __pyx_pw_3pop_4data_22ImmutableNamespaceDict_21__repr__, /*tp_repr*/
+  __pyx_pw_4data_22ImmutableNamespaceDict_21__repr__, /*tp_repr*/
   &__pyx_tp_as_number_ImmutableNamespaceDict, /*tp_as_number*/
   &__pyx_tp_as_sequence_ImmutableNamespaceDict, /*tp_as_sequence*/
   &__pyx_tp_as_mapping_ImmutableNamespaceDict, /*tp_as_mapping*/
   0, /*tp_hash*/
-  __pyx_pw_3pop_4data_22ImmutableNamespaceDict_11__call__, /*tp_call*/
+  __pyx_pw_4data_22ImmutableNamespaceDict_11__call__, /*tp_call*/
   0, /*tp_str*/
-  __pyx_tp_getattro_3pop_4data_ImmutableNamespaceDict, /*tp_getattro*/
-  __pyx_tp_setattro_3pop_4data_ImmutableNamespaceDict, /*tp_setattro*/
+  __pyx_tp_getattro_4data_ImmutableNamespaceDict, /*tp_getattro*/
+  __pyx_tp_setattro_4data_ImmutableNamespaceDict, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_3pop_4data_ImmutableNamespaceDict, /*tp_traverse*/
-  __pyx_tp_clear_3pop_4data_ImmutableNamespaceDict, /*tp_clear*/
-  __pyx_tp_richcompare_3pop_4data_ImmutableNamespaceDict, /*tp_richcompare*/
+  __pyx_tp_traverse_4data_ImmutableNamespaceDict, /*tp_traverse*/
+  __pyx_tp_clear_4data_ImmutableNamespaceDict, /*tp_clear*/
+  __pyx_tp_richcompare_4data_ImmutableNamespaceDict, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
-  __pyx_pw_3pop_4data_22ImmutableNamespaceDict_15__iter__, /*tp_iter*/
+  __pyx_pw_4data_22ImmutableNamespaceDict_15__iter__, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_3pop_4data_ImmutableNamespaceDict, /*tp_methods*/
+  __pyx_methods_4data_ImmutableNamespaceDict, /*tp_methods*/
   0, /*tp_members*/
-  __pyx_getsets_3pop_4data_ImmutableNamespaceDict, /*tp_getset*/
+  __pyx_getsets_4data_ImmutableNamespaceDict, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
   #endif
-  __pyx_pw_3pop_4data_22ImmutableNamespaceDict_1__init__, /*tp_init*/
+  __pyx_pw_4data_22ImmutableNamespaceDict_1__init__, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_3pop_4data_ImmutableNamespaceDict, /*tp_new*/
+  __pyx_tp_new_4data_ImmutableNamespaceDict, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -13129,108 +13124,108 @@
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
 #if CYTHON_USE_FREELISTS
-static struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__ *__pyx_freelist_3pop_4data___pyx_scope_struct____contains__[8];
-static int __pyx_freecount_3pop_4data___pyx_scope_struct____contains__ = 0;
+static struct __pyx_obj_4data___pyx_scope_struct____contains__ *__pyx_freelist_4data___pyx_scope_struct____contains__[8];
+static int __pyx_freecount_4data___pyx_scope_struct____contains__ = 0;
 #endif
 
-static PyObject *__pyx_tp_new_3pop_4data___pyx_scope_struct____contains__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+static PyObject *__pyx_tp_new_4data___pyx_scope_struct____contains__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
   #if CYTHON_USE_FREELISTS
-  if (likely((int)(__pyx_freecount_3pop_4data___pyx_scope_struct____contains__ > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__)))) {
-    o = (PyObject*)__pyx_freelist_3pop_4data___pyx_scope_struct____contains__[--__pyx_freecount_3pop_4data___pyx_scope_struct____contains__];
-    memset(o, 0, sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__));
+  if (likely((int)(__pyx_freecount_4data___pyx_scope_struct____contains__ > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_4data___pyx_scope_struct____contains__)))) {
+    o = (PyObject*)__pyx_freelist_4data___pyx_scope_struct____contains__[--__pyx_freecount_4data___pyx_scope_struct____contains__];
+    memset(o, 0, sizeof(struct __pyx_obj_4data___pyx_scope_struct____contains__));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
   {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
   #endif
   return o;
 }
 
-static void __pyx_tp_dealloc_3pop_4data___pyx_scope_struct____contains__(PyObject *o) {
-  struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__ *p = (struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__ *)o;
+static void __pyx_tp_dealloc_4data___pyx_scope_struct____contains__(PyObject *o) {
+  struct __pyx_obj_4data___pyx_scope_struct____contains__ *p = (struct __pyx_obj_4data___pyx_scope_struct____contains__ *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
-    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_3pop_4data___pyx_scope_struct____contains__) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_4data___pyx_scope_struct____contains__) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_item);
   #if CYTHON_USE_FREELISTS
-  if (((int)(__pyx_freecount_3pop_4data___pyx_scope_struct____contains__ < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__)))) {
-    __pyx_freelist_3pop_4data___pyx_scope_struct____contains__[__pyx_freecount_3pop_4data___pyx_scope_struct____contains__++] = ((struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__ *)o);
+  if (((int)(__pyx_freecount_4data___pyx_scope_struct____contains__ < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_4data___pyx_scope_struct____contains__)))) {
+    __pyx_freelist_4data___pyx_scope_struct____contains__[__pyx_freecount_4data___pyx_scope_struct____contains__++] = ((struct __pyx_obj_4data___pyx_scope_struct____contains__ *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
     #else
     {
       freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
       if (tp_free) tp_free(o);
     }
     #endif
   }
 }
 
-static int __pyx_tp_traverse_3pop_4data___pyx_scope_struct____contains__(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_4data___pyx_scope_struct____contains__(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__ *p = (struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__ *)o;
+  struct __pyx_obj_4data___pyx_scope_struct____contains__ *p = (struct __pyx_obj_4data___pyx_scope_struct____contains__ *)o;
   if (p->__pyx_v_item) {
     e = (*v)(p->__pyx_v_item, a); if (e) return e;
   }
   return 0;
 }
 
-static int __pyx_tp_clear_3pop_4data___pyx_scope_struct____contains__(PyObject *o) {
+static int __pyx_tp_clear_4data___pyx_scope_struct____contains__(PyObject *o) {
   PyObject* tmp;
-  struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__ *p = (struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__ *)o;
+  struct __pyx_obj_4data___pyx_scope_struct____contains__ *p = (struct __pyx_obj_4data___pyx_scope_struct____contains__ *)o;
   tmp = ((PyObject*)p->__pyx_v_item);
   p->__pyx_v_item = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 #if CYTHON_USE_TYPE_SPECS
-static PyType_Slot __pyx_type_3pop_4data___pyx_scope_struct____contains___slots[] = {
-  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_3pop_4data___pyx_scope_struct____contains__},
-  {Py_tp_traverse, (void *)__pyx_tp_traverse_3pop_4data___pyx_scope_struct____contains__},
-  {Py_tp_clear, (void *)__pyx_tp_clear_3pop_4data___pyx_scope_struct____contains__},
-  {Py_tp_new, (void *)__pyx_tp_new_3pop_4data___pyx_scope_struct____contains__},
+static PyType_Slot __pyx_type_4data___pyx_scope_struct____contains___slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_4data___pyx_scope_struct____contains__},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_4data___pyx_scope_struct____contains__},
+  {Py_tp_clear, (void *)__pyx_tp_clear_4data___pyx_scope_struct____contains__},
+  {Py_tp_new, (void *)__pyx_tp_new_4data___pyx_scope_struct____contains__},
   {0, 0},
 };
-static PyType_Spec __pyx_type_3pop_4data___pyx_scope_struct____contains___spec = {
-  "pop.data.__pyx_scope_struct____contains__",
-  sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__),
+static PyType_Spec __pyx_type_4data___pyx_scope_struct____contains___spec = {
+  "data.__pyx_scope_struct____contains__",
+  sizeof(struct __pyx_obj_4data___pyx_scope_struct____contains__),
   0,
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE,
-  __pyx_type_3pop_4data___pyx_scope_struct____contains___slots,
+  __pyx_type_4data___pyx_scope_struct____contains___slots,
 };
 #else
 
-static PyTypeObject __pyx_type_3pop_4data___pyx_scope_struct____contains__ = {
+static PyTypeObject __pyx_type_4data___pyx_scope_struct____contains__ = {
   PyVarObject_HEAD_INIT(0, 0)
-  "pop.data.""__pyx_scope_struct____contains__", /*tp_name*/
-  sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct____contains__), /*tp_basicsize*/
+  "data.""__pyx_scope_struct____contains__", /*tp_name*/
+  sizeof(struct __pyx_obj_4data___pyx_scope_struct____contains__), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_3pop_4data___pyx_scope_struct____contains__, /*tp_dealloc*/
+  __pyx_tp_dealloc_4data___pyx_scope_struct____contains__, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -13249,16 +13244,16 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_3pop_4data___pyx_scope_struct____contains__, /*tp_traverse*/
-  __pyx_tp_clear_3pop_4data___pyx_scope_struct____contains__, /*tp_clear*/
+  __pyx_tp_traverse_4data___pyx_scope_struct____contains__, /*tp_traverse*/
+  __pyx_tp_clear_4data___pyx_scope_struct____contains__, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
@@ -13267,15 +13262,15 @@
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
   #endif
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_3pop_4data___pyx_scope_struct____contains__, /*tp_new*/
+  __pyx_tp_new_4data___pyx_scope_struct____contains__, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -13300,106 +13295,106 @@
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
 #if CYTHON_USE_FREELISTS
-static struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr *__pyx_freelist_3pop_4data___pyx_scope_struct_1_genexpr[8];
-static int __pyx_freecount_3pop_4data___pyx_scope_struct_1_genexpr = 0;
+static struct __pyx_obj_4data___pyx_scope_struct_1_genexpr *__pyx_freelist_4data___pyx_scope_struct_1_genexpr[8];
+static int __pyx_freecount_4data___pyx_scope_struct_1_genexpr = 0;
 #endif
 
-static PyObject *__pyx_tp_new_3pop_4data___pyx_scope_struct_1_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+static PyObject *__pyx_tp_new_4data___pyx_scope_struct_1_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
   #if CYTHON_USE_FREELISTS
-  if (likely((int)(__pyx_freecount_3pop_4data___pyx_scope_struct_1_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr)))) {
-    o = (PyObject*)__pyx_freelist_3pop_4data___pyx_scope_struct_1_genexpr[--__pyx_freecount_3pop_4data___pyx_scope_struct_1_genexpr];
-    memset(o, 0, sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr));
+  if (likely((int)(__pyx_freecount_4data___pyx_scope_struct_1_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_4data___pyx_scope_struct_1_genexpr)))) {
+    o = (PyObject*)__pyx_freelist_4data___pyx_scope_struct_1_genexpr[--__pyx_freecount_4data___pyx_scope_struct_1_genexpr];
+    memset(o, 0, sizeof(struct __pyx_obj_4data___pyx_scope_struct_1_genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
   {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
   #endif
   return o;
 }
 
-static void __pyx_tp_dealloc_3pop_4data___pyx_scope_struct_1_genexpr(PyObject *o) {
-  struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr *p = (struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr *)o;
+static void __pyx_tp_dealloc_4data___pyx_scope_struct_1_genexpr(PyObject *o) {
+  struct __pyx_obj_4data___pyx_scope_struct_1_genexpr *p = (struct __pyx_obj_4data___pyx_scope_struct_1_genexpr *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
-    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_3pop_4data___pyx_scope_struct_1_genexpr) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_4data___pyx_scope_struct_1_genexpr) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_outer_scope);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_base_dict);
   #if CYTHON_USE_FREELISTS
-  if (((int)(__pyx_freecount_3pop_4data___pyx_scope_struct_1_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr)))) {
-    __pyx_freelist_3pop_4data___pyx_scope_struct_1_genexpr[__pyx_freecount_3pop_4data___pyx_scope_struct_1_genexpr++] = ((struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr *)o);
+  if (((int)(__pyx_freecount_4data___pyx_scope_struct_1_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_4data___pyx_scope_struct_1_genexpr)))) {
+    __pyx_freelist_4data___pyx_scope_struct_1_genexpr[__pyx_freecount_4data___pyx_scope_struct_1_genexpr++] = ((struct __pyx_obj_4data___pyx_scope_struct_1_genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
     #else
     {
       freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
       if (tp_free) tp_free(o);
     }
     #endif
   }
 }
 
-static int __pyx_tp_traverse_3pop_4data___pyx_scope_struct_1_genexpr(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_4data___pyx_scope_struct_1_genexpr(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr *p = (struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr *)o;
+  struct __pyx_obj_4data___pyx_scope_struct_1_genexpr *p = (struct __pyx_obj_4data___pyx_scope_struct_1_genexpr *)o;
   if (p->__pyx_outer_scope) {
     e = (*v)(((PyObject *)p->__pyx_outer_scope), a); if (e) return e;
   }
   if (p->__pyx_genexpr_arg_0) {
     e = (*v)(p->__pyx_genexpr_arg_0, a); if (e) return e;
   }
   if (p->__pyx_v_base_dict) {
     e = (*v)(p->__pyx_v_base_dict, a); if (e) return e;
   }
   return 0;
 }
 #if CYTHON_USE_TYPE_SPECS
-static PyType_Slot __pyx_type_3pop_4data___pyx_scope_struct_1_genexpr_slots[] = {
-  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_3pop_4data___pyx_scope_struct_1_genexpr},
-  {Py_tp_traverse, (void *)__pyx_tp_traverse_3pop_4data___pyx_scope_struct_1_genexpr},
-  {Py_tp_new, (void *)__pyx_tp_new_3pop_4data___pyx_scope_struct_1_genexpr},
+static PyType_Slot __pyx_type_4data___pyx_scope_struct_1_genexpr_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_4data___pyx_scope_struct_1_genexpr},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_4data___pyx_scope_struct_1_genexpr},
+  {Py_tp_new, (void *)__pyx_tp_new_4data___pyx_scope_struct_1_genexpr},
   {0, 0},
 };
-static PyType_Spec __pyx_type_3pop_4data___pyx_scope_struct_1_genexpr_spec = {
-  "pop.data.__pyx_scope_struct_1_genexpr",
-  sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr),
+static PyType_Spec __pyx_type_4data___pyx_scope_struct_1_genexpr_spec = {
+  "data.__pyx_scope_struct_1_genexpr",
+  sizeof(struct __pyx_obj_4data___pyx_scope_struct_1_genexpr),
   0,
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE,
-  __pyx_type_3pop_4data___pyx_scope_struct_1_genexpr_slots,
+  __pyx_type_4data___pyx_scope_struct_1_genexpr_slots,
 };
 #else
 
-static PyTypeObject __pyx_type_3pop_4data___pyx_scope_struct_1_genexpr = {
+static PyTypeObject __pyx_type_4data___pyx_scope_struct_1_genexpr = {
   PyVarObject_HEAD_INIT(0, 0)
-  "pop.data.""__pyx_scope_struct_1_genexpr", /*tp_name*/
-  sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct_1_genexpr), /*tp_basicsize*/
+  "data.""__pyx_scope_struct_1_genexpr", /*tp_name*/
+  sizeof(struct __pyx_obj_4data___pyx_scope_struct_1_genexpr), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_3pop_4data___pyx_scope_struct_1_genexpr, /*tp_dealloc*/
+  __pyx_tp_dealloc_4data___pyx_scope_struct_1_genexpr, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -13418,15 +13413,15 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_3pop_4data___pyx_scope_struct_1_genexpr, /*tp_traverse*/
+  __pyx_tp_traverse_4data___pyx_scope_struct_1_genexpr, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
@@ -13436,15 +13431,15 @@
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
   #endif
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_3pop_4data___pyx_scope_struct_1_genexpr, /*tp_new*/
+  __pyx_tp_new_4data___pyx_scope_struct_1_genexpr, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -13469,106 +13464,106 @@
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
 #if CYTHON_USE_FREELISTS
-static struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr *__pyx_freelist_3pop_4data___pyx_scope_struct_2_genexpr[8];
-static int __pyx_freecount_3pop_4data___pyx_scope_struct_2_genexpr = 0;
+static struct __pyx_obj_4data___pyx_scope_struct_2_genexpr *__pyx_freelist_4data___pyx_scope_struct_2_genexpr[8];
+static int __pyx_freecount_4data___pyx_scope_struct_2_genexpr = 0;
 #endif
 
-static PyObject *__pyx_tp_new_3pop_4data___pyx_scope_struct_2_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+static PyObject *__pyx_tp_new_4data___pyx_scope_struct_2_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
   #if CYTHON_USE_FREELISTS
-  if (likely((int)(__pyx_freecount_3pop_4data___pyx_scope_struct_2_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr)))) {
-    o = (PyObject*)__pyx_freelist_3pop_4data___pyx_scope_struct_2_genexpr[--__pyx_freecount_3pop_4data___pyx_scope_struct_2_genexpr];
-    memset(o, 0, sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr));
+  if (likely((int)(__pyx_freecount_4data___pyx_scope_struct_2_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_4data___pyx_scope_struct_2_genexpr)))) {
+    o = (PyObject*)__pyx_freelist_4data___pyx_scope_struct_2_genexpr[--__pyx_freecount_4data___pyx_scope_struct_2_genexpr];
+    memset(o, 0, sizeof(struct __pyx_obj_4data___pyx_scope_struct_2_genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
   {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
   #endif
   return o;
 }
 
-static void __pyx_tp_dealloc_3pop_4data___pyx_scope_struct_2_genexpr(PyObject *o) {
-  struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr *p = (struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr *)o;
+static void __pyx_tp_dealloc_4data___pyx_scope_struct_2_genexpr(PyObject *o) {
+  struct __pyx_obj_4data___pyx_scope_struct_2_genexpr *p = (struct __pyx_obj_4data___pyx_scope_struct_2_genexpr *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
-    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_3pop_4data___pyx_scope_struct_2_genexpr) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_4data___pyx_scope_struct_2_genexpr) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_value);
   Py_CLEAR(p->__pyx_t_0);
   #if CYTHON_USE_FREELISTS
-  if (((int)(__pyx_freecount_3pop_4data___pyx_scope_struct_2_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr)))) {
-    __pyx_freelist_3pop_4data___pyx_scope_struct_2_genexpr[__pyx_freecount_3pop_4data___pyx_scope_struct_2_genexpr++] = ((struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr *)o);
+  if (((int)(__pyx_freecount_4data___pyx_scope_struct_2_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_4data___pyx_scope_struct_2_genexpr)))) {
+    __pyx_freelist_4data___pyx_scope_struct_2_genexpr[__pyx_freecount_4data___pyx_scope_struct_2_genexpr++] = ((struct __pyx_obj_4data___pyx_scope_struct_2_genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
     #else
     {
       freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
       if (tp_free) tp_free(o);
     }
     #endif
   }
 }
 
-static int __pyx_tp_traverse_3pop_4data___pyx_scope_struct_2_genexpr(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_4data___pyx_scope_struct_2_genexpr(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr *p = (struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr *)o;
+  struct __pyx_obj_4data___pyx_scope_struct_2_genexpr *p = (struct __pyx_obj_4data___pyx_scope_struct_2_genexpr *)o;
   if (p->__pyx_genexpr_arg_0) {
     e = (*v)(p->__pyx_genexpr_arg_0, a); if (e) return e;
   }
   if (p->__pyx_v_value) {
     e = (*v)(p->__pyx_v_value, a); if (e) return e;
   }
   if (p->__pyx_t_0) {
     e = (*v)(p->__pyx_t_0, a); if (e) return e;
   }
   return 0;
 }
 #if CYTHON_USE_TYPE_SPECS
-static PyType_Slot __pyx_type_3pop_4data___pyx_scope_struct_2_genexpr_slots[] = {
-  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_3pop_4data___pyx_scope_struct_2_genexpr},
-  {Py_tp_traverse, (void *)__pyx_tp_traverse_3pop_4data___pyx_scope_struct_2_genexpr},
-  {Py_tp_new, (void *)__pyx_tp_new_3pop_4data___pyx_scope_struct_2_genexpr},
+static PyType_Slot __pyx_type_4data___pyx_scope_struct_2_genexpr_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_4data___pyx_scope_struct_2_genexpr},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_4data___pyx_scope_struct_2_genexpr},
+  {Py_tp_new, (void *)__pyx_tp_new_4data___pyx_scope_struct_2_genexpr},
   {0, 0},
 };
-static PyType_Spec __pyx_type_3pop_4data___pyx_scope_struct_2_genexpr_spec = {
-  "pop.data.__pyx_scope_struct_2_genexpr",
-  sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr),
+static PyType_Spec __pyx_type_4data___pyx_scope_struct_2_genexpr_spec = {
+  "data.__pyx_scope_struct_2_genexpr",
+  sizeof(struct __pyx_obj_4data___pyx_scope_struct_2_genexpr),
   0,
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE,
-  __pyx_type_3pop_4data___pyx_scope_struct_2_genexpr_slots,
+  __pyx_type_4data___pyx_scope_struct_2_genexpr_slots,
 };
 #else
 
-static PyTypeObject __pyx_type_3pop_4data___pyx_scope_struct_2_genexpr = {
+static PyTypeObject __pyx_type_4data___pyx_scope_struct_2_genexpr = {
   PyVarObject_HEAD_INIT(0, 0)
-  "pop.data.""__pyx_scope_struct_2_genexpr", /*tp_name*/
-  sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct_2_genexpr), /*tp_basicsize*/
+  "data.""__pyx_scope_struct_2_genexpr", /*tp_name*/
+  sizeof(struct __pyx_obj_4data___pyx_scope_struct_2_genexpr), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_3pop_4data___pyx_scope_struct_2_genexpr, /*tp_dealloc*/
+  __pyx_tp_dealloc_4data___pyx_scope_struct_2_genexpr, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -13587,15 +13582,15 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_3pop_4data___pyx_scope_struct_2_genexpr, /*tp_traverse*/
+  __pyx_tp_traverse_4data___pyx_scope_struct_2_genexpr, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
@@ -13605,15 +13600,15 @@
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
   #endif
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_3pop_4data___pyx_scope_struct_2_genexpr, /*tp_new*/
+  __pyx_tp_new_4data___pyx_scope_struct_2_genexpr, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -13638,106 +13633,106 @@
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
 #if CYTHON_USE_FREELISTS
-static struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr *__pyx_freelist_3pop_4data___pyx_scope_struct_3_genexpr[8];
-static int __pyx_freecount_3pop_4data___pyx_scope_struct_3_genexpr = 0;
+static struct __pyx_obj_4data___pyx_scope_struct_3_genexpr *__pyx_freelist_4data___pyx_scope_struct_3_genexpr[8];
+static int __pyx_freecount_4data___pyx_scope_struct_3_genexpr = 0;
 #endif
 
-static PyObject *__pyx_tp_new_3pop_4data___pyx_scope_struct_3_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+static PyObject *__pyx_tp_new_4data___pyx_scope_struct_3_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
   #if CYTHON_USE_FREELISTS
-  if (likely((int)(__pyx_freecount_3pop_4data___pyx_scope_struct_3_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr)))) {
-    o = (PyObject*)__pyx_freelist_3pop_4data___pyx_scope_struct_3_genexpr[--__pyx_freecount_3pop_4data___pyx_scope_struct_3_genexpr];
-    memset(o, 0, sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr));
+  if (likely((int)(__pyx_freecount_4data___pyx_scope_struct_3_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_4data___pyx_scope_struct_3_genexpr)))) {
+    o = (PyObject*)__pyx_freelist_4data___pyx_scope_struct_3_genexpr[--__pyx_freecount_4data___pyx_scope_struct_3_genexpr];
+    memset(o, 0, sizeof(struct __pyx_obj_4data___pyx_scope_struct_3_genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
   {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
   #endif
   return o;
 }
 
-static void __pyx_tp_dealloc_3pop_4data___pyx_scope_struct_3_genexpr(PyObject *o) {
-  struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr *p = (struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr *)o;
+static void __pyx_tp_dealloc_4data___pyx_scope_struct_3_genexpr(PyObject *o) {
+  struct __pyx_obj_4data___pyx_scope_struct_3_genexpr *p = (struct __pyx_obj_4data___pyx_scope_struct_3_genexpr *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
-    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_3pop_4data___pyx_scope_struct_3_genexpr) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_4data___pyx_scope_struct_3_genexpr) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_value);
   Py_CLEAR(p->__pyx_t_0);
   #if CYTHON_USE_FREELISTS
-  if (((int)(__pyx_freecount_3pop_4data___pyx_scope_struct_3_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr)))) {
-    __pyx_freelist_3pop_4data___pyx_scope_struct_3_genexpr[__pyx_freecount_3pop_4data___pyx_scope_struct_3_genexpr++] = ((struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr *)o);
+  if (((int)(__pyx_freecount_4data___pyx_scope_struct_3_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_4data___pyx_scope_struct_3_genexpr)))) {
+    __pyx_freelist_4data___pyx_scope_struct_3_genexpr[__pyx_freecount_4data___pyx_scope_struct_3_genexpr++] = ((struct __pyx_obj_4data___pyx_scope_struct_3_genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
     #else
     {
       freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
       if (tp_free) tp_free(o);
     }
     #endif
   }
 }
 
-static int __pyx_tp_traverse_3pop_4data___pyx_scope_struct_3_genexpr(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_4data___pyx_scope_struct_3_genexpr(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr *p = (struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr *)o;
+  struct __pyx_obj_4data___pyx_scope_struct_3_genexpr *p = (struct __pyx_obj_4data___pyx_scope_struct_3_genexpr *)o;
   if (p->__pyx_genexpr_arg_0) {
     e = (*v)(p->__pyx_genexpr_arg_0, a); if (e) return e;
   }
   if (p->__pyx_v_value) {
     e = (*v)(p->__pyx_v_value, a); if (e) return e;
   }
   if (p->__pyx_t_0) {
     e = (*v)(p->__pyx_t_0, a); if (e) return e;
   }
   return 0;
 }
 #if CYTHON_USE_TYPE_SPECS
-static PyType_Slot __pyx_type_3pop_4data___pyx_scope_struct_3_genexpr_slots[] = {
-  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_3pop_4data___pyx_scope_struct_3_genexpr},
-  {Py_tp_traverse, (void *)__pyx_tp_traverse_3pop_4data___pyx_scope_struct_3_genexpr},
-  {Py_tp_new, (void *)__pyx_tp_new_3pop_4data___pyx_scope_struct_3_genexpr},
+static PyType_Slot __pyx_type_4data___pyx_scope_struct_3_genexpr_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_4data___pyx_scope_struct_3_genexpr},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_4data___pyx_scope_struct_3_genexpr},
+  {Py_tp_new, (void *)__pyx_tp_new_4data___pyx_scope_struct_3_genexpr},
   {0, 0},
 };
-static PyType_Spec __pyx_type_3pop_4data___pyx_scope_struct_3_genexpr_spec = {
-  "pop.data.__pyx_scope_struct_3_genexpr",
-  sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr),
+static PyType_Spec __pyx_type_4data___pyx_scope_struct_3_genexpr_spec = {
+  "data.__pyx_scope_struct_3_genexpr",
+  sizeof(struct __pyx_obj_4data___pyx_scope_struct_3_genexpr),
   0,
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE,
-  __pyx_type_3pop_4data___pyx_scope_struct_3_genexpr_slots,
+  __pyx_type_4data___pyx_scope_struct_3_genexpr_slots,
 };
 #else
 
-static PyTypeObject __pyx_type_3pop_4data___pyx_scope_struct_3_genexpr = {
+static PyTypeObject __pyx_type_4data___pyx_scope_struct_3_genexpr = {
   PyVarObject_HEAD_INIT(0, 0)
-  "pop.data.""__pyx_scope_struct_3_genexpr", /*tp_name*/
-  sizeof(struct __pyx_obj_3pop_4data___pyx_scope_struct_3_genexpr), /*tp_basicsize*/
+  "data.""__pyx_scope_struct_3_genexpr", /*tp_name*/
+  sizeof(struct __pyx_obj_4data___pyx_scope_struct_3_genexpr), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_3pop_4data___pyx_scope_struct_3_genexpr, /*tp_dealloc*/
+  __pyx_tp_dealloc_4data___pyx_scope_struct_3_genexpr, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -13756,15 +13751,15 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_3pop_4data___pyx_scope_struct_3_genexpr, /*tp_traverse*/
+  __pyx_tp_traverse_4data___pyx_scope_struct_3_genexpr, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
@@ -13774,15 +13769,15 @@
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
   #endif
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_3pop_4data___pyx_scope_struct_3_genexpr, /*tp_new*/
+  __pyx_tp_new_4data___pyx_scope_struct_3_genexpr, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -13894,16 +13889,15 @@
     {&__pyx_n_s_merge_lists, __pyx_k_merge_lists, sizeof(__pyx_k_merge_lists), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
     {&__pyx_kp_u_not_found_in_any_base_dictionar, __pyx_k_not_found_in_any_base_dictionar, sizeof(__pyx_k_not_found_in_any_base_dictionar), 0, 1, 0, 0},
     {&__pyx_n_s_object, __pyx_k_object, sizeof(__pyx_k_object), 0, 0, 1, 1},
     {&__pyx_kp_u_object_has_no_attribute, __pyx_k_object_has_no_attribute, sizeof(__pyx_k_object_has_no_attribute), 0, 1, 0, 0},
     {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
-    {&__pyx_n_s_pop_data, __pyx_k_pop_data, sizeof(__pyx_k_pop_data), 0, 0, 1, 1},
-    {&__pyx_kp_s_pop_pop_data_pyx, __pyx_k_pop_pop_data_pyx, sizeof(__pyx_k_pop_pop_data_pyx), 0, 0, 1, 0},
+    {&__pyx_kp_s_pop_data_pyx, __pyx_k_pop_data_pyx, sizeof(__pyx_k_pop_data_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_unpickle_ImmutableNamespac, __pyx_k_pyx_unpickle_ImmutableNamespac, sizeof(__pyx_k_pyx_unpickle_ImmutableNamespac), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_unpickle_MultidictCache, __pyx_k_pyx_unpickle_MultidictCache, sizeof(__pyx_k_pyx_unpickle_MultidictCache), 0, 0, 1, 1},
@@ -13944,37 +13938,37 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "pop/pop.data.pyx":94
+  /* "data.pyx":94
  *             object.__setattr__(self, key, value)
  *         else:
  *             raise TypeError("ImmutableNamespaceDict does not support attribute assignment")             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(self, key, value):
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_ImmutableNamespaceDict_does_not); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "pop/pop.data.pyx":97
+  /* "data.pyx":97
  * 
  *     def __setitem__(self, key, value):
  *         raise TypeError("ImmutableNamespaceDict does not support item assignment")             # <<<<<<<<<<<<<<
  * 
  *     def __call__(self):
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_ImmutableNamespaceDict_does_not_2); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "pop/pop.data.pyx":192
+  /* "data.pyx":192
  *                 dest[key] = ret
  *             elif isinstance(dest_subkey, list) and isinstance(val, list) and merge_lists:
  *                 merged = dest_subkey[:]             # <<<<<<<<<<<<<<
  *                 merged.extend([x for x in val if x not in merged])
  *                 dest[key] = merged
  */
   __pyx_slice__6 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__6)) __PYX_ERR(0, 192, __pyx_L1_error)
@@ -14015,25 +14009,25 @@
  *     __pyx_unpickle_NamespaceDict__set_state(self, __pyx_state)
  */
   __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
   __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(2, 16, __pyx_L1_error)
 
-  /* "pop/pop.data.pyx":38
+  /* "data.pyx":38
  *         self._split_cache = dict[str, list[str]]()
  * 
  *     cpdef _clear(self):             # <<<<<<<<<<<<<<
  *         self._cache.clear()
  *         self._split_cache.clear()
  */
   __pyx_tuple__15 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_pop_data_pyx, __pyx_n_s_clear, 38, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_data_pyx, __pyx_n_s_clear, 38, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 38, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
   __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(2, 1, __pyx_L1_error)
@@ -14042,64 +14036,64 @@
  *     else:
  *         return __pyx_unpickle_MultidictCache, (type(self), 0x09e6f20, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_MultidictCache__set_state(self, __pyx_state)
  */
   __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(2, 16, __pyx_L1_error)
 
-  /* "pop/pop.data.pyx":127
+  /* "data.pyx":127
  *         return not self.__eq__(other)
  * 
  *     def keys(self):             # <<<<<<<<<<<<<<
  *         return self.__data.keys()
  * 
  */
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_pop_data_pyx, __pyx_n_s_keys, 127, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_data_pyx, __pyx_n_s_keys, 127, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 127, __pyx_L1_error)
 
-  /* "pop/pop.data.pyx":130
+  /* "data.pyx":130
  *         return self.__data.keys()
  * 
  *     def values(self):             # <<<<<<<<<<<<<<
  *         return self.__data.values()
  * 
  */
-  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_pop_data_pyx, __pyx_n_s_values, 130, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_data_pyx, __pyx_n_s_values, 130, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 130, __pyx_L1_error)
 
-  /* "pop/pop.data.pyx":133
+  /* "data.pyx":133
  *         return self.__data.values()
  * 
  *     def items(self):             # <<<<<<<<<<<<<<
  *         return self.__data.items()
  * 
  */
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_pop_data_pyx, __pyx_n_s_items, 133, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_data_pyx, __pyx_n_s_items, 133, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 133, __pyx_L1_error)
 
-  /* "pop/pop.data.pyx":136
+  /* "data.pyx":136
  *         return self.__data.items()
  * 
  *     def get(self, key, default=None):             # <<<<<<<<<<<<<<
  *         return self.__data.get(key, default)
  * 
  */
   __pyx_tuple__22 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_key, __pyx_n_s_default); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_pop_data_pyx, __pyx_n_s_get, 136, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_data_pyx, __pyx_n_s_get, 136, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 136, __pyx_L1_error)
   __pyx_tuple__24 = PyTuple_Pack(1, Py_None); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
 
-  /* "pop/pop.data.pyx":139
+  /* "data.pyx":139
  *         return self.__data.get(key, default)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         return unfreeze(self.__data)
  * 
  */
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_pop_data_pyx, __pyx_n_s_copy, 139, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_data_pyx, __pyx_n_s_copy, 139, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 139, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
   __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(2, 1, __pyx_L1_error)
@@ -14108,49 +14102,49 @@
  *     else:
  *         return __pyx_unpickle_ImmutableNamespaceDict, (type(self), 0x9077974, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_ImmutableNamespaceDict__set_state(self, __pyx_state)
  */
   __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(2, 16, __pyx_L1_error)
 
-  /* "pop/pop.data.pyx":143
+  /* "data.pyx":143
  * 
  * 
  * def freeze(data):             # <<<<<<<<<<<<<<
  *     if isinstance(data, ImmutableNamespaceDict):
  *         return data
  */
   __pyx_tuple__28 = PyTuple_Pack(6, __pyx_n_s_data, __pyx_n_s_key, __pyx_n_s_value, __pyx_n_s_genexpr, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_pop_data_pyx, __pyx_n_s_freeze, 143, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_data_pyx, __pyx_n_s_freeze, 143, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 143, __pyx_L1_error)
 
-  /* "pop/pop.data.pyx":155
+  /* "data.pyx":155
  *         return data
  * 
  * def unfreeze(data):             # <<<<<<<<<<<<<<
  *     if isinstance(data, ImmutableNamespaceDict):
  *         return {key: unfreeze(value) for key, value in data.items()}
  */
   __pyx_tuple__30 = PyTuple_Pack(5, __pyx_n_s_data, __pyx_n_s_key, __pyx_n_s_value, __pyx_n_s_value, __pyx_n_s_value); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__30);
   __Pyx_GIVEREF(__pyx_tuple__30);
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_pop_data_pyx, __pyx_n_s_unfreeze, 155, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_data_pyx, __pyx_n_s_unfreeze, 155, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 155, __pyx_L1_error)
 
-  /* "pop/pop.data.pyx":166
+  /* "data.pyx":166
  * 
  * 
  * cpdef update(dest, upd, bint recursive_update=True, bint merge_lists=False):             # <<<<<<<<<<<<<<
  *     """
  *     Recursive version of the default dict.update
  */
   __pyx_tuple__32 = PyTuple_Pack(4, __pyx_n_s_dest, __pyx_n_s_upd, __pyx_n_s_recursive_update, __pyx_n_s_merge_lists); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__32);
   __Pyx_GIVEREF(__pyx_tuple__32);
-  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_pop_data_pyx, __pyx_n_s_update, 166, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pop_data_pyx, __pyx_n_s_update, 166, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 166, __pyx_L1_error)
   __pyx_tuple__34 = PyTuple_Pack(2, Py_True, Py_False); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__34);
   __Pyx_GIVEREF(__pyx_tuple__34);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_NamespaceDict(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
@@ -14208,15 +14202,15 @@
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_import_code(void); /*proto*/
 
 static int __Pyx_modinit_global_init_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_global_init_code", 0);
   /*--- Global init code ---*/
-  __pyx_v_3pop_4data_DICT_ATTRS = ((PyObject*)Py_None); Py_INCREF(Py_None);
+  __pyx_v_4data_DICT_ATTRS = ((PyObject*)Py_None); Py_INCREF(Py_None);
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_variable_export_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_export_code", 0);
@@ -14240,160 +14234,160 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   #if CYTHON_USE_TYPE_SPECS
   __pyx_t_1 = PyTuple_Pack(1, (PyObject *)(&PyDict_Type)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3pop_4data_NamespaceDict = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_3pop_4data_NamespaceDict_spec, __pyx_t_1);
+  __pyx_ptype_4data_NamespaceDict = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4data_NamespaceDict_spec, __pyx_t_1);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_ptype_3pop_4data_NamespaceDict)) __PYX_ERR(0, 11, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_3pop_4data_NamespaceDict_spec, __pyx_ptype_3pop_4data_NamespaceDict) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
+  if (unlikely(!__pyx_ptype_4data_NamespaceDict)) __PYX_ERR(0, 11, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4data_NamespaceDict_spec, __pyx_ptype_4data_NamespaceDict) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   #else
-  __pyx_ptype_3pop_4data_NamespaceDict = &__pyx_type_3pop_4data_NamespaceDict;
+  __pyx_ptype_4data_NamespaceDict = &__pyx_type_4data_NamespaceDict;
   #endif
-  if (sizeof(struct __pyx_obj_3pop_4data_NamespaceDict) != sizeof(PyDictObject)) {
+  if (sizeof(struct __pyx_obj_4data_NamespaceDict) != sizeof(PyDictObject)) {
     if (__Pyx_validate_extern_base((&PyDict_Type)) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   }
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  __pyx_ptype_3pop_4data_NamespaceDict->tp_dealloc = (&PyDict_Type)->tp_dealloc;
-  __pyx_ptype_3pop_4data_NamespaceDict->tp_base = (&PyDict_Type);
-  __pyx_ptype_3pop_4data_NamespaceDict->tp_new = (&PyDict_Type)->tp_new;
+  __pyx_ptype_4data_NamespaceDict->tp_dealloc = (&PyDict_Type)->tp_dealloc;
+  __pyx_ptype_4data_NamespaceDict->tp_base = (&PyDict_Type);
+  __pyx_ptype_4data_NamespaceDict->tp_new = (&PyDict_Type)->tp_new;
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_3pop_4data_NamespaceDict) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_4data_NamespaceDict) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
-  __pyx_ptype_3pop_4data_NamespaceDict->tp_print = 0;
+  __pyx_ptype_4data_NamespaceDict->tp_print = 0;
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_NamespaceDict, (PyObject *) __pyx_ptype_3pop_4data_NamespaceDict) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_NamespaceDict, (PyObject *) __pyx_ptype_4data_NamespaceDict) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_3pop_4data_NamespaceDict) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4data_NamespaceDict) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   #endif
-  __pyx_vtabptr_3pop_4data_MultidictCache = &__pyx_vtable_3pop_4data_MultidictCache;
-  __pyx_vtable_3pop_4data_MultidictCache._clear = (PyObject *(*)(struct __pyx_obj_3pop_4data_MultidictCache *, int __pyx_skip_dispatch))__pyx_f_3pop_4data_14MultidictCache__clear;
+  __pyx_vtabptr_4data_MultidictCache = &__pyx_vtable_4data_MultidictCache;
+  __pyx_vtable_4data_MultidictCache._clear = (PyObject *(*)(struct __pyx_obj_4data_MultidictCache *, int __pyx_skip_dispatch))__pyx_f_4data_14MultidictCache__clear;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_3pop_4data_MultidictCache = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_3pop_4data_MultidictCache_spec, NULL); if (unlikely(!__pyx_ptype_3pop_4data_MultidictCache)) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_3pop_4data_MultidictCache_spec, __pyx_ptype_3pop_4data_MultidictCache) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_ptype_4data_MultidictCache = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4data_MultidictCache_spec, NULL); if (unlikely(!__pyx_ptype_4data_MultidictCache)) __PYX_ERR(0, 26, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4data_MultidictCache_spec, __pyx_ptype_4data_MultidictCache) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   #else
-  __pyx_ptype_3pop_4data_MultidictCache = &__pyx_type_3pop_4data_MultidictCache;
+  __pyx_ptype_4data_MultidictCache = &__pyx_type_4data_MultidictCache;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_3pop_4data_MultidictCache) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_4data_MultidictCache) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
-  __pyx_ptype_3pop_4data_MultidictCache->tp_print = 0;
+  __pyx_ptype_4data_MultidictCache->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_3pop_4data_MultidictCache->tp_dictoffset && __pyx_ptype_3pop_4data_MultidictCache->tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_ptype_3pop_4data_MultidictCache->tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_4data_MultidictCache->tp_dictoffset && __pyx_ptype_4data_MultidictCache->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_4data_MultidictCache->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_3pop_4data_MultidictCache, __pyx_vtabptr_3pop_4data_MultidictCache) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_4data_MultidictCache, __pyx_vtabptr_4data_MultidictCache) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_3pop_4data_MultidictCache) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_4data_MultidictCache) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MultidictCache, (PyObject *) __pyx_ptype_3pop_4data_MultidictCache) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MultidictCache, (PyObject *) __pyx_ptype_4data_MultidictCache) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_3pop_4data_MultidictCache) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4data_MultidictCache) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_3pop_4data_ImmutableNamespaceDict = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_3pop_4data_ImmutableNamespaceDict_spec, NULL); if (unlikely(!__pyx_ptype_3pop_4data_ImmutableNamespaceDict)) __PYX_ERR(0, 68, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_3pop_4data_ImmutableNamespaceDict_spec, __pyx_ptype_3pop_4data_ImmutableNamespaceDict) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_ptype_4data_ImmutableNamespaceDict = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4data_ImmutableNamespaceDict_spec, NULL); if (unlikely(!__pyx_ptype_4data_ImmutableNamespaceDict)) __PYX_ERR(0, 68, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4data_ImmutableNamespaceDict_spec, __pyx_ptype_4data_ImmutableNamespaceDict) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
   #else
-  __pyx_ptype_3pop_4data_ImmutableNamespaceDict = &__pyx_type_3pop_4data_ImmutableNamespaceDict;
+  __pyx_ptype_4data_ImmutableNamespaceDict = &__pyx_type_4data_ImmutableNamespaceDict;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_3pop_4data_ImmutableNamespaceDict) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_4data_ImmutableNamespaceDict) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
-  __pyx_ptype_3pop_4data_ImmutableNamespaceDict->tp_print = 0;
+  __pyx_ptype_4data_ImmutableNamespaceDict->tp_print = 0;
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ImmutableNamespaceDict, (PyObject *) __pyx_ptype_3pop_4data_ImmutableNamespaceDict) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ImmutableNamespaceDict, (PyObject *) __pyx_ptype_4data_ImmutableNamespaceDict) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_3pop_4data_ImmutableNamespaceDict) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4data_ImmutableNamespaceDict) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_3pop_4data___pyx_scope_struct____contains__ = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_3pop_4data___pyx_scope_struct____contains___spec, NULL); if (unlikely(!__pyx_ptype_3pop_4data___pyx_scope_struct____contains__)) __PYX_ERR(0, 65, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_3pop_4data___pyx_scope_struct____contains___spec, __pyx_ptype_3pop_4data___pyx_scope_struct____contains__) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_ptype_4data___pyx_scope_struct____contains__ = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4data___pyx_scope_struct____contains___spec, NULL); if (unlikely(!__pyx_ptype_4data___pyx_scope_struct____contains__)) __PYX_ERR(0, 65, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4data___pyx_scope_struct____contains___spec, __pyx_ptype_4data___pyx_scope_struct____contains__) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
   #else
-  __pyx_ptype_3pop_4data___pyx_scope_struct____contains__ = &__pyx_type_3pop_4data___pyx_scope_struct____contains__;
+  __pyx_ptype_4data___pyx_scope_struct____contains__ = &__pyx_type_4data___pyx_scope_struct____contains__;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_3pop_4data___pyx_scope_struct____contains__) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_4data___pyx_scope_struct____contains__) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
-  __pyx_ptype_3pop_4data___pyx_scope_struct____contains__->tp_print = 0;
+  __pyx_ptype_4data___pyx_scope_struct____contains__->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_3pop_4data___pyx_scope_struct____contains__->tp_dictoffset && __pyx_ptype_3pop_4data___pyx_scope_struct____contains__->tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_ptype_3pop_4data___pyx_scope_struct____contains__->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_4data___pyx_scope_struct____contains__->tp_dictoffset && __pyx_ptype_4data___pyx_scope_struct____contains__->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_4data___pyx_scope_struct____contains__->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_3pop_4data___pyx_scope_struct_1_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_3pop_4data___pyx_scope_struct_1_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_3pop_4data___pyx_scope_struct_1_genexpr)) __PYX_ERR(0, 66, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_3pop_4data___pyx_scope_struct_1_genexpr_spec, __pyx_ptype_3pop_4data___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_ptype_4data___pyx_scope_struct_1_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4data___pyx_scope_struct_1_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_4data___pyx_scope_struct_1_genexpr)) __PYX_ERR(0, 66, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4data___pyx_scope_struct_1_genexpr_spec, __pyx_ptype_4data___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
   #else
-  __pyx_ptype_3pop_4data___pyx_scope_struct_1_genexpr = &__pyx_type_3pop_4data___pyx_scope_struct_1_genexpr;
+  __pyx_ptype_4data___pyx_scope_struct_1_genexpr = &__pyx_type_4data___pyx_scope_struct_1_genexpr;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_3pop_4data___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_4data___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
-  __pyx_ptype_3pop_4data___pyx_scope_struct_1_genexpr->tp_print = 0;
+  __pyx_ptype_4data___pyx_scope_struct_1_genexpr->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_3pop_4data___pyx_scope_struct_1_genexpr->tp_dictoffset && __pyx_ptype_3pop_4data___pyx_scope_struct_1_genexpr->tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_ptype_3pop_4data___pyx_scope_struct_1_genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_4data___pyx_scope_struct_1_genexpr->tp_dictoffset && __pyx_ptype_4data___pyx_scope_struct_1_genexpr->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_4data___pyx_scope_struct_1_genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_3pop_4data___pyx_scope_struct_2_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_3pop_4data___pyx_scope_struct_2_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_3pop_4data___pyx_scope_struct_2_genexpr)) __PYX_ERR(0, 149, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_3pop_4data___pyx_scope_struct_2_genexpr_spec, __pyx_ptype_3pop_4data___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_ptype_4data___pyx_scope_struct_2_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4data___pyx_scope_struct_2_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_4data___pyx_scope_struct_2_genexpr)) __PYX_ERR(0, 149, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4data___pyx_scope_struct_2_genexpr_spec, __pyx_ptype_4data___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
   #else
-  __pyx_ptype_3pop_4data___pyx_scope_struct_2_genexpr = &__pyx_type_3pop_4data___pyx_scope_struct_2_genexpr;
+  __pyx_ptype_4data___pyx_scope_struct_2_genexpr = &__pyx_type_4data___pyx_scope_struct_2_genexpr;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_3pop_4data___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_4data___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
-  __pyx_ptype_3pop_4data___pyx_scope_struct_2_genexpr->tp_print = 0;
+  __pyx_ptype_4data___pyx_scope_struct_2_genexpr->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_3pop_4data___pyx_scope_struct_2_genexpr->tp_dictoffset && __pyx_ptype_3pop_4data___pyx_scope_struct_2_genexpr->tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_ptype_3pop_4data___pyx_scope_struct_2_genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_4data___pyx_scope_struct_2_genexpr->tp_dictoffset && __pyx_ptype_4data___pyx_scope_struct_2_genexpr->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_4data___pyx_scope_struct_2_genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_3pop_4data___pyx_scope_struct_3_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_3pop_4data___pyx_scope_struct_3_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_3pop_4data___pyx_scope_struct_3_genexpr)) __PYX_ERR(0, 151, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_3pop_4data___pyx_scope_struct_3_genexpr_spec, __pyx_ptype_3pop_4data___pyx_scope_struct_3_genexpr) < 0) __PYX_ERR(0, 151, __pyx_L1_error)
+  __pyx_ptype_4data___pyx_scope_struct_3_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4data___pyx_scope_struct_3_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_4data___pyx_scope_struct_3_genexpr)) __PYX_ERR(0, 151, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4data___pyx_scope_struct_3_genexpr_spec, __pyx_ptype_4data___pyx_scope_struct_3_genexpr) < 0) __PYX_ERR(0, 151, __pyx_L1_error)
   #else
-  __pyx_ptype_3pop_4data___pyx_scope_struct_3_genexpr = &__pyx_type_3pop_4data___pyx_scope_struct_3_genexpr;
+  __pyx_ptype_4data___pyx_scope_struct_3_genexpr = &__pyx_type_4data___pyx_scope_struct_3_genexpr;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_3pop_4data___pyx_scope_struct_3_genexpr) < 0) __PYX_ERR(0, 151, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_4data___pyx_scope_struct_3_genexpr) < 0) __PYX_ERR(0, 151, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
-  __pyx_ptype_3pop_4data___pyx_scope_struct_3_genexpr->tp_print = 0;
+  __pyx_ptype_4data___pyx_scope_struct_3_genexpr->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_3pop_4data___pyx_scope_struct_3_genexpr->tp_dictoffset && __pyx_ptype_3pop_4data___pyx_scope_struct_3_genexpr->tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_ptype_3pop_4data___pyx_scope_struct_3_genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_4data___pyx_scope_struct_3_genexpr->tp_dictoffset && __pyx_ptype_4data___pyx_scope_struct_3_genexpr->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_4data___pyx_scope_struct_3_genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -14699,22 +14693,22 @@
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_pop__data) {
+  if (__pyx_module_is_main_data) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "pop.data")) {
-      if (unlikely((PyDict_SetItemString(modules, "pop.data", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "data")) {
+      if (unlikely((PyDict_SetItemString(modules, "data", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -14727,15 +14721,15 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "pop/pop.data.pyx":3
+  /* "data.pyx":3
  * # cython: language_level=3
  * 
  * from collections.abc import Mapping             # <<<<<<<<<<<<<<
  * from cpython cimport dict
  * from cython cimport pint
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
@@ -14748,249 +14742,249 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_Mapping); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Mapping, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pop/pop.data.pyx":9
+  /* "data.pyx":9
  * 
  * 
  * cdef frozenset DICT_ATTRS = frozenset(dir(dict))             # <<<<<<<<<<<<<<
  * 
  * cdef class NamespaceDict(dict[str, object]):
  */
   __pyx_t_3 = PyObject_Dir(((PyObject *)(&PyDict_Type))); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = __Pyx_PyFrozenSet_New(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_XGOTREF(__pyx_v_3pop_4data_DICT_ATTRS);
-  __Pyx_DECREF_SET(__pyx_v_3pop_4data_DICT_ATTRS, ((PyObject*)__pyx_t_2));
+  __Pyx_XGOTREF(__pyx_v_4data_DICT_ATTRS);
+  __Pyx_DECREF_SET(__pyx_v_4data_DICT_ATTRS, ((PyObject*)__pyx_t_2));
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_13NamespaceDict_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_NamespaceDict___reduce_cython, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_13NamespaceDict_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_NamespaceDict___reduce_cython, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_3pop_4data_NamespaceDict, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_4data_NamespaceDict, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  PyType_Modified(__pyx_ptype_3pop_4data_NamespaceDict);
+  PyType_Modified(__pyx_ptype_4data_NamespaceDict);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_NamespaceDict, (type(self), 0xe3b0c44, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_NamespaceDict__set_state(self, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_13NamespaceDict_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_NamespaceDict___setstate_cython, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_13NamespaceDict_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_NamespaceDict___setstate_cython, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_3pop_4data_NamespaceDict, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(2, 16, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_4data_NamespaceDict, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  PyType_Modified(__pyx_ptype_3pop_4data_NamespaceDict);
+  PyType_Modified(__pyx_ptype_4data_NamespaceDict);
 
-  /* "pop/pop.data.pyx":38
+  /* "data.pyx":38
  *         self._split_cache = dict[str, list[str]]()
  * 
  *     cpdef _clear(self):             # <<<<<<<<<<<<<<
  *         self._cache.clear()
  *         self._split_cache.clear()
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_14MultidictCache_3_clear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_MultidictCache__clear, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_14MultidictCache_3_clear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_MultidictCache__clear, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_3pop_4data_MultidictCache, __pyx_n_s_clear, __pyx_t_2) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_4data_MultidictCache, __pyx_n_s_clear, __pyx_t_2) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  PyType_Modified(__pyx_ptype_3pop_4data_MultidictCache);
+  PyType_Modified(__pyx_ptype_4data_MultidictCache);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_14MultidictCache_11__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_MultidictCache___reduce_cython, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_14MultidictCache_11__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_MultidictCache___reduce_cython, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_3pop_4data_MultidictCache, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_4data_MultidictCache, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  PyType_Modified(__pyx_ptype_3pop_4data_MultidictCache);
+  PyType_Modified(__pyx_ptype_4data_MultidictCache);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_MultidictCache, (type(self), 0x09e6f20, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_MultidictCache__set_state(self, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_14MultidictCache_13__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_MultidictCache___setstate_cython, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_14MultidictCache_13__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_MultidictCache___setstate_cython, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_3pop_4data_MultidictCache, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(2, 16, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_4data_MultidictCache, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  PyType_Modified(__pyx_ptype_3pop_4data_MultidictCache);
+  PyType_Modified(__pyx_ptype_4data_MultidictCache);
 
-  /* "pop/pop.data.pyx":127
+  /* "data.pyx":127
  *         return not self.__eq__(other)
  * 
  *     def keys(self):             # <<<<<<<<<<<<<<
  *         return self.__data.keys()
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_22ImmutableNamespaceDict_27keys, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ImmutableNamespaceDict_keys, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_22ImmutableNamespaceDict_27keys, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ImmutableNamespaceDict_keys, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_3pop_4data_ImmutableNamespaceDict, __pyx_n_s_keys, __pyx_t_2) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_4data_ImmutableNamespaceDict, __pyx_n_s_keys, __pyx_t_2) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  PyType_Modified(__pyx_ptype_3pop_4data_ImmutableNamespaceDict);
+  PyType_Modified(__pyx_ptype_4data_ImmutableNamespaceDict);
 
-  /* "pop/pop.data.pyx":130
+  /* "data.pyx":130
  *         return self.__data.keys()
  * 
  *     def values(self):             # <<<<<<<<<<<<<<
  *         return self.__data.values()
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_22ImmutableNamespaceDict_29values, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ImmutableNamespaceDict_values, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_22ImmutableNamespaceDict_29values, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ImmutableNamespaceDict_values, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_3pop_4data_ImmutableNamespaceDict, __pyx_n_s_values, __pyx_t_2) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_4data_ImmutableNamespaceDict, __pyx_n_s_values, __pyx_t_2) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  PyType_Modified(__pyx_ptype_3pop_4data_ImmutableNamespaceDict);
+  PyType_Modified(__pyx_ptype_4data_ImmutableNamespaceDict);
 
-  /* "pop/pop.data.pyx":133
+  /* "data.pyx":133
  *         return self.__data.values()
  * 
  *     def items(self):             # <<<<<<<<<<<<<<
  *         return self.__data.items()
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_22ImmutableNamespaceDict_31items, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ImmutableNamespaceDict_items, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_22ImmutableNamespaceDict_31items, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ImmutableNamespaceDict_items, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_3pop_4data_ImmutableNamespaceDict, __pyx_n_s_items, __pyx_t_2) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_4data_ImmutableNamespaceDict, __pyx_n_s_items, __pyx_t_2) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  PyType_Modified(__pyx_ptype_3pop_4data_ImmutableNamespaceDict);
+  PyType_Modified(__pyx_ptype_4data_ImmutableNamespaceDict);
 
-  /* "pop/pop.data.pyx":136
+  /* "data.pyx":136
  *         return self.__data.items()
  * 
  *     def get(self, key, default=None):             # <<<<<<<<<<<<<<
  *         return self.__data.get(key, default)
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_22ImmutableNamespaceDict_33get, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ImmutableNamespaceDict_get, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_22ImmutableNamespaceDict_33get, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ImmutableNamespaceDict_get, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__24);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_3pop_4data_ImmutableNamespaceDict, __pyx_n_s_get, __pyx_t_2) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_4data_ImmutableNamespaceDict, __pyx_n_s_get, __pyx_t_2) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  PyType_Modified(__pyx_ptype_3pop_4data_ImmutableNamespaceDict);
+  PyType_Modified(__pyx_ptype_4data_ImmutableNamespaceDict);
 
-  /* "pop/pop.data.pyx":139
+  /* "data.pyx":139
  *         return self.__data.get(key, default)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         return unfreeze(self.__data)
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_22ImmutableNamespaceDict_35copy, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ImmutableNamespaceDict_copy, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_22ImmutableNamespaceDict_35copy, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ImmutableNamespaceDict_copy, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_3pop_4data_ImmutableNamespaceDict, __pyx_n_s_copy, __pyx_t_2) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_4data_ImmutableNamespaceDict, __pyx_n_s_copy, __pyx_t_2) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  PyType_Modified(__pyx_ptype_3pop_4data_ImmutableNamespaceDict);
+  PyType_Modified(__pyx_ptype_4data_ImmutableNamespaceDict);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_22ImmutableNamespaceDict_37__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ImmutableNamespaceDict___reduce, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_22ImmutableNamespaceDict_37__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ImmutableNamespaceDict___reduce, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_3pop_4data_ImmutableNamespaceDict, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_4data_ImmutableNamespaceDict, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  PyType_Modified(__pyx_ptype_3pop_4data_ImmutableNamespaceDict);
+  PyType_Modified(__pyx_ptype_4data_ImmutableNamespaceDict);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_ImmutableNamespaceDict, (type(self), 0x9077974, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_ImmutableNamespaceDict__set_state(self, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_22ImmutableNamespaceDict_39__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ImmutableNamespaceDict___setstat, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_22ImmutableNamespaceDict_39__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ImmutableNamespaceDict___setstat, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_3pop_4data_ImmutableNamespaceDict, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(2, 16, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_4data_ImmutableNamespaceDict, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  PyType_Modified(__pyx_ptype_3pop_4data_ImmutableNamespaceDict);
+  PyType_Modified(__pyx_ptype_4data_ImmutableNamespaceDict);
 
-  /* "pop/pop.data.pyx":143
+  /* "data.pyx":143
  * 
  * 
  * def freeze(data):             # <<<<<<<<<<<<<<
  *     if isinstance(data, ImmutableNamespaceDict):
  *         return data
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_1freeze, 0, __pyx_n_s_freeze, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_1freeze, 0, __pyx_n_s_freeze, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_freeze, __pyx_t_2) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pop/pop.data.pyx":155
+  /* "data.pyx":155
  *         return data
  * 
  * def unfreeze(data):             # <<<<<<<<<<<<<<
  *     if isinstance(data, ImmutableNamespaceDict):
  *         return {key: unfreeze(value) for key, value in data.items()}
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_3unfreeze, 0, __pyx_n_s_unfreeze, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_3unfreeze, 0, __pyx_n_s_unfreeze, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_unfreeze, __pyx_t_2) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pop/pop.data.pyx":166
+  /* "data.pyx":166
  * 
  * 
  * cpdef update(dest, upd, bint recursive_update=True, bint merge_lists=False):             # <<<<<<<<<<<<<<
  *     """
  *     Recursive version of the default dict.update
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_5update, 0, __pyx_n_s_update, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_5update, 0, __pyx_n_s_update, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__34);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_update, __pyx_t_2) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_NamespaceDict(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_7__pyx_unpickle_NamespaceDict, 0, __pyx_n_s_pyx_unpickle_NamespaceDict, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_7__pyx_unpickle_NamespaceDict, 0, __pyx_n_s_pyx_unpickle_NamespaceDict, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_NamespaceDict, __pyx_t_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_NamespaceDict__set_state(<NamespaceDict> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_NamespaceDict__set_state(NamespaceDict __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     if len(__pyx_state) > 0 and hasattr(__pyx_result, '__dict__'):
  *         __pyx_result.__dict__.update(__pyx_state[0])
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_9__pyx_unpickle_MultidictCache, 0, __pyx_n_s_pyx_unpickle_MultidictCache, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_9__pyx_unpickle_MultidictCache, 0, __pyx_n_s_pyx_unpickle_MultidictCache, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_MultidictCache, __pyx_t_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_ImmutableNamespaceDict(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_3pop_4data_11__pyx_unpickle_ImmutableNamespaceDict, 0, __pyx_n_s_pyx_unpickle_ImmutableNamespac, NULL, __pyx_n_s_pop_data, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4data_11__pyx_unpickle_ImmutableNamespaceDict, 0, __pyx_n_s_pyx_unpickle_ImmutableNamespac, NULL, __pyx_n_s_data, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_ImmutableNamespac, __pyx_t_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pop/pop.data.pyx":1
+  /* "data.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * 
  * from collections.abc import Mapping
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -15000,29 +14994,29 @@
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   if (__pyx_m) {
     if (__pyx_d && stringtab_initialized) {
-      __Pyx_AddTraceback("init pop.data", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init data", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
     #else
     Py_DECREF(__pyx_m);
     if (pystate_addmodule_run) {
       PyObject *tp, *value, *tb;
       PyErr_Fetch(&tp, &value, &tb);
       PyState_RemoveModule(&__pyx_moduledef);
       PyErr_Restore(tp, value, tb);
     }
     #endif
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init pop.data");
+    PyErr_SetString(PyExc_ImportError, "init data");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
```

### Comparing `cpop-28.0.4/pop/pop.data.pyx` & `cpop-28.0.5/pop/data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-28.0.4/pop/ref.py` & `cpop-28.0.5/pop/ref.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.4/pop/scanner.py` & `cpop-28.0.5/pop/scanner.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.4/pop/verify.py` & `cpop-28.0.5/pop/verify.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.4/pyproject.toml` & `cpop-28.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpop"
-version = "28.0.4"
+version = "28.0.5"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch@saltstack.com"},
 ]
 classifiers = [
```

### Comparing `cpop-28.0.4/setup.py` & `cpop-28.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,23 +27,23 @@
                         shutil.rmtree(os.path.join(root, dir_))
 
 
 def discover_packages():
     modules = []
     # dot-delimited list of modules to not package. It's not good to package tests:
     skip_mods = ["tests"]
-    for package in (NAME,):
+    for package in ("pop", "hub"):
         for root, _, files in os.walk(os.path.join(SETUP_DIRNAME, package)):
             pdir = os.path.relpath(root, SETUP_DIRNAME)
             modname = pdir.replace(os.sep, ".")
             if modname not in skip_mods:
                 modules.append(modname)
     return modules
 
 
 
 setup(
-    ext_modules=cythonize(os.path.join("pop", "pop.data.pyx")),
+    ext_modules=cythonize(os.path.join("pop", "data.pyx")),
     packages=discover_packages(),
     cmdclass={"clean": Clean},
 
 )
```

