# Comparing `tmp/GenCasting-0.0.4.tar.gz` & `tmp/GenCasting-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenCasting-0.0.4.tar", last modified: Mon Apr  1 20:08:52 2024, max compression
+gzip compressed data, was "GenCasting-0.0.5.tar", last modified: Mon Apr  1 20:57:00 2024, max compression
```

## Comparing `GenCasting-0.0.4.tar` & `GenCasting-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 20:08:52.018873 GenCasting-0.0.4/
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 20:08:52.016709 GenCasting-0.0.4/GenCasting/
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       41 2024-04-01 20:07:30.000000 GenCasting-0.0.4/GenCasting/__init__.py
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     6781 2024-04-01 19:53:44.000000 GenCasting-0.0.4/GenCasting/logit_extraction.py
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 20:08:52.018070 GenCasting-0.0.4/GenCasting.egg-info/
--rw-r--r--   0 faf32    (50383) faf32    (50391)      579 2024-04-01 20:08:51.000000 GenCasting-0.0.4/GenCasting.egg-info/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)      249 2024-04-01 20:08:51.000000 GenCasting-0.0.4/GenCasting.egg-info/SOURCES.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-01 20:08:51.000000 GenCasting-0.0.4/GenCasting.egg-info/dependency_links.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       59 2024-04-01 20:08:51.000000 GenCasting-0.0.4/GenCasting.egg-info/requires.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       11 2024-04-01 20:08:51.000000 GenCasting-0.0.4/GenCasting.egg-info/top_level.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 GenCasting-0.0.4/LICENSE
--rw-r--r--   0 faf32    (50383) faf32    (50391)      579 2024-04-01 20:08:52.018452 GenCasting-0.0.4/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       37 2024-04-01 19:42:20.000000 GenCasting-0.0.4/README.md
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-01 20:08:52.018935 GenCasting-0.0.4/setup.cfg
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     1114 2024-04-01 20:08:22.000000 GenCasting-0.0.4/setup.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 20:57:00.097855 GenCasting-0.0.5/
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 20:57:00.095595 GenCasting-0.0.5/GenCasting/
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       41 2024-04-01 20:07:30.000000 GenCasting-0.0.5/GenCasting/__init__.py
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     6781 2024-04-01 19:53:44.000000 GenCasting-0.0.5/GenCasting/logit_extraction.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-01 20:57:00.096939 GenCasting-0.0.5/GenCasting.egg-info/
+-rw-r--r--   0 faf32    (50383) faf32    (50391)      598 2024-04-01 20:57:00.096014 GenCasting-0.0.5/GenCasting.egg-info/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)      249 2024-04-01 20:57:00.096252 GenCasting-0.0.5/GenCasting.egg-info/SOURCES.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-01 20:57:00.096465 GenCasting-0.0.5/GenCasting.egg-info/dependency_links.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-01 20:57:00.096673 GenCasting-0.0.5/GenCasting.egg-info/requires.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       11 2024-04-01 20:57:00.096993 GenCasting-0.0.5/GenCasting.egg-info/top_level.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 GenCasting-0.0.5/LICENSE
+-rw-r--r--   0 faf32    (50383) faf32    (50391)      598 2024-04-01 20:57:00.097366 GenCasting-0.0.5/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       37 2024-04-01 19:42:20.000000 GenCasting-0.0.5/README.md
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-01 20:57:00.097916 GenCasting-0.0.5/setup.cfg
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     1120 2024-04-01 20:56:39.000000 GenCasting-0.0.5/setup.py
```

### Comparing `GenCasting-0.0.4/GenCasting/logit_extraction.py` & `GenCasting-0.0.5/GenCasting/logit_extraction.py`

 * *Files identical despite different names*

### Comparing `GenCasting-0.0.4/GenCasting.egg-info/PKG-INFO` & `GenCasting-0.0.5/GenCasting.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: GenCasting
-Version: 0.0.4
+Version: 0.0.5
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bitsandbytes
 Requires-Dist: datasets
 Requires-Dist: accelerate
 Requires-Dist: loralib
 Requires-Dist: transformers
 Requires-Dist: peft
+Requires-Dist: trl
 
 
 ## GenCasting 
 
 
 Description to come.
```

### Comparing `GenCasting-0.0.4/PKG-INFO` & `GenCasting-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: GenCasting
-Version: 0.0.4
+Version: 0.0.5
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bitsandbytes
 Requires-Dist: datasets
 Requires-Dist: accelerate
 Requires-Dist: loralib
 Requires-Dist: transformers
 Requires-Dist: peft
+Requires-Dist: trl
 
 
 ## GenCasting 
 
 
 Description to come.
```

### Comparing `GenCasting-0.0.4/setup.py` & `GenCasting-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Extract token-level probabilities from LLMs for classification-type outputs.'
 LONG_DESCRIPTION = 'A package that allows one to extract token-level probabilities. This method can be used for example to extract sentiment class probabilities instead of parsing text-generation outputs.'
 
 # Setting up
 setup(
     name="GenCasting",
     version=VERSION,
     author="Francesco A. Fabozzi",
     author_email="francescoafabozzi@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['bitsandbytes', 'datasets', 'accelerate', 'loralib', 'transformers','peft'],
+    install_requires=['bitsandbytes', 'datasets', 'accelerate', 'loralib', 'transformers','peft','trl'],
     keywords=['python', 'LLMs', 'finance', 'forecasting', 'language models', 'huggingface'],
     classifiers=[
         "Development Status :: 1 - Planning"
     ]
 )
```

