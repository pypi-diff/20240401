# Comparing `tmp/pytubefix-3.1rc1.tar.gz` & `tmp/pytubefix-4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytubefix-3.1rc1.tar", last modified: Sun Mar 31 02:18:19 2024, max compression
+gzip compressed data, was "pytubefix-4.0rc1.tar", last modified: Mon Apr  1 11:25:37 2024, max compression
```

## Comparing `pytubefix-3.1rc1.tar` & `pytubefix-4.0rc1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-03-31 02:18:19.318516 pytubefix-3.1rc1/
--rw-rw-r--   0 juan      (1000) juan      (1000)     1101 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/LICENSE
--rw-rw-r--   0 juan      (1000) juan      (1000)       18 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/MANIFEST.in
--rw-r--r--   0 juan      (1000) juan      (1000)     4506 2024-03-31 02:18:19.314515 pytubefix-3.1rc1/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     3174 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/README.md
--rw-rw-r--   0 juan      (1000) juan      (1000)     1524 2024-03-31 02:16:43.000000 pytubefix-3.1rc1/pyproject.toml
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-03-31 02:18:19.310515 pytubefix-3.1rc1/pytubefix/
--rw-rw-r--   0 juan      (1000) juan      (1000)      614 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    17933 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/__main__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     6595 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/captions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1121 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/chapters.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    22543 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/cipher.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    17032 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/cli.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      786 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/colors.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-03-31 02:18:19.314515 pytubefix-3.1rc1/pytubefix/contrib/
--rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/contrib/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    19995 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/contrib/channel.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14600 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/contrib/playlist.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    11048 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/contrib/search.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     4115 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/exceptions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    18093 2024-03-31 02:13:47.000000 pytubefix-3.1rc1/pytubefix/extract.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     9944 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/helpers.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    16833 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/innertube.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     4311 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/itags.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1483 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/metadata.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      478 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/monostate.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5960 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/parser.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14289 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/query.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     8817 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/request.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14818 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/pytubefix/streams.py
--rw-rw-r--   0 juan      (1000) juan      (1000)       75 2024-03-31 02:17:00.000000 pytubefix-3.1rc1/pytubefix/version.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-03-31 02:18:19.314515 pytubefix-3.1rc1/pytubefix.egg-info/
--rw-r--r--   0 juan      (1000) juan      (1000)     4506 2024-03-31 02:18:19.000000 pytubefix-3.1rc1/pytubefix.egg-info/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     1007 2024-03-31 02:18:19.000000 pytubefix-3.1rc1/pytubefix.egg-info/SOURCES.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-03-31 02:18:19.000000 pytubefix-3.1rc1/pytubefix.egg-info/dependency_links.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       49 2024-03-31 02:18:19.000000 pytubefix-3.1rc1/pytubefix.egg-info/entry_points.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       10 2024-03-31 02:18:19.000000 pytubefix-3.1rc1/pytubefix.egg-info/top_level.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-03-31 02:18:19.318516 pytubefix-3.1rc1/setup.cfg
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-03-31 02:18:19.314515 pytubefix-3.1rc1/tests/
--rw-rw-r--   0 juan      (1000) juan      (1000)     6579 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/tests/test_captions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2742 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/tests/test_cipher.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    18009 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/tests/test_cli.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     3626 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/tests/test_exceptions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2963 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/tests/test_extract.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5060 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/tests/test_helpers.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      279 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/tests/test_itags.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1939 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/tests/test_main.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      501 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/tests/test_metadata.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1412 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/tests/test_parser.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     6172 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/tests/test_query.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1882 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/tests/test_request.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    13661 2024-03-31 02:08:58.000000 pytubefix-3.1rc1/tests/test_streams.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-01 11:25:37.693410 pytubefix-4.0rc1/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1101 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/LICENSE
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       18 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/MANIFEST.in
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     4506 2024-04-01 11:25:37.693410 pytubefix-4.0rc1/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     3174 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/README.md
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1524 2024-04-01 11:23:09.000000 pytubefix-4.0rc1/pyproject.toml
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-01 11:25:37.685410 pytubefix-4.0rc1/pytubefix/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      614 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/__init__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    17933 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/__main__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     6595 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/captions.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1121 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/chapters.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    22543 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/cipher.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    17032 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/cli.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      786 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/colors.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-01 11:25:37.685410 pytubefix-4.0rc1/pytubefix/contrib/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        0 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/contrib/__init__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    19995 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/contrib/channel.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    14600 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/contrib/playlist.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    11048 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/contrib/search.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     4115 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/exceptions.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    18093 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/extract.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     9944 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/helpers.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    16837 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/innertube.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     4311 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/itags.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1483 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/metadata.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      478 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/monostate.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     5960 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/parser.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    14289 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/query.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     8817 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/request.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    14818 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/pytubefix/streams.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-04-01 11:23:15.000000 pytubefix-4.0rc1/pytubefix/version.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-01 11:25:37.689410 pytubefix-4.0rc1/pytubefix.egg-info/
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     4506 2024-04-01 11:25:37.000000 pytubefix-4.0rc1/pytubefix.egg-info/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1007 2024-04-01 11:25:37.000000 pytubefix-4.0rc1/pytubefix.egg-info/SOURCES.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-04-01 11:25:37.000000 pytubefix-4.0rc1/pytubefix.egg-info/dependency_links.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       49 2024-04-01 11:25:37.000000 pytubefix-4.0rc1/pytubefix.egg-info/entry_points.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       10 2024-04-01 11:25:37.000000 pytubefix-4.0rc1/pytubefix.egg-info/top_level.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-04-01 11:25:37.693410 pytubefix-4.0rc1/setup.cfg
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-01 11:25:37.689410 pytubefix-4.0rc1/tests/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     6579 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/tests/test_captions.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2742 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/tests/test_cipher.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    18009 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/tests/test_cli.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     3626 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/tests/test_exceptions.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2963 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/tests/test_extract.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     5060 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/tests/test_helpers.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      279 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/tests/test_itags.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1939 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/tests/test_main.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      501 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/tests/test_metadata.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1412 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/tests/test_parser.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     6172 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/tests/test_query.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1882 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/tests/test_request.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    13661 2024-04-01 11:17:12.000000 pytubefix-4.0rc1/tests/test_streams.py
```

### Comparing `pytubefix-3.1rc1/LICENSE` & `pytubefix-4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/PKG-INFO` & `pytubefix-4.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 3.1rc1
+Version: 4.0rc1
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 3.1rc1 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 4.0rc1 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytubefix-3.1rc1/README.md` & `pytubefix-4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pyproject.toml` & `pytubefix-4.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytubefix"
-version = "3.1-rc1"
+version = "4.0-rc1"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python3 library for downloading YouTube Videos."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT license"}
```

### Comparing `pytubefix-3.1rc1/pytubefix/__init__.py` & `pytubefix-4.0rc1/pytubefix/__init__.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/__main__.py` & `pytubefix-4.0rc1/pytubefix/__main__.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/captions.py` & `pytubefix-4.0rc1/pytubefix/captions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/chapters.py` & `pytubefix-4.0rc1/pytubefix/chapters.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/cipher.py` & `pytubefix-4.0rc1/pytubefix/cipher.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/cli.py` & `pytubefix-4.0rc1/pytubefix/cli.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/colors.py` & `pytubefix-4.0rc1/pytubefix/colors.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/contrib/channel.py` & `pytubefix-4.0rc1/pytubefix/contrib/channel.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/contrib/playlist.py` & `pytubefix-4.0rc1/pytubefix/contrib/playlist.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/contrib/search.py` & `pytubefix-4.0rc1/pytubefix/contrib/search.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/exceptions.py` & `pytubefix-4.0rc1/pytubefix/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/extract.py` & `pytubefix-4.0rc1/pytubefix/extract.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/helpers.py` & `pytubefix-4.0rc1/pytubefix/helpers.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/innertube.py` & `pytubefix-4.0rc1/pytubefix/innertube.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             'context': {
                 'client': {
                     'clientName': 'ANDROID',
                     'clientVersion': '19.08.35',
                     'androidSdkVersion': 30
                 }
             },
