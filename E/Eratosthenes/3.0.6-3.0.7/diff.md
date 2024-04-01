# Comparing `tmp/Eratosthenes-3.0.6.tar.gz` & `tmp/Eratosthenes-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Eratosthenes-3.0.6.tar", last modified: Sun Mar 31 22:39:33 2024, max compression
+gzip compressed data, was "Eratosthenes-3.0.7.tar", last modified: Mon Apr  1 14:08:01 2024, max compression
```

## Comparing `Eratosthenes-3.0.6.tar` & `Eratosthenes-3.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-03-31 22:39:33.062950 Eratosthenes-3.0.6/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-03-31 22:39:33.062950 Eratosthenes-3.0.6/Eratosthenes.egg-info/
--rw-r--r--   0 iamu      (1000) iamu      (1000)     1550 2024-03-31 22:39:33.000000 Eratosthenes-3.0.6/Eratosthenes.egg-info/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      305 2024-03-31 22:39:33.000000 Eratosthenes-3.0.6/Eratosthenes.egg-info/SOURCES.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2024-03-31 22:39:33.000000 Eratosthenes-3.0.6/Eratosthenes.egg-info/dependency_links.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       13 2024-03-31 22:39:33.000000 Eratosthenes-3.0.6/Eratosthenes.egg-info/top_level.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1064 2024-03-26 16:40:08.000000 Eratosthenes-3.0.6/LICENSE
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       19 2024-03-26 17:27:20.000000 Eratosthenes-3.0.6/MANIFEST.in
--rw-r--r--   0 iamu      (1000) iamu      (1000)     1550 2024-03-31 22:39:33.062950 Eratosthenes-3.0.6/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      814 2024-03-29 23:46:05.000000 Eratosthenes-3.0.6/README.md
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2024-03-31 22:39:33.062950 Eratosthenes-3.0.6/setup.cfg
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1318 2024-03-31 22:38:52.000000 Eratosthenes-3.0.6/setup.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-03-31 22:39:33.062950 Eratosthenes-3.0.6/src/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2895 2024-03-30 14:21:10.000000 Eratosthenes-3.0.6/src/dispatchqueue.cpp
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-03-31 22:39:33.062950 Eratosthenes-3.0.6/src/include/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      767 2024-03-26 15:47:52.000000 Eratosthenes-3.0.6/src/include/config.h
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1941 2024-03-30 14:18:47.000000 Eratosthenes-3.0.6/src/include/dispatchqueue.hpp
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3651 2024-03-30 20:24:43.000000 Eratosthenes-3.0.6/src/include/prime_generator.hpp
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    14916 2024-03-31 22:36:51.000000 Eratosthenes-3.0.6/src/prime_gen.cpp
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-01 14:08:01.949711 Eratosthenes-3.0.7/
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-01 14:08:01.949711 Eratosthenes-3.0.7/Eratosthenes.egg-info/
+-rw-r--r--   0 iamu      (1000) iamu      (1000)     1550 2024-04-01 14:08:01.000000 Eratosthenes-3.0.7/Eratosthenes.egg-info/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      305 2024-04-01 14:08:01.000000 Eratosthenes-3.0.7/Eratosthenes.egg-info/SOURCES.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2024-04-01 14:08:01.000000 Eratosthenes-3.0.7/Eratosthenes.egg-info/dependency_links.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       13 2024-04-01 14:08:01.000000 Eratosthenes-3.0.7/Eratosthenes.egg-info/top_level.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1064 2024-03-26 16:40:08.000000 Eratosthenes-3.0.7/LICENSE
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       19 2024-03-26 17:27:20.000000 Eratosthenes-3.0.7/MANIFEST.in
+-rw-r--r--   0 iamu      (1000) iamu      (1000)     1550 2024-04-01 14:08:01.949711 Eratosthenes-3.0.7/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      814 2024-03-29 23:46:05.000000 Eratosthenes-3.0.7/README.md
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2024-04-01 14:08:01.949711 Eratosthenes-3.0.7/setup.cfg
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1318 2024-04-01 14:07:19.000000 Eratosthenes-3.0.7/setup.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-01 14:08:01.949711 Eratosthenes-3.0.7/src/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2895 2024-04-01 14:02:53.000000 Eratosthenes-3.0.7/src/dispatchqueue.cpp
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-01 14:08:01.949711 Eratosthenes-3.0.7/src/include/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      767 2024-03-26 15:47:52.000000 Eratosthenes-3.0.7/src/include/config.h
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1941 2024-03-30 14:18:47.000000 Eratosthenes-3.0.7/src/include/dispatchqueue.hpp
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     3651 2024-03-30 20:24:43.000000 Eratosthenes-3.0.7/src/include/prime_generator.hpp
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    14917 2024-04-01 14:06:17.000000 Eratosthenes-3.0.7/src/prime_gen.cpp
```

### Comparing `Eratosthenes-3.0.6/Eratosthenes.egg-info/PKG-INFO` & `Eratosthenes-3.0.7/Eratosthenes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Eratosthenes
-Version: 3.0.6
+Version: 3.0.7
 Summary: Fast prime generation for Python based on Sieve of Eratosthenes and Trial Division
 Home-page: https://github.com/vm6502q/Eratosthenes
 Author: Dan Strano
 Author-email: dan@unitary.fund
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `Eratosthenes-3.0.6/LICENSE` & `Eratosthenes-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Eratosthenes-3.0.6/PKG-INFO` & `Eratosthenes-3.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Eratosthenes
-Version: 3.0.6
+Version: 3.0.7
 Summary: Fast prime generation for Python based on Sieve of Eratosthenes and Trial Division
 Home-page: https://github.com/vm6502q/Eratosthenes
 Author: Dan Strano
 Author-email: dan@unitary.fund
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `Eratosthenes-3.0.6/README.md` & `Eratosthenes-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `Eratosthenes-3.0.6/setup.py` & `Eratosthenes-3.0.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         language='c++',
         extra_compile_args = cpp_args,
     ),
 ]
 
 setup(
     name='Eratosthenes',
-    version='3.0.6',
+    version='3.0.7',
     author='Dan Strano',
     author_email='dan@unitary.fund',
     description='Fast prime generation for Python based on Sieve of Eratosthenes and Trial Division',
     long_description=README,
     long_description_content_type='text/markdown',
     url="https://github.com/vm6502q/Eratosthenes",
     license="MIT",
```

