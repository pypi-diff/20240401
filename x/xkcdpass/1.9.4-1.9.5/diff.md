# Comparing `tmp/xkcdpass-1.9.4.tar.gz` & `tmp/xkcdpass-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xkcdpass-1.9.4.tar", last modified: Fri Mar 24 22:04:28 2017, max compression
+gzip compressed data, was "dist/xkcdpass-1.9.5.tar", last modified: Mon Mar 27 10:40:37 2017, max compression
```

## Comparing `xkcdpass-1.9.4.tar` & `xkcdpass-1.9.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 steven    (1000) steven    (1000)        0 2017-03-24 22:04:27.000000 xkcdpass-1.9.4/
--rw-rw-rw-   0 steven    (1000) steven    (1000)     1524 2017-03-24 21:56:48.000000 xkcdpass-1.9.4/LICENSE.BSD
--rw-rw-rw-   0 steven    (1000) steven    (1000)      100 2016-09-04 16:12:50.000000 xkcdpass-1.9.4/MANIFEST.in
--rw-rw-rw-   0 steven    (1000) steven    (1000)     9795 2017-03-24 22:04:27.000000 xkcdpass-1.9.4/PKG-INFO
--rw-rw-rw-   0 steven    (1000) steven    (1000)     7503 2017-03-24 22:02:08.000000 xkcdpass-1.9.4/README.rst
-drwxrwxrwx   0 steven    (1000) steven    (1000)        0 2017-03-24 22:04:27.000000 xkcdpass-1.9.4/examples/
--rw-rw-rw-   0 steven    (1000) steven    (1000)      464 2016-09-04 16:12:50.000000 xkcdpass-1.9.4/examples/example_import.py
--rw-rw-rw-   0 steven    (1000) steven    (1000)      864 2017-03-24 21:56:48.000000 xkcdpass-1.9.4/examples/example_json.py
--rwxrwxrwx   0 steven    (1000) steven    (1000)      689 2017-03-24 21:56:48.000000 xkcdpass-1.9.4/examples/example_postprocess.py
--rw-rw-rw-   0 steven    (1000) steven    (1000)       59 2017-03-24 22:04:27.000000 xkcdpass-1.9.4/setup.cfg
--rw-rw-rw-   0 steven    (1000) steven    (1000)     1114 2017-03-24 22:00:50.000000 xkcdpass-1.9.4/setup.py
-drwxrwxrwx   0 steven    (1000) steven    (1000)        0 2017-03-24 22:04:27.000000 xkcdpass-1.9.4/tests/
--rw-rw-rw-   0 steven    (1000) steven    (1000)       66 2016-09-04 16:12:50.000000 xkcdpass-1.9.4/tests/test_list.txt
--rw-rw-rw-   0 steven    (1000) steven    (1000)     1530 2016-09-04 16:12:50.000000 xkcdpass-1.9.4/tests/xkcdp_tests.py
-drwxrwxrwx   0 steven    (1000) steven    (1000)        0 2017-03-24 22:04:27.000000 xkcdpass-1.9.4/xkcdpass/
--rw-rw-rw-   0 steven    (1000) steven    (1000)        0 2016-09-04 16:12:50.000000 xkcdpass-1.9.4/xkcdpass/__init__.py
-drwxrwxrwx   0 steven    (1000) steven    (1000)        0 2017-03-24 22:04:27.000000 xkcdpass-1.9.4/xkcdpass/static/
--rw-rw-rw-   0 steven    (1000) steven    (1000)   691880 2017-03-24 21:56:48.000000 xkcdpass-1.9.4/xkcdpass/static/default.txt
--rwxrwxrwx   0 steven    (1000) steven    (1000)    12958 2017-03-24 21:56:48.000000 xkcdpass-1.9.4/xkcdpass/xkcd_password.py
--rw-rw-rw-   0 steven    (1000) steven    (1000)     3293 2016-09-04 16:12:50.000000 xkcdpass-1.9.4/xkcdpass.1
-drwxrwxrwx   0 steven    (1000) steven    (1000)        0 2017-03-24 22:04:27.000000 xkcdpass-1.9.4/xkcdpass.egg-info/
--rw-rw-rw-   0 steven    (1000) steven    (1000)     9795 2017-03-24 22:04:27.000000 xkcdpass-1.9.4/xkcdpass.egg-info/PKG-INFO
--rw-rw-rw-   0 steven    (1000) steven    (1000)      448 2017-03-24 22:04:27.000000 xkcdpass-1.9.4/xkcdpass.egg-info/SOURCES.txt
--rw-rw-rw-   0 steven    (1000) steven    (1000)        1 2017-03-24 22:04:27.000000 xkcdpass-1.9.4/xkcdpass.egg-info/dependency_links.txt
--rw-rw-rw-   0 steven    (1000) steven    (1000)       58 2017-03-24 22:04:27.000000 xkcdpass-1.9.4/xkcdpass.egg-info/entry_points.txt
--rw-rw-rw-   0 steven    (1000) steven    (1000)        1 2016-09-04 16:19:52.000000 xkcdpass-1.9.4/xkcdpass.egg-info/not-zip-safe
--rw-rw-rw-   0 steven    (1000) steven    (1000)        9 2017-03-24 22:04:27.000000 xkcdpass-1.9.4/xkcdpass.egg-info/top_level.txt
+drwxr-xr-x   0 steventobin   (501) staff       (20)        0 2017-03-27 10:40:37.000000 xkcdpass-1.9.5/
+drwxr-xr-x   0 steventobin   (501) staff       (20)        0 2017-03-27 10:40:37.000000 xkcdpass-1.9.5/examples/
+-rw-r--r--   0 steventobin   (501) staff       (20)      464 2017-03-19 20:41:22.000000 xkcdpass-1.9.5/examples/example_import.py
+-rw-r--r--   0 steventobin   (501) staff       (20)      864 2017-03-19 20:41:22.000000 xkcdpass-1.9.5/examples/example_json.py
+-rwxr-xr-x   0 steventobin   (501) staff       (20)      689 2017-03-19 20:46:37.000000 xkcdpass-1.9.5/examples/example_postprocess.py
+-rw-r--r--   0 steventobin   (501) staff       (20)     1524 2017-03-19 20:41:22.000000 xkcdpass-1.9.5/LICENSE.BSD
+-rw-r--r--   0 steventobin   (501) staff       (20)      100 2017-03-19 20:41:22.000000 xkcdpass-1.9.5/MANIFEST.in
+-rw-r--r--   0 steventobin   (501) staff       (20)     9831 2017-03-27 10:40:37.000000 xkcdpass-1.9.5/PKG-INFO
+-rw-r--r--   0 steventobin   (501) staff       (20)     7531 2017-03-27 10:39:16.000000 xkcdpass-1.9.5/README.rst
+-rw-r--r--   0 steventobin   (501) staff       (20)       38 2017-03-27 10:40:37.000000 xkcdpass-1.9.5/setup.cfg
+-rw-r--r--   0 steventobin   (501) staff       (20)     1114 2017-03-27 10:38:43.000000 xkcdpass-1.9.5/setup.py
+drwxr-xr-x   0 steventobin   (501) staff       (20)        0 2017-03-27 10:40:37.000000 xkcdpass-1.9.5/tests/
+-rw-r--r--   0 steventobin   (501) staff       (20)       66 2017-03-19 20:41:22.000000 xkcdpass-1.9.5/tests/test_list.txt
+-rw-r--r--   0 steventobin   (501) staff       (20)     1530 2017-03-27 10:38:32.000000 xkcdpass-1.9.5/tests/xkcdp_tests.py
+drwxr-xr-x   0 steventobin   (501) staff       (20)        0 2017-03-27 10:40:37.000000 xkcdpass-1.9.5/xkcdpass/
+-rw-r--r--   0 steventobin   (501) staff       (20)        0 2017-03-19 20:41:22.000000 xkcdpass-1.9.5/xkcdpass/__init__.py
+drwxr-xr-x   0 steventobin   (501) staff       (20)        0 2017-03-27 10:40:37.000000 xkcdpass-1.9.5/xkcdpass/static/
+-rw-r--r--   0 steventobin   (501) staff       (20)   691880 2017-03-27 10:37:21.000000 xkcdpass-1.9.5/xkcdpass/static/default.txt
+-rwxr-xr-x   0 steventobin   (501) staff       (20)    12958 2017-03-19 20:41:22.000000 xkcdpass-1.9.5/xkcdpass/xkcd_password.py
+-rw-r--r--   0 steventobin   (501) staff       (20)     3293 2017-03-19 20:41:22.000000 xkcdpass-1.9.5/xkcdpass.1
+drwxr-xr-x   0 steventobin   (501) staff       (20)        0 2017-03-27 10:40:37.000000 xkcdpass-1.9.5/xkcdpass.egg-info/
+-rw-r--r--   0 steventobin   (501) staff       (20)        1 2017-03-27 10:40:36.000000 xkcdpass-1.9.5/xkcdpass.egg-info/dependency_links.txt
+-rw-r--r--   0 steventobin   (501) staff       (20)       58 2017-03-27 10:40:36.000000 xkcdpass-1.9.5/xkcdpass.egg-info/entry_points.txt
+-rw-r--r--   0 steventobin   (501) staff       (20)        1 2017-03-27 10:40:36.000000 xkcdpass-1.9.5/xkcdpass.egg-info/not-zip-safe
+-rw-r--r--   0 steventobin   (501) staff       (20)     9831 2017-03-27 10:40:36.000000 xkcdpass-1.9.5/xkcdpass.egg-info/PKG-INFO
+-rw-r--r--   0 steventobin   (501) staff       (20)      448 2017-03-27 10:40:37.000000 xkcdpass-1.9.5/xkcdpass.egg-info/SOURCES.txt
+-rw-r--r--   0 steventobin   (501) staff       (20)        9 2017-03-27 10:40:36.000000 xkcdpass-1.9.5/xkcdpass.egg-info/top_level.txt
```

### Comparing `xkcdpass-1.9.4/LICENSE.BSD` & `xkcdpass-1.9.5/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `xkcdpass-1.9.4/PKG-INFO` & `xkcdpass-1.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xkcdpass
-Version: 1.9.4
+Version: 1.9.5
 Summary: Generate secure multiword passwords/passphrases, inspired by XKCD
 Home-page: https://github.com/redacted/XKCD-password-generator
 Author: Steven Tobin
 Author-email: steventtobin@gmail.com
 License: BSD
 Description: xkcdpass
         ========
@@ -168,14 +168,15 @@
         While we recommend the standard word list for most purposes, we note that this list is uncensored and, as such, generated passwords could offend. For this reason, `a filtered word list can be found in the github repo <https://github.com/redacted/XKCD-password-generator/tree/master/contrib/office-safe.txt>`_ (filtered by Twig Nyugen and included here with permission).
         
         An important caveat: due to the significant reduction in the size of the filtered word list when compared to the default, the strength of the corresponding passwords is also reduced. Users should expect approximately an *order of magnitude* reduction in the strength of a five word passphrase. This can be mitigated by increasing the length of generated passphrases.
         
         
         Changelog
         =========
