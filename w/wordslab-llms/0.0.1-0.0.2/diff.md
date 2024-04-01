# Comparing `tmp/wordslab_llms-0.0.1.tar.gz` & `tmp/wordslab_llms-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordslab_llms-0.0.1.tar", last modified: Fri Feb 16 22:29:54 2024, max compression
+gzip compressed data, was "wordslab_llms-0.0.2.tar", last modified: Mon Apr  1 16:50:32 2024, max compression
```

## Comparing `wordslab_llms-0.0.1.tar` & `wordslab_llms-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 22:29:54.255202 wordslab_llms-0.0.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-02-11 09:01:31.000000 wordslab_llms-0.0.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      111 2023-04-27 10:12:58.000000 wordslab_llms-0.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1113 2024-02-16 22:29:54.255202 wordslab_llms-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      305 2024-02-16 21:59:04.000000 wordslab_llms-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1086 2024-02-11 11:42:15.000000 wordslab_llms-0.0.1/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-16 22:29:54.255202 wordslab_llms-0.0.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2596 2023-04-27 10:12:58.000000 wordslab_llms-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 22:29:54.255202 wordslab_llms-0.0.1/wordslab_llms/
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-16 21:59:03.000000 wordslab_llms-0.0.1/wordslab_llms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-02-16 21:59:03.000000 wordslab_llms-0.0.1/wordslab_llms/_modidx.py
--rw-r--r--   0 root         (0) root         (0)      173 2024-02-16 21:59:03.000000 wordslab_llms-0.0.1/wordslab_llms/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 22:29:54.255202 wordslab_llms-0.0.1/wordslab_llms.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1113 2024-02-16 22:29:54.000000 wordslab_llms-0.0.1/wordslab_llms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      386 2024-02-16 22:29:54.000000 wordslab_llms-0.0.1/wordslab_llms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-16 22:29:54.000000 wordslab_llms-0.0.1/wordslab_llms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-02-16 22:29:54.000000 wordslab_llms-0.0.1/wordslab_llms.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-16 21:14:54.000000 wordslab_llms-0.0.1/wordslab_llms.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        7 2024-02-16 22:29:54.000000 wordslab_llms-0.0.1/wordslab_llms.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-02-16 22:29:54.000000 wordslab_llms-0.0.1/wordslab_llms.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 16:50:32.025281 wordslab_llms-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-02-11 09:01:31.000000 wordslab_llms-0.0.2/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      111 2023-04-27 10:12:58.000000 wordslab_llms-0.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1211 2024-04-01 16:50:32.025281 wordslab_llms-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      403 2024-04-01 16:28:17.000000 wordslab_llms-0.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      949 2024-04-01 16:49:53.000000 wordslab_llms-0.0.2/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-01 16:50:32.025281 wordslab_llms-0.0.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2596 2023-04-27 10:12:58.000000 wordslab_llms-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 16:50:32.015281 wordslab_llms-0.0.2/wordslab_llms/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-01 16:50:06.000000 wordslab_llms-0.0.2/wordslab_llms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-01 16:50:06.000000 wordslab_llms-0.0.2/wordslab_llms/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)     8337 2024-04-01 16:50:06.000000 wordslab_llms-0.0.2/wordslab_llms/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 16:50:32.015281 wordslab_llms-0.0.2/wordslab_llms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1211 2024-04-01 16:50:32.000000 wordslab_llms-0.0.2/wordslab_llms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      386 2024-04-01 16:50:32.000000 wordslab_llms-0.0.2/wordslab_llms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 16:50:32.000000 wordslab_llms-0.0.2/wordslab_llms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-01 16:50:32.000000 wordslab_llms-0.0.2/wordslab_llms.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-16 21:14:54.000000 wordslab_llms-0.0.2/wordslab_llms.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-01 16:50:32.000000 wordslab_llms-0.0.2/wordslab_llms.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-01 16:50:32.000000 wordslab_llms-0.0.2/wordslab_llms.egg-info/top_level.txt
```

### Comparing `wordslab_llms-0.0.1/LICENSE` & `wordslab_llms-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wordslab_llms-0.0.1/PKG-INFO` & `wordslab_llms-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordslab_llms
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library for easy and efficient inference and fine tuning of popular open source llms
 Home-page: https://github.com/wordslab-org/wordslab-llms-lib
 Author: Laurent Prud'hon
 Author-email: laurent.prudhon@hotmail.fr
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python llm huggingface transformers
 Platform: UNKNOWN
@@ -34,13 +34,13 @@
 ```
 
 ## How to use
 
 Check if the library is installed:
 
 ``` python
-test()
+base_models['mistral_7b']
 ```
 
-    wordslab_llms models
+    mistral_7b: mistralai/Mistral-7B-v0.1 => params: 7.3 B | disk: 13.49 GB | vram: 14.324 GB (16 bits)
```

### Comparing `wordslab_llms-0.0.1/setup.py` & `wordslab_llms-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `wordslab_llms-0.0.1/wordslab_llms.egg-info/PKG-INFO` & `wordslab_llms-0.0.2/wordslab_llms.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordslab-llms
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library for easy and efficient inference and fine tuning of popular open source llms
 Home-page: https://github.com/wordslab-org/wordslab-llms-lib
 Author: Laurent Prud'hon
 Author-email: laurent.prudhon@hotmail.fr
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python llm huggingface transformers
 Platform: UNKNOWN
@@ -34,13 +34,13 @@
 ```
 
 ## How to use
 
 Check if the library is installed:
 
 ``` python
-test()
+base_models['mistral_7b']
 ```
 
-    wordslab_llms models
+    mistral_7b: mistralai/Mistral-7B-v0.1 => params: 7.3 B | disk: 13.49 GB | vram: 14.324 GB (16 bits)
```

