# Comparing `tmp/qa_metrics-0.1.8.tar.gz` & `tmp/qa_metrics-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qa_metrics-0.1.8.tar", last modified: Sun Jan 21 17:03:38 2024, max compression
+gzip compressed data, was "qa_metrics-0.1.9.tar", last modified: Sun Jan 21 18:27:47 2024, max compression
```

## Comparing `qa_metrics-0.1.8.tar` & `qa_metrics-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-01-21 17:03:38.619607 qa_metrics-0.1.8/
--rw-r--r--   0 zongxiali   (501) staff       (20)     1071 2024-01-21 05:47:39.000000 qa_metrics-0.1.8/LICENSE
--rw-r--r--   0 zongxiali   (501) staff       (20)       69 2024-01-21 16:07:24.000000 qa_metrics-0.1.8/MANIFEST.in
--rw-r--r--   0 zongxiali   (501) staff       (20)      949 2024-01-21 17:03:38.619151 qa_metrics-0.1.8/PKG-INFO
--rw-r--r--   0 zongxiali   (501) staff       (20)        0 2024-01-20 16:46:16.000000 qa_metrics-0.1.8/README.md
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-01-21 17:03:38.610907 qa_metrics-0.1.8/qa_metrics/
--rw-r--r--   0 zongxiali   (501) staff       (20)     2514 2024-01-21 17:03:24.000000 qa_metrics-0.1.8/qa_metrics/__init__.py
--rw-r--r--   0 zongxiali   (501) staff       (20)       53 2024-01-21 05:42:31.000000 qa_metrics-0.1.8/qa_metrics/bem.py
--rw-r--r--   0 zongxiali   (501) staff       (20)    12329 2024-01-21 17:01:52.000000 qa_metrics-0.1.8/qa_metrics/cfm.py
--rw-r--r--   0 zongxiali   (501) staff       (20)      995 2024-01-21 06:57:51.000000 qa_metrics-0.1.8/qa_metrics/em.py
--rw-r--r--   0 zongxiali   (501) staff       (20)     2449 2024-01-21 06:57:53.000000 qa_metrics-0.1.8/qa_metrics/f1.py
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-01-21 17:03:38.617491 qa_metrics-0.1.8/qa_metrics/utils/
--rw-r--r--   0 zongxiali   (501) staff       (20)        0 2024-01-21 06:58:23.000000 qa_metrics-0.1.8/qa_metrics/utils/__init__.py
--rw-r--r--   0 zongxiali   (501) staff       (20)      680 2024-01-21 16:35:36.000000 qa_metrics-0.1.8/qa_metrics/utils/tools.py
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-01-21 17:03:38.618625 qa_metrics-0.1.8/qa_metrics.egg-info/
--rw-r--r--   0 zongxiali   (501) staff       (20)      949 2024-01-21 17:03:38.000000 qa_metrics-0.1.8/qa_metrics.egg-info/PKG-INFO
--rw-r--r--   0 zongxiali   (501) staff       (20)      355 2024-01-21 17:03:38.000000 qa_metrics-0.1.8/qa_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)        1 2024-01-21 17:03:38.000000 qa_metrics-0.1.8/qa_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)       83 2024-01-21 17:03:38.000000 qa_metrics-0.1.8/qa_metrics.egg-info/requires.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)       11 2024-01-21 17:03:38.000000 qa_metrics-0.1.8/qa_metrics.egg-info/top_level.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)       38 2024-01-21 17:03:38.619711 qa_metrics-0.1.8/setup.cfg
--rw-r--r--   0 zongxiali   (501) staff       (20)     1281 2024-01-21 17:03:35.000000 qa_metrics-0.1.8/setup.py
+drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-01-21 18:27:47.498692 qa_metrics-0.1.9/
+-rw-r--r--   0 zongxiali   (501) staff       (20)     1071 2024-01-21 05:47:39.000000 qa_metrics-0.1.9/LICENSE
+-rw-r--r--   0 zongxiali   (501) staff       (20)       69 2024-01-21 16:07:24.000000 qa_metrics-0.1.9/MANIFEST.in
+-rw-r--r--   0 zongxiali   (501) staff       (20)      949 2024-01-21 18:27:47.497756 qa_metrics-0.1.9/PKG-INFO
+-rw-r--r--   0 zongxiali   (501) staff       (20)        0 2024-01-20 16:46:16.000000 qa_metrics-0.1.9/README.md
+drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-01-21 18:27:47.490463 qa_metrics-0.1.9/qa_metrics/
+-rw-r--r--   0 zongxiali   (501) staff       (20)     2731 2024-01-21 18:14:55.000000 qa_metrics-0.1.9/qa_metrics/__init__.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)    12329 2024-01-21 17:01:52.000000 qa_metrics-0.1.9/qa_metrics/cfm.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)      995 2024-01-21 06:57:51.000000 qa_metrics-0.1.9/qa_metrics/em.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)     2449 2024-01-21 06:57:53.000000 qa_metrics-0.1.9/qa_metrics/f1.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)     2448 2024-01-21 18:25:45.000000 qa_metrics-0.1.9/qa_metrics/transformerMatcher.py
+drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-01-21 18:27:47.495172 qa_metrics-0.1.9/qa_metrics/utils/
+-rw-r--r--   0 zongxiali   (501) staff       (20)        0 2024-01-21 06:58:23.000000 qa_metrics-0.1.9/qa_metrics/utils/__init__.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)      680 2024-01-21 16:35:36.000000 qa_metrics-0.1.9/qa_metrics/utils/tools.py
+drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-01-21 18:27:47.496738 qa_metrics-0.1.9/qa_metrics.egg-info/
+-rw-r--r--   0 zongxiali   (501) staff       (20)      949 2024-01-21 18:27:47.000000 qa_metrics-0.1.9/qa_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 zongxiali   (501) staff       (20)      370 2024-01-21 18:27:47.000000 qa_metrics-0.1.9/qa_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 zongxiali   (501) staff       (20)        1 2024-01-21 18:27:47.000000 qa_metrics-0.1.9/qa_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 zongxiali   (501) staff       (20)       83 2024-01-21 18:27:47.000000 qa_metrics-0.1.9/qa_metrics.egg-info/requires.txt
+-rw-r--r--   0 zongxiali   (501) staff       (20)       11 2024-01-21 18:27:47.000000 qa_metrics-0.1.9/qa_metrics.egg-info/top_level.txt
+-rw-r--r--   0 zongxiali   (501) staff       (20)       38 2024-01-21 18:27:47.498904 qa_metrics-0.1.9/setup.cfg
+-rw-r--r--   0 zongxiali   (501) staff       (20)     1281 2024-01-21 17:34:07.000000 qa_metrics-0.1.9/setup.py
```

### Comparing `qa_metrics-0.1.8/LICENSE` & `qa_metrics-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.1.8/PKG-INFO` & `qa_metrics-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qa_metrics
-Version: 0.1.8
+Version: 0.1.9
 Summary: This package provides standard and classifier-based short form QA evaluation methods
 Home-page: https://github.com/zli12321/qa_metrics
 Author: Zongxia Li
 Author-email: zli12321@umd.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `qa_metrics-0.1.8/qa_metrics/__init__.py` & `qa_metrics-0.1.9/qa_metrics/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,53 @@
 import requests
 import os
 
 def download(model_name):
-    if model_name.lower() == 'bert':
-        # Download BERT model
-        url = 'https://drive.google.com/file/d/1ena_zUd42ju_5R3wKBidKdKuJYmF-IE_/view?usp=sharing'
-        model_dir = os.path.join(os.path.dirname(__file__), 'transformer_models')
-        model_path = os.path.join(model_dir, 'ae_tuned_bert.bin')
-
-        if not os.path.exists(model_dir):
-            os.makedirs(model_dir)
-
-        if not os.path.isfile(model_path):
-            print("Downloading BERT Matching model...")
+    def download_link(file, url, name):
+        if not os.path.isfile(file):
+            print("Downloading {}...".format(name))
             response = requests.get(url, stream=True)
 
             if response.status_code == 200:
-                with open(model_path, 'wb') as f:
+                with open(file, 'wb') as f:
                     f.write(response.content)
-                print("Download complete.")
+                print("Download {} complete.".format(name))
             else:
                 print("Failed to download the model. Status code:", response.status_code)
-        # else:
-        #     print("BERT model already exists.")
 
-        return model_path
+    if model_name.lower() == 'bert':
+        # Download BERT model
+        model_url = 'https://drive.google.com/file/d/1ena_zUd42ju_5R3wKBidKdKuJYmF-IE_/view?usp=sharing'
+        tokenizer_url = 'https://drive.google.com/file/d/1gpmCgHKX-zLpShDr-kDrotS0Fk6F8Ht1/view?usp=sharing'
+        tokenizer_config_url = 'https://drive.google.com/file/d/1kxMwo9dD-gzgDuZMZAP64GmD_KLTofUh/view?usp=sharing'
+        config_url = 'https://drive.google.com/file/d/14d3X6BbrDrKYlnwOYBDlW7_sjK5u2Msw/view?usp=sharing'
+        vocab_url = 'https://drive.google.com/file/d/1N_kiKtJFvsIv8cwb-6ZOwXpqOi6ZLEEl/view?usp=sharing'
+
+        model_dir = os.path.join(os.path.dirname(__file__), 'transformer_models/bert')
+        model_path = os.path.join(model_dir, 'ae_tuned_bert.bin')
+        tokenizer_path = os.path.join(model_dir, 'tokenizer.json')
+        tokenizer_config_path = os.path.join(model_dir, 'tokenizer_config.json')
+        config_path = os.path.join(model_dir, 'config.json')
+        vocab_path = os.path.join(model_dir, 'vocab.txt')
+
+        if not os.path.exists(model_dir):
+            os.makedirs(model_dir)
+
+        download_link(model_path, model_url, 'Fine-tuned BERT model')
+        download_link(tokenizer_path, tokenizer_url, 'BERT tokenizer')
+        download_link(tokenizer_config_path, tokenizer_config_url, 'BERT tokenizer config')
+        download_link(config_path, config_url, 'BERT config')
+        download_link(vocab_path, vocab_url, 'BERT vocab')        
+        
+        
     if model_name.lower() == 'cfm':
         clf_url = 'https://github.com/zli12321/qa_metrics/raw/master/qa_metrics/classifier/lr_classifier'
         vectorizer_url = 'https://github.com/zli12321/qa_metrics/raw/master/qa_metrics/classifier/tf-idf_vectorizer'
         model_dir = os.path.join(os.path.dirname(__file__), 'classifier')
         model_path = os.path.join(model_dir, 'lr_classifier.pkl')
         vectorizer_path = os.path.join(model_dir, 'tf-idf_vectorizer.pkl')
 
         if not os.path.exists(model_dir):
             os.makedirs(model_dir)
 
-        if not os.path.isfile(model_path):
-            print("Downloading CF Matching model...")
-            response = requests.get(clf_url, stream=True)
-            if response.status_code == 200:
-                with open(model_path, 'wb') as f:
-                    f.write(response.content)
-                print("Download clf model complete.")
-            else:
-                print("Failed to download the model. Status code:", response.status_code)
-
-        if not os.path.isfile(vectorizer_path):
-            print("Downloading CF Matching model tokenizer...")
-            response_tokenizer = requests.get(vectorizer_url, stream=True)
-            if response_tokenizer.status_code == 200:
-                with open(vectorizer_path, 'wb') as f:
-                    f.write(response_tokenizer.content)
-                print("Download clf tokzenizer complete.")
-            else:
-                print("Failed to download the model. Status code:", response.status_code)
+        download_link(model_path, clf_url, 'CF Matching model')
+        download_link(vectorizer_path, vectorizer_url, 'CF Matching model tokenizer')
```

### Comparing `qa_metrics-0.1.8/qa_metrics/cfm.py` & `qa_metrics-0.1.9/qa_metrics/cfm.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.1.8/qa_metrics/em.py` & `qa_metrics-0.1.9/qa_metrics/em.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.1.8/qa_metrics/f1.py` & `qa_metrics-0.1.9/qa_metrics/f1.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.1.8/qa_metrics/utils/tools.py` & `qa_metrics-0.1.9/qa_metrics/utils/tools.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.1.8/qa_metrics.egg-info/PKG-INFO` & `qa_metrics-0.1.9/qa_metrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qa_metrics
-Version: 0.1.8
+Version: 0.1.9
 Summary: This package provides standard and classifier-based short form QA evaluation methods
 Home-page: https://github.com/zli12321/qa_metrics
 Author: Zongxia Li
 Author-email: zli12321@umd.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `qa_metrics-0.1.8/setup.py` & `qa_metrics-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 import os
 
 
 setup(
     name='qa_metrics',
-    version='0.1.8',
+    version='0.1.9',
     author='Zongxia Li',
     author_email='zli12321@umd.edu',
     description='This package provides standard and classifier-based short form QA evaluation methods',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/zli12321/qa_metrics',
     packages=find_packages(),
```