### Comparing `Eratosthenes-3.0.6/src/dispatchqueue.cpp` & `Eratosthenes-3.0.7/src/dispatchqueue.cpp`

 * *Files identical despite different names*

### Comparing `Eratosthenes-3.0.6/src/include/config.h` & `Eratosthenes-3.0.7/src/include/config.h`

 * *Files identical despite different names*

### Comparing `Eratosthenes-3.0.6/src/include/dispatchqueue.hpp` & `Eratosthenes-3.0.7/src/include/dispatchqueue.hpp`

 * *Files identical despite different names*

### Comparing `Eratosthenes-3.0.6/src/include/prime_generator.hpp` & `Eratosthenes-3.0.7/src/include/prime_generator.hpp`

 * *Files identical despite different names*

### Comparing `Eratosthenes-3.0.6/src/prime_gen.cpp` & `Eratosthenes-3.0.7/src/prime_gen.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,15 @@
                 }
 
                 return false;
             });
         }
         dispatch.finish();
 
-        if (knownPrimes.back() > sqrtnp1) {
+        if (knownPrimes.back() >= sqrtnp1) {
             for (size_t o = 1U; o <= cardinality; ++o) {
                 if (!notPrime[o]) {
                     ++count;
                 }
             }
         } else {
             for (size_t o = 1U; o <= cardinality; ++o) {
```