+        - **1.9.5** Fix broken test
         - **1.9.4** Improve office-safe wordlist contents
         - **1.9.3** Link EFF wordlist information, fix typos, update copyright
         - **1.9.2** Added Debian cracklib path
         - **1.9.1** Fixed typo in example
         - **1.9.0** Improvements to interactive mode
         - **1.8.2** `generate_wordlist` behaviour didn't match docstring, fixed
         - **1.8.1** Fix typo in validation function
```

### Comparing `xkcdpass-1.9.4/README.rst` & `xkcdpass-1.9.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,15 @@
 While we recommend the standard word list for most purposes, we note that this list is uncensored and, as such, generated passwords could offend. For this reason, `a filtered word list can be found in the github repo <https://github.com/redacted/XKCD-password-generator/tree/master/contrib/office-safe.txt>`_ (filtered by Twig Nyugen and included here with permission).
 
 An important caveat: due to the significant reduction in the size of the filtered word list when compared to the default, the strength of the corresponding passwords is also reduced. Users should expect approximately an *order of magnitude* reduction in the strength of a five word passphrase. This can be mitigated by increasing the length of generated passphrases.
 
 
 Changelog
 =========
+- **1.9.5** Fix broken test
 - **1.9.4** Improve office-safe wordlist contents
 - **1.9.3** Link EFF wordlist information, fix typos, update copyright
 - **1.9.2** Added Debian cracklib path
 - **1.9.1** Fixed typo in example
 - **1.9.0** Improvements to interactive mode
 - **1.8.2** `generate_wordlist` behaviour didn't match docstring, fixed
 - **1.8.1** Fix typo in validation function
