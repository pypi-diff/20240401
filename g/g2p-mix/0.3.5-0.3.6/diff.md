# Comparing `tmp/g2p_mix-0.3.5.tar.gz` & `tmp/g2p_mix-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2p_mix-0.3.5.tar", last modified: Fri Mar 29 02:46:54 2024, max compression
+gzip compressed data, was "g2p_mix-0.3.6.tar", last modified: Mon Apr  1 12:42:37 2024, max compression
```

## Comparing `g2p_mix-0.3.5.tar` & `g2p_mix-0.3.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-29 02:46:54.263921 g2p_mix-0.3.5/
--rw-r--r--   0 admin      (501) staff       (20)     1066 2024-03-28 03:45:18.000000 g2p_mix-0.3.5/LICENSE
--rw-r--r--   0 admin      (501) staff       (20)       67 2024-03-29 02:45:49.000000 g2p_mix-0.3.5/MANIFEST.in
--rw-r--r--   0 admin      (501) staff       (20)     1378 2024-03-29 02:46:54.263670 g2p_mix-0.3.5/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      775 2024-03-28 03:45:18.000000 g2p_mix-0.3.5/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-29 02:46:54.256299 g2p_mix-0.3.5/g2p_mix/
--rw-r--r--   0 admin      (501) staff       (20)      630 2024-03-28 03:45:18.000000 g2p_mix-0.3.5/g2p_mix/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     3147 2024-03-28 03:45:18.000000 g2p_mix-0.3.5/g2p_mix/constants.py
--rw-r--r--   0 admin      (501) staff       (20)     2455 2024-03-28 03:45:18.000000 g2p_mix-0.3.5/g2p_mix/g2p_eng.py
--rw-r--r--   0 admin      (501) staff       (20)     4433 2024-03-29 02:00:07.000000 g2p_mix-0.3.5/g2p_mix/g2p_mix.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-29 02:46:54.253333 g2p_mix-0.3.5/g2p_mix/nltk_data/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-29 02:46:54.257615 g2p_mix-0.3.5/g2p_mix/nltk_data/corpora/
--rw-r--r--   0 admin      (501) staff       (20)   896069 2024-03-28 03:45:18.000000 g2p_mix-0.3.5/g2p_mix/nltk_data/corpora/cmudict.zip
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-29 02:46:54.259733 g2p_mix-0.3.5/g2p_mix/nltk_data/taggers/
--rw-r--r--   0 admin      (501) staff       (20)  2526731 2024-03-28 03:45:18.000000 g2p_mix-0.3.5/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip
--rw-r--r--   0 admin      (501) staff       (20)     2047 2024-03-28 03:45:18.000000 g2p_mix-0.3.5/g2p_mix/token.py
--rw-r--r--   0 admin      (501) staff       (20)    11066 2024-03-28 03:45:18.000000 g2p_mix-0.3.5/g2p_mix/tone_sandhi.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-29 02:46:54.257461 g2p_mix-0.3.5/g2p_mix.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     1378 2024-03-29 02:46:54.000000 g2p_mix-0.3.5/g2p_mix.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      423 2024-03-29 02:46:54.000000 g2p_mix-0.3.5/g2p_mix.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2024-03-29 02:46:54.000000 g2p_mix-0.3.5/g2p_mix.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       87 2024-03-29 02:46:54.000000 g2p_mix-0.3.5/g2p_mix.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        8 2024-03-29 02:46:54.000000 g2p_mix-0.3.5/g2p_mix.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       48 2024-03-29 02:28:25.000000 g2p_mix-0.3.5/requirements.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2024-03-29 02:46:54.263975 g2p_mix-0.3.5/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1434 2024-03-29 02:46:26.000000 g2p_mix-0.3.5/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-01 12:42:37.872111 g2p_mix-0.3.6/
+-rw-r--r--   0 admin      (501) staff       (20)     1066 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/LICENSE
+-rw-r--r--   0 admin      (501) staff       (20)       67 2024-03-29 02:45:49.000000 g2p_mix-0.3.6/MANIFEST.in
+-rw-r--r--   0 admin      (501) staff       (20)     1378 2024-04-01 12:42:37.871883 g2p_mix-0.3.6/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      775 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-01 12:42:37.866469 g2p_mix-0.3.6/g2p_mix/
+-rw-r--r--   0 admin      (501) staff       (20)      630 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/g2p_mix/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     3147 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/g2p_mix/constants.py
+-rw-r--r--   0 admin      (501) staff       (20)     2455 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/g2p_mix/g2p_eng.py
+-rw-r--r--   0 admin      (501) staff       (20)     4433 2024-03-29 02:00:07.000000 g2p_mix-0.3.6/g2p_mix/g2p_mix.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-01 12:42:37.864655 g2p_mix-0.3.6/g2p_mix/nltk_data/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-01 12:42:37.867545 g2p_mix-0.3.6/g2p_mix/nltk_data/corpora/
+-rw-r--r--   0 admin      (501) staff       (20)   896069 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/g2p_mix/nltk_data/corpora/cmudict.zip
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-01 12:42:37.868854 g2p_mix-0.3.6/g2p_mix/nltk_data/taggers/
+-rw-r--r--   0 admin      (501) staff       (20)  2526731 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip
+-rw-r--r--   0 admin      (501) staff       (20)     2047 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/g2p_mix/token.py
+-rw-r--r--   0 admin      (501) staff       (20)    11066 2024-03-28 03:45:18.000000 g2p_mix-0.3.6/g2p_mix/tone_sandhi.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-01 12:42:37.867389 g2p_mix-0.3.6/g2p_mix.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     1378 2024-04-01 12:42:37.000000 g2p_mix-0.3.6/g2p_mix.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      423 2024-04-01 12:42:37.000000 g2p_mix-0.3.6/g2p_mix.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2024-04-01 12:42:37.000000 g2p_mix-0.3.6/g2p_mix.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       87 2024-04-01 12:42:37.000000 g2p_mix-0.3.6/g2p_mix.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)        8 2024-04-01 12:42:37.000000 g2p_mix-0.3.6/g2p_mix.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       48 2024-03-29 02:28:25.000000 g2p_mix-0.3.6/requirements.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2024-04-01 12:42:37.872156 g2p_mix-0.3.6/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1465 2024-04-01 12:42:25.000000 g2p_mix-0.3.6/setup.py
```

### Comparing `g2p_mix-0.3.5/LICENSE` & `g2p_mix-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.5/PKG-INFO` & `g2p_mix-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p_mix
-Version: 0.3.5
+Version: 0.3.6
 Summary: G2P mix
 Home-page: https://github.com/pengzhendong/g2p_mix
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
```

### Comparing `g2p_mix-0.3.5/README.md` & `g2p_mix-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.5/g2p_mix/__init__.py` & `g2p_mix-0.3.6/g2p_mix/__init__.py`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.5/g2p_mix/constants.py` & `g2p_mix-0.3.6/g2p_mix/constants.py`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.5/g2p_mix/g2p_eng.py` & `g2p_mix-0.3.6/g2p_mix/g2p_eng.py`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.5/g2p_mix/g2p_mix.py` & `g2p_mix-0.3.6/g2p_mix/g2p_mix.py`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.5/g2p_mix/nltk_data/corpora/cmudict.zip` & `g2p_mix-0.3.6/g2p_mix/nltk_data/corpora/cmudict.zip`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.5/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip` & `g2p_mix-0.3.6/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.5/g2p_mix/token.py` & `g2p_mix-0.3.6/g2p_mix/token.py`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.5/g2p_mix/tone_sandhi.py` & `g2p_mix-0.3.6/g2p_mix/tone_sandhi.py`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.5/g2p_mix.egg-info/PKG-INFO` & `g2p_mix-0.3.6/g2p_mix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p-mix
-Version: 0.3.5
+Version: 0.3.6
 Summary: G2P mix
 Home-page: https://github.com/pengzhendong/g2p_mix
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
```

### Comparing `g2p_mix-0.3.5/setup.py` & `g2p_mix-0.3.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,22 +21,23 @@
 
 with open("requirements.txt", encoding="utf-8") as f:
     requirements = f.readlines()
 extras_require = {"g2pw": ["torch", "modelscope", "pypinyin-g2pw"]}
 
 setup(
     name="g2p_mix",
-    version=os.getenv("BUILD_VERSION") or "0.3.5",
+    version=os.getenv("BUILD_VERSION") or "0.3.6",
     author="Zhendong Peng",
     author_email="pzd17@tsinghua.org.cn",
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="G2P mix",
     url="https://github.com/pengzhendong/g2p_mix",
     packages=find_packages(),
+    include_package_data=True,
     install_requires=requirements,
     extras_require=extras_require,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering",
     ],
 )
```

