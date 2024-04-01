# Comparing `tmp/botnikkk-0.0.6.tar.gz` & `tmp/botnikkk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botnikkk-0.0.6.tar", last modified: Mon Apr  1 16:08:27 2024, max compression
+gzip compressed data, was "botnikkk-0.0.7.tar", last modified: Mon Apr  1 16:12:02 2024, max compression
```

## Comparing `botnikkk-0.0.6.tar` & `botnikkk-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 16:08:27.182315 botnikkk-0.0.6/
--rw-rw-rw-   0        0        0     2273 2024-04-01 16:08:27.179316 botnikkk-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1633 2024-04-01 16:06:13.000000 botnikkk-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 16:08:27.167320 botnikkk-0.0.6/botnikkk/
--rw-rw-rw-   0        0        0      172 2024-03-31 09:55:49.000000 botnikkk-0.0.6/botnikkk/__init__.py
--rw-rw-rw-   0        0        0     2619 2024-04-01 16:02:27.000000 botnikkk-0.0.6/botnikkk/formatting.py
-drwxrwxrwx   0        0        0        0 2024-04-01 16:08:27.178316 botnikkk-0.0.6/botnikkk.egg-info/
--rw-rw-rw-   0        0        0     2273 2024-04-01 16:08:27.000000 botnikkk-0.0.6/botnikkk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-04-01 16:08:27.000000 botnikkk-0.0.6/botnikkk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 16:08:27.000000 botnikkk-0.0.6/botnikkk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-01 16:08:27.000000 botnikkk-0.0.6/botnikkk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-01 16:08:27.000000 botnikkk-0.0.6/botnikkk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 16:08:27.182315 botnikkk-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1000 2024-04-01 16:07:43.000000 botnikkk-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:12:02.010647 botnikkk-0.0.7/
+-rw-rw-rw-   0        0        0     2181 2024-04-01 16:12:02.007647 botnikkk-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1543 2024-04-01 16:11:21.000000 botnikkk-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 16:12:01.995499 botnikkk-0.0.7/botnikkk/
+-rw-rw-rw-   0        0        0      172 2024-03-31 09:55:49.000000 botnikkk-0.0.7/botnikkk/__init__.py
+-rw-rw-rw-   0        0        0     2619 2024-04-01 16:02:27.000000 botnikkk-0.0.7/botnikkk/formatting.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:12:02.004655 botnikkk-0.0.7/botnikkk.egg-info/
+-rw-rw-rw-   0        0        0     2181 2024-04-01 16:12:01.000000 botnikkk-0.0.7/botnikkk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-04-01 16:12:01.000000 botnikkk-0.0.7/botnikkk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 16:12:01.000000 botnikkk-0.0.7/botnikkk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-01 16:12:01.000000 botnikkk-0.0.7/botnikkk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-01 16:12:01.000000 botnikkk-0.0.7/botnikkk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 16:12:02.011647 botnikkk-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1000 2024-04-01 16:11:50.000000 botnikkk-0.0.7/setup.py
```

### Comparing `botnikkk-0.0.6/PKG-INFO` & `botnikkk-0.0.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botnikkk
-Version: 0.0.6
+Version: 0.0.7
 Summary: a personal package
 Author: BotNikkk
 Author-email: <nikhi.ace.chd@gmail.com>
 Keywords: python,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -28,15 +28,14 @@
 ## 1. centre() function
 
 Usage = Centering Elemtents.
 
 ```python
 import botnikkk
 
-#printing a centred text
 botnikkk.centre('text')
 ```
 
 It also takes 2 extra parameters as input :
 
 1. symbol : determines what symbol will fill in the blank space, deault parameter = " "
 
@@ -53,43 +52,41 @@
 ## 2. format_input() function
 
 Usage = centering the input variable.
 
 ```python
 import botnikkk
 
-#printing a centred text
 botnikkk.format_input('input_question')
 ```
 
 ## 3. int_check() function
 
 Usage = checks if an input variable is a interger or not, takes repetetive inputs if not Interger.
 
 ```python
 import botnikkk
 
-#printing a centred text
 botnikkk.int_check('any_variable')
 ```
 
 ## 4. ans_check() function
 
 Usage = takes a list of strings as input and displays it to the user as centred options, returns the choosen option. 
 
 ```python
 import botnikkk
 
-#printing a centred text
 botnikkk.ans_check(['list_of_varibales'])
 ```
 
 ## 4. redirect() function
 
 Usage = takes a input string as screen name and redirects the user to the said screen in a countdown of 3 seconds. Can only be used in async functions due it's await nature.
 
 ```python
 import botnikkk
 
-#printing a centred text
 await botnikkk.redirect("screen_name")
 ```
