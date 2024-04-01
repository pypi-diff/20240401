# Comparing `tmp/rot-kbd-2024.4.1.tar.gz` & `tmp/rot-kbd-2024.4.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rot-kbd-2024.4.1.tar", last modified: Sun Mar 31 23:56:57 2024, max compression
+gzip compressed data, was "rot-kbd-2024.4.1.post1.tar", last modified: Mon Apr  1 13:37:41 2024, max compression
```

## Comparing `rot-kbd-2024.4.1.tar` & `rot-kbd-2024.4.1.post1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-31 23:56:57.111698 rot-kbd-2024.4.1/
--rw-r--r--   0 alex       (501) staff       (20)     1056 2024-03-31 00:58:22.000000 rot-kbd-2024.4.1/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)     1239 2024-03-31 23:56:57.111504 rot-kbd-2024.4.1/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      652 2024-03-31 11:37:45.000000 rot-kbd-2024.4.1/README.md
--rw-r--r--   0 alex       (501) staff       (20)      671 2024-03-31 09:28:04.000000 rot-kbd-2024.4.1/pyproject.toml
--rw-r--r--   0 alex       (501) staff       (20)       38 2024-03-31 23:56:57.111742 rot-kbd-2024.4.1/setup.cfg
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-31 23:56:57.110509 rot-kbd-2024.4.1/src/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-31 23:56:57.111288 rot-kbd-2024.4.1/src/rot_kbd.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     1239 2024-03-31 23:56:57.000000 rot-kbd-2024.4.1/src/rot_kbd.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      187 2024-03-31 23:56:57.000000 rot-kbd-2024.4.1/src/rot_kbd.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2024-03-31 23:56:57.000000 rot-kbd-2024.4.1/src/rot_kbd.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)        8 2024-03-31 23:56:57.000000 rot-kbd-2024.4.1/src/rot_kbd.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)     2882 2024-03-31 01:41:07.000000 rot-kbd-2024.4.1/src/rot_kbd.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-01 13:37:41.996261 rot-kbd-2024.4.1.post1/
+-rw-r--r--   0 alex       (501) staff       (20)     1056 2024-03-31 00:58:22.000000 rot-kbd-2024.4.1.post1/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)     1312 2024-04-01 13:37:41.996067 rot-kbd-2024.4.1.post1/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      719 2024-04-01 13:35:30.000000 rot-kbd-2024.4.1.post1/README.md
+-rw-r--r--   0 alex       (501) staff       (20)      677 2024-04-01 13:35:58.000000 rot-kbd-2024.4.1.post1/pyproject.toml
+-rw-r--r--   0 alex       (501) staff       (20)       38 2024-04-01 13:37:41.996307 rot-kbd-2024.4.1.post1/setup.cfg
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-01 13:37:41.995172 rot-kbd-2024.4.1.post1/src/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-01 13:37:41.995854 rot-kbd-2024.4.1.post1/src/rot_kbd.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     1312 2024-04-01 13:37:41.000000 rot-kbd-2024.4.1.post1/src/rot_kbd.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      187 2024-04-01 13:37:41.000000 rot-kbd-2024.4.1.post1/src/rot_kbd.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-01 13:37:41.000000 rot-kbd-2024.4.1.post1/src/rot_kbd.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)        8 2024-04-01 13:37:41.000000 rot-kbd-2024.4.1.post1/src/rot_kbd.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)     2882 2024-03-31 01:41:07.000000 rot-kbd-2024.4.1.post1/src/rot_kbd.py
```

### Comparing `rot-kbd-2024.4.1/LICENSE` & `rot-kbd-2024.4.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `rot-kbd-2024.4.1/PKG-INFO` & `rot-kbd-2024.4.1.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rot-kbd
-Version: 2024.4.1
+Version: 2024.4.1.post1
 Summary: A terrible encryption scheme, like rot13 but keyboards
 Author-email: Alex Willmer <alex@moreati.org.uk>
 Project-URL: Homepage, https://github.com/moreati/rot-kbd
 Project-URL: Issues, https://github.com/moreati/rot-kbd/issues
 Keywords: dvorak,qwerty
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -45,7 +45,11 @@
 
 ## Supposedly Asked Questions
 
 ### Is this secure?
 
 Absolutely not, it's not even close. `rot_wertyq` and `rot_yqwert` are
 certified upto an adversary rated SA 8.75 (Sibling, Age 8¾).
+
+### Is this some kind-a joke?
+
+Yes. We prefer them to mean jokes.
```

### Comparing `rot-kbd-2024.4.1/README.md` & `rot-kbd-2024.4.1.post1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -29,7 +29,11 @@
 
 ## Supposedly Asked Questions
 
 ### Is this secure?
 
 Absolutely not, it's not even close. `rot_wertyq` and `rot_yqwert` are
 certified upto an adversary rated SA 8.75 (Sibling, Age 8¾).
+
+### Is this some kind-a joke?
+
+Yes. We prefer them to mean jokes.
```

### Comparing `rot-kbd-2024.4.1/pyproject.toml` & `rot-kbd-2024.4.1.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rot-kbd"
-version = "2024.4.1"
+version = "2024.4.1.post1"
 authors = [
     {name="Alex Willmer", email="alex@moreati.org.uk"},
 ]
 description = "A terrible encryption scheme, like rot13 but keyboards"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `rot-kbd-2024.4.1/src/rot_kbd.egg-info/PKG-INFO` & `rot-kbd-2024.4.1.post1/src/rot_kbd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rot-kbd
-Version: 2024.4.1
+Version: 2024.4.1.post1
 Summary: A terrible encryption scheme, like rot13 but keyboards
 Author-email: Alex Willmer <alex@moreati.org.uk>
 Project-URL: Homepage, https://github.com/moreati/rot-kbd
 Project-URL: Issues, https://github.com/moreati/rot-kbd/issues
 Keywords: dvorak,qwerty
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -45,7 +45,11 @@
 
 ## Supposedly Asked Questions
 
 ### Is this secure?
 
 Absolutely not, it's not even close. `rot_wertyq` and `rot_yqwert` are
 certified upto an adversary rated SA 8.75 (Sibling, Age 8¾).
+
+### Is this some kind-a joke?
+
+Yes. We prefer them to mean jokes.
```

### Comparing `rot-kbd-2024.4.1/src/rot_kbd.py` & `rot-kbd-2024.4.1.post1/src/rot_kbd.py`

 * *Files identical despite different names*

