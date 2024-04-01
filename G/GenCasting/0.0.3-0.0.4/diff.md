# Comparing `tmp/GenCasting-0.0.3.tar.gz` & `tmp/GenCasting-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenCasting-0.0.3.tar", last modified: Mon Apr  1 20:03:28 2024, max compression
+gzip compressed data, was "GenCasting-0.0.4.tar", last modified: Mon Apr  1 20:08:52 2024, max compression
```

## Comparing `GenCasting-0.0.3.tar` & `GenCasting-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 20:03:28.544401 GenCasting-0.0.3/
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 20:03:28.541973 GenCasting-0.0.3/GenCasting/
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-01 20:00:34.000000 GenCasting-0.0.3/GenCasting/__init__.py
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     6781 2024-04-01 19:53:44.000000 GenCasting-0.0.3/GenCasting/logit_extraction.py
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 20:03:28.543437 GenCasting-0.0.3/GenCasting.egg-info/
--rw-r--r--   0 faf32    (50383) faf32    (50391)      579 2024-04-01 20:03:28.542405 GenCasting-0.0.3/GenCasting.egg-info/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)      249 2024-04-01 20:03:28.542689 GenCasting-0.0.3/GenCasting.egg-info/SOURCES.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-01 20:03:28.542922 GenCasting-0.0.3/GenCasting.egg-info/dependency_links.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       59 2024-04-01 20:03:28.543166 GenCasting-0.0.3/GenCasting.egg-info/requires.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       11 2024-04-01 20:03:28.543494 GenCasting-0.0.3/GenCasting.egg-info/top_level.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 GenCasting-0.0.3/LICENSE
--rw-r--r--   0 faf32    (50383) faf32    (50391)      579 2024-04-01 20:03:28.543883 GenCasting-0.0.3/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       37 2024-04-01 19:42:20.000000 GenCasting-0.0.3/README.md
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-01 20:03:28.544472 GenCasting-0.0.3/setup.cfg
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     1114 2024-04-01 20:03:12.000000 GenCasting-0.0.3/setup.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 20:08:52.018873 GenCasting-0.0.4/
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 20:08:52.016709 GenCasting-0.0.4/GenCasting/
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       41 2024-04-01 20:07:30.000000 GenCasting-0.0.4/GenCasting/__init__.py
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     6781 2024-04-01 19:53:44.000000 GenCasting-0.0.4/GenCasting/logit_extraction.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 20:08:52.018070 GenCasting-0.0.4/GenCasting.egg-info/
+-rw-r--r--   0 faf32    (50383) faf32    (50391)      579 2024-04-01 20:08:51.000000 GenCasting-0.0.4/GenCasting.egg-info/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)      249 2024-04-01 20:08:51.000000 GenCasting-0.0.4/GenCasting.egg-info/SOURCES.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-01 20:08:51.000000 GenCasting-0.0.4/GenCasting.egg-info/dependency_links.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       59 2024-04-01 20:08:51.000000 GenCasting-0.0.4/GenCasting.egg-info/requires.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       11 2024-04-01 20:08:51.000000 GenCasting-0.0.4/GenCasting.egg-info/top_level.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 GenCasting-0.0.4/LICENSE
+-rw-r--r--   0 faf32    (50383) faf32    (50391)      579 2024-04-01 20:08:52.018452 GenCasting-0.0.4/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       37 2024-04-01 19:42:20.000000 GenCasting-0.0.4/README.md
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-01 20:08:52.018935 GenCasting-0.0.4/setup.cfg
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     1114 2024-04-01 20:08:22.000000 GenCasting-0.0.4/setup.py
```

### Comparing `GenCasting-0.0.3/GenCasting/logit_extraction.py` & `GenCasting-0.0.4/GenCasting/logit_extraction.py`

 * *Files identical despite different names*

### Comparing `GenCasting-0.0.3/GenCasting.egg-info/PKG-INFO` & `GenCasting-0.0.4/GenCasting.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenCasting
-Version: 0.0.3
+Version: 0.0.4
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `GenCasting-0.0.3/PKG-INFO` & `GenCasting-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenCasting
-Version: 0.0.3
+Version: 0.0.4
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `GenCasting-0.0.3/setup.py` & `GenCasting-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Extract token-level probabilities from LLMs for classification-type outputs.'
 LONG_DESCRIPTION = 'A package that allows one to extract token-level probabilities. This method can be used for example to extract sentiment class probabilities instead of parsing text-generation outputs.'
 
 # Setting up
 setup(
     name="GenCasting",
     version=VERSION,
```