+
+check out : https://botnikkk.github.io
```

### Comparing `botnikkk-0.0.6/README.md` & `botnikkk-0.0.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 ## 1. centre() function
 
 Usage = Centering Elemtents.
 
 ```python
 import botnikkk
 
-#printing a centred text
 botnikkk.centre('text')
 ```
 
 It also takes 2 extra parameters as input :
 
 1. symbol : determines what symbol will fill in the blank space, deault parameter = " "
 
@@ -35,43 +34,41 @@
 ## 2. format_input() function
 
 Usage = centering the input variable.
 
 ```python
 import botnikkk
 
-#printing a centred text
 botnikkk.format_input('input_question')
 ```
 
 ## 3. int_check() function
 
 Usage = checks if an input variable is a interger or not, takes repetetive inputs if not Interger.
 
 ```python
 import botnikkk
 
-#printing a centred text
 botnikkk.int_check('any_variable')
 ```
 
 ## 4. ans_check() function
 
 Usage = takes a list of strings as input and displays it to the user as centred options, returns the choosen option. 
 
 ```python
 import botnikkk
 
-#printing a centred text
 botnikkk.ans_check(['list_of_varibales'])
 ```
 
 ## 4. redirect() function
 
 Usage = takes a input string as screen name and redirects the user to the said screen in a countdown of 3 seconds. Can only be used in async functions due it's await nature.
 
 ```python
 import botnikkk
 
-#printing a centred text
 await botnikkk.redirect("screen_name")
 ```
+
+check out : https://botnikkk.github.io
```

### Comparing `botnikkk-0.0.6/botnikkk/formatting.py` & `botnikkk-0.0.7/botnikkk/formatting.py`

 * *Files identical despite different names*

### Comparing `botnikkk-0.0.6/botnikkk.egg-info/PKG-INFO` & `botnikkk-0.0.7/botnikkk.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botnikkk
-Version: 0.0.6
+Version: 0.0.7
 Summary: a personal package
 Author: BotNikkk
 Author-email: <nikhi.ace.chd@gmail.com>
 Keywords: python,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -28,15 +28,14 @@
 ## 1. centre() function
 
 Usage = Centering Elemtents.
 
 ```python
 import botnikkk
 
-#printing a centred text
 botnikkk.centre('text')
 ```
 
 It also takes 2 extra parameters as input :
 
 1. symbol : determines what symbol will fill in the blank space, deault parameter = " "
 
@@ -53,43 +52,41 @@
 ## 2. format_input() function
 
 Usage = centering the input variable.
 
 ```python
 import botnikkk
 
-#printing a centred text
 botnikkk.format_input('input_question')
 ```
 
 ## 3. int_check() function
 
 Usage = checks if an input variable is a interger or not, takes repetetive inputs if not Interger.
 
 ```python
 import botnikkk
 
-#printing a centred text
 botnikkk.int_check('any_variable')
 ```
 
 ## 4. ans_check() function
 
 Usage = takes a list of strings as input and displays it to the user as centred options, returns the choosen option. 
 
 ```python
 import botnikkk
 
-#printing a centred text
 botnikkk.ans_check(['list_of_varibales'])
 ```
 
 ## 4. redirect() function
 
 Usage = takes a input string as screen name and redirects the user to the said screen in a countdown of 3 seconds. Can only be used in async functions due it's await nature.
 
 ```python
 import botnikkk
 
-#printing a centred text
 await botnikkk.redirect("screen_name")
 ```
+
+check out : https://botnikkk.github.io
```

### Comparing `botnikkk-0.0.6/setup.py` & `botnikkk-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'a personal package'
 
 # Setting up
 setup(
     name="botnikkk",
     version=VERSION,
     author="BotNikkk",
```