-            "params": "CgIQBg"
+            "params": "CgIIAdgDAQ%3D%3D"
         },
         'header': {
             'User-Agent': 'com.google.android.youtube/',
         },
         'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8'
     },
     'IOS': {
@@ -245,15 +245,15 @@
 _token_timeout = 1800
 _cache_dir = pathlib.Path(__file__).parent.resolve() / '__cache__'
 _token_file = os.path.join(_cache_dir, 'tokens.json')
 
 
 class InnerTube:
     """Object for interacting with the innertube API."""
-    def __init__(self, client='ANDROID_MUSIC', use_oauth=False, allow_cache=True):
+    def __init__(self, client='ANDROID', use_oauth=False, allow_cache=True):
         """Initialize an InnerTube object.
 
         :param str client:
             Client to use for the object.
             The default is ANDROID because there is no need to decrypt the
             signature cipher and throttling parameter.
         :param bool use_oauth:
```

### Comparing `pytubefix-3.1rc1/pytubefix/itags.py` & `pytubefix-4.0rc1/pytubefix/itags.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/metadata.py` & `pytubefix-4.0rc1/pytubefix/metadata.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/parser.py` & `pytubefix-4.0rc1/pytubefix/parser.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/query.py` & `pytubefix-4.0rc1/pytubefix/query.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/request.py` & `pytubefix-4.0rc1/pytubefix/request.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix/streams.py` & `pytubefix-4.0rc1/pytubefix/streams.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/pytubefix.egg-info/PKG-INFO` & `pytubefix-4.0rc1/pytubefix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 3.1rc1
+Version: 4.0rc1
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 3.1rc1 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 4.0rc1 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytubefix-3.1rc1/pytubefix.egg-info/SOURCES.txt` & `pytubefix-4.0rc1/pytubefix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/tests/test_captions.py` & `pytubefix-4.0rc1/tests/test_captions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/tests/test_cipher.py` & `pytubefix-4.0rc1/tests/test_cipher.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/tests/test_cli.py` & `pytubefix-4.0rc1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/tests/test_exceptions.py` & `pytubefix-4.0rc1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/tests/test_extract.py` & `pytubefix-4.0rc1/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/tests/test_helpers.py` & `pytubefix-4.0rc1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/tests/test_main.py` & `pytubefix-4.0rc1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/tests/test_parser.py` & `pytubefix-4.0rc1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/tests/test_query.py` & `pytubefix-4.0rc1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/tests/test_request.py` & `pytubefix-4.0rc1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `pytubefix-3.1rc1/tests/test_streams.py` & `pytubefix-4.0rc1/tests/test_streams.py`

 * *Files identical despite different names*