```

### Comparing `xkcdpass-1.9.4/examples/example_json.py` & `xkcdpass-1.9.5/examples/example_json.py`

 * *Files identical despite different names*

### Comparing `xkcdpass-1.9.4/examples/example_postprocess.py` & `xkcdpass-1.9.5/examples/example_postprocess.py`

 * *Files identical despite different names*

### Comparing `xkcdpass-1.9.4/setup.py` & `xkcdpass-1.9.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='xkcdpass',
-    version='1.9.4',
+    version='1.9.5',
     author='Steven Tobin',
     author_email='steventtobin@gmail.com',
     url='https://github.com/redacted/XKCD-password-generator',
     description='Generate secure multiword passwords/passphrases, inspired by XKCD',
     long_description=open('README.rst').read(),
     packages=['xkcdpass'],
     zip_safe=False,
```

### Comparing `xkcdpass-1.9.4/tests/xkcdp_tests.py` & `xkcdpass-1.9.5/tests/xkcdp_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             min_length=5,
             max_length=8,)
         self.wordlist_small = xkcd_password.generate_wordlist(
             wordfile='tests/test_list.txt',
             valid_chars='[a-z]')
 
     def test_loadwordfile(self):
-        self.assertEquals(len(self.wordlist_full), 29612)
+        self.assertEquals(len(self.wordlist_full), 29611)
 
     def test_regex(self):
         self.assertNotIn("__$$$__", self.wordlist_small)
 
     def test_acrostic(self):
         word = "face"
         result = xkcd_password.generate_xkcdpassword(
```

### Comparing `xkcdpass-1.9.4/xkcdpass/static/default.txt` & `xkcdpass-1.9.5/xkcdpass/static/default.txt`

 * *Files identical despite different names*

### Comparing `xkcdpass-1.9.4/xkcdpass/xkcd_password.py` & `xkcdpass-1.9.5/xkcdpass/xkcd_password.py`

 * *Files identical despite different names*

### Comparing `xkcdpass-1.9.4/xkcdpass.1` & `xkcdpass-1.9.5/xkcdpass.1`

 * *Files identical despite different names*

### Comparing `xkcdpass-1.9.4/xkcdpass.egg-info/PKG-INFO` & `xkcdpass-1.9.5/xkcdpass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xkcdpass
-Version: 1.9.4
+Version: 1.9.5
 Summary: Generate secure multiword passwords/passphrases, inspired by XKCD
 Home-page: https://github.com/redacted/XKCD-password-generator
 Author: Steven Tobin
 Author-email: steventtobin@gmail.com
 License: BSD
 Description: xkcdpass
         ========
@@ -168,14 +168,15 @@
         While we recommend the standard word list for most purposes, we note that this list is uncensored and, as such, generated passwords could offend. For this reason, `a filtered word list can be found in the github repo <https://github.com/redacted/XKCD-password-generator/tree/master/contrib/office-safe.txt>`_ (filtered by Twig Nyugen and included here with permission).
         
         An important caveat: due to the significant reduction in the size of the filtered word list when compared to the default, the strength of the corresponding passwords is also reduced. Users should expect approximately an *order of magnitude* reduction in the strength of a five word passphrase. This can be mitigated by increasing the length of generated passphrases.
         
         
         Changelog
         =========
+        - **1.9.5** Fix broken test
         - **1.9.4** Improve office-safe wordlist contents
         - **1.9.3** Link EFF wordlist information, fix typos, update copyright
         - **1.9.2** Added Debian cracklib path
         - **1.9.1** Fixed typo in example
         - **1.9.0** Improvements to interactive mode
         - **1.8.2** `generate_wordlist` behaviour didn't match docstring, fixed
         - **1.8.1** Fix typo in validation function
```

