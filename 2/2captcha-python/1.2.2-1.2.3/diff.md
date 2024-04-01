# Comparing `tmp/2captcha-python-1.2.2.tar.gz` & `tmp/2captcha-python-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2captcha-python-1.2.2.tar", last modified: Mon Oct  9 11:35:30 2023, max compression
+gzip compressed data, was "2captcha-python-1.2.3.tar", last modified: Mon Apr  1 10:53:55 2024, max compression
```

## Comparing `2captcha-python-1.2.2.tar` & `2captcha-python-1.2.3.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 11:35:30.619843 2captcha-python-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 11:35:30.615843 2captcha-python-1.2.2/2captcha_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14432 2023-10-09 11:35:30.000000 2captcha-python-1.2.2/2captcha_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-10-09 11:35:30.000000 2captcha-python-1.2.2/2captcha_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-09 11:35:30.000000 2captcha-python-1.2.2/2captcha_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-09 11:35:30.000000 2captcha-python-1.2.2/2captcha_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-09 11:35:30.000000 2captcha-python-1.2.2/2captcha_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14432 2023-10-09 11:35:30.619843 2captcha-python-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-09 11:35:30.619843 2captcha-python-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 11:35:30.619843 2captcha-python-1.2.2/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2634 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/tests/test_amazon_waf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1774 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/tests/test_canvas.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      720 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/tests/test_capy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1630 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/tests/test_coordinates.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1329 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/tests/test_funcaptcha.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1034 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/tests/test_geetest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      758 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/tests/test_geetest_v4.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1892 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/tests/test_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      727 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/tests/test_hcaptcha.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1254 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/tests/test_keycaptcha.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      985 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/tests/test_lemin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/tests/test_normal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1882 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/tests/test_recaptcha.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2164 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/tests/test_rotate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      835 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/tests/test_text.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      847 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/tests/test_turnstile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 11:35:30.619843 2captcha-python-1.2.2/twocaptcha/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/twocaptcha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/twocaptcha/api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17982 2023-10-09 11:35:20.000000 2captcha-python-1.2.2/twocaptcha/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:53:55.268637 2captcha-python-1.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:53:55.268637 2captcha-python-1.2.3/2captcha_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15429 2024-04-01 10:53:55.000000 2captcha-python-1.2.3/2captcha_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-01 10:53:55.000000 2captcha-python-1.2.3/2captcha_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 10:53:55.000000 2captcha-python-1.2.3/2captcha_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 10:53:55.000000 2captcha-python-1.2.3/2captcha_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 10:53:55.000000 2captcha-python-1.2.3/2captcha_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15429 2024-04-01 10:53:55.268637 2captcha-python-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14947 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 10:53:55.268637 2captcha-python-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:53:55.268637 2captcha-python-1.2.3/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2634 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_amazon_waf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1774 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_canvas.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_capy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1630 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_cutcaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_friendly_captcha.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1329 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_funcaptcha.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1034 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_geetest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      758 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_geetest_v4.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1892 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      727 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_hcaptcha.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1254 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_keycaptcha.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      985 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_lemin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_mtcaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_normal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1882 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_recaptcha.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2164 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_rotate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      835 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_text.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      847 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/tests/test_turnstile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:53:55.268637 2captcha-python-1.2.3/twocaptcha/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/twocaptcha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/twocaptcha/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19639 2024-04-01 10:53:51.000000 2captcha-python-1.2.3/twocaptcha/solver.py
```

### Comparing `2captcha-python-1.2.2/2captcha_python.egg-info/PKG-INFO` & `2captcha-python-1.2.3/2captcha_python.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 2captcha-python
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python module for easy integration with 2Captcha API
 Home-page: https://github.com/2captcha/2captcha-python/
 Author: 2Captcha
 Author-email: info@2captcha.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,17 @@
     - [Amazon WAF](#amazon-waf)
     - [KeyCaptcha](#keycaptcha)
     - [Capy](#capy)
     - [Grid](#grid)
     - [Canvas](#canvas)
     - [ClickCaptcha](#clickcaptcha)
     - [Rotate](#rotate)
+    - [MTCaptcha](#mtcaptcha)
+    - [Friendly Captcha](#friendly_captcha)
+    - [Cutcaptcha](#cutcaptcha)
   - [Other methods](#other-methods)
     - [send / getResult](#send--getresult)
     - [balance](#balance)
     - [report](#report)
     - [Error handling](#error-handling)
     - [Proxies](#proxies)
     - [Async calls](#async-calls)
@@ -264,14 +267,40 @@
 
 ### Rotate
 This method can be used to solve a captcha that asks to rotate an object. Mostly used to bypass FunCaptcha. Returns the rotation angle.
 ```python
 result = solver.rotate('path/to/captcha.jpg', param1=..., ...)
 ```
 
+### MTCaptcha
+Use this method to solve MTCaptcha and obtain a token to bypass the protection.
+```python
+result = solver.mtcaptcha(sitekey='MTPublic-KzqLY1cKH',
+                          url='https://2captcha.com/demo/mtcaptcha',
+                          param1=..., ...)
+```
+
+### Friendly Captcha
+Friendly Captcha solving method. Returns a token.
+```python
+result = solver.friendly_captcha(sitekey='FCMGEMUD2KTDSQ5H',
+                                 url='https://friendlycaptcha.com/demo',
+                                 param1=..., ...)
+```
+
+### Cutcaptcha
+Use this method to solve Cutcaptcha. Returns the response in JSON.
+```python
+result = solver.cutcaptcha(misery_key='ad52c87af17e2ec09b8d918c9f00416b1cb8c320',
+                           apikey='SAs61IAI',
+                           url='https://mysite.com/page/with/cutcaptcha',
+                           param1=..., ...)
+```
+
+
 ## Other methods
 
 ### send / getResult
 These methods can be used for manual captcha submission and answer polling.
 ```python
 import time
 . . . . .
```

### Comparing `2captcha-python-1.2.2/2captcha_python.egg-info/SOURCES.txt` & `2captcha-python-1.2.3/2captcha_python.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,21 +6,24 @@
 2captcha_python.egg-info/dependency_links.txt
 2captcha_python.egg-info/requires.txt
 2captcha_python.egg-info/top_level.txt
 tests/test_amazon_waf.py
 tests/test_canvas.py
 tests/test_capy.py
 tests/test_coordinates.py
+tests/test_cutcaptcha.py
+tests/test_friendly_captcha.py
 tests/test_funcaptcha.py
 tests/test_geetest.py
 tests/test_geetest_v4.py
 tests/test_grid.py
 tests/test_hcaptcha.py
 tests/test_keycaptcha.py
 tests/test_lemin.py
+tests/test_mtcaptcha.py
 tests/test_normal.py
 tests/test_recaptcha.py
 tests/test_rotate.py
 tests/test_text.py
 tests/test_turnstile.py
 twocaptcha/__init__.py
 twocaptcha/api.py
```

### Comparing `2captcha-python-1.2.2/LICENSE` & `2captcha-python-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/PKG-INFO` & `2captcha-python-1.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 2captcha-python
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python module for easy integration with 2Captcha API
 Home-page: https://github.com/2captcha/2captcha-python/
 Author: 2Captcha
 Author-email: info@2captcha.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,17 @@
     - [Amazon WAF](#amazon-waf)
     - [KeyCaptcha](#keycaptcha)
     - [Capy](#capy)
     - [Grid](#grid)
     - [Canvas](#canvas)
     - [ClickCaptcha](#clickcaptcha)
     - [Rotate](#rotate)
+    - [MTCaptcha](#mtcaptcha)
+    - [Friendly Captcha](#friendly_captcha)
+    - [Cutcaptcha](#cutcaptcha)
   - [Other methods](#other-methods)
     - [send / getResult](#send--getresult)
     - [balance](#balance)
     - [report](#report)
     - [Error handling](#error-handling)
     - [Proxies](#proxies)
     - [Async calls](#async-calls)
@@ -264,14 +267,40 @@
 
 ### Rotate
 This method can be used to solve a captcha that asks to rotate an object. Mostly used to bypass FunCaptcha. Returns the rotation angle.
 ```python
 result = solver.rotate('path/to/captcha.jpg', param1=..., ...)
 ```
 
+### MTCaptcha
+Use this method to solve MTCaptcha and obtain a token to bypass the protection.
+```python
+result = solver.mtcaptcha(sitekey='MTPublic-KzqLY1cKH',
+                          url='https://2captcha.com/demo/mtcaptcha',
+                          param1=..., ...)
+```
+
+### Friendly Captcha
+Friendly Captcha solving method. Returns a token.
+```python
+result = solver.friendly_captcha(sitekey='FCMGEMUD2KTDSQ5H',
+                                 url='https://friendlycaptcha.com/demo',
+                                 param1=..., ...)
+```
+
+### Cutcaptcha
+Use this method to solve Cutcaptcha. Returns the response in JSON.
+```python
+result = solver.cutcaptcha(misery_key='ad52c87af17e2ec09b8d918c9f00416b1cb8c320',
+                           apikey='SAs61IAI',
+                           url='https://mysite.com/page/with/cutcaptcha',
+                           param1=..., ...)
+```
+
+
 ## Other methods
 
 ### send / getResult
 These methods can be used for manual captcha submission and answer polling.
 ```python
 import time
 . . . . .
```

### Comparing `2captcha-python-1.2.2/README.md` & `2captcha-python-1.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,17 @@
     - [Amazon WAF](#amazon-waf)
     - [KeyCaptcha](#keycaptcha)
     - [Capy](#capy)
     - [Grid](#grid)
     - [Canvas](#canvas)
     - [ClickCaptcha](#clickcaptcha)
     - [Rotate](#rotate)
+    - [MTCaptcha](#mtcaptcha)
+    - [Friendly Captcha](#friendly_captcha)
+    - [Cutcaptcha](#cutcaptcha)
   - [Other methods](#other-methods)
     - [send / getResult](#send--getresult)
     - [balance](#balance)
     - [report](#report)
     - [Error handling](#error-handling)
     - [Proxies](#proxies)
     - [Async calls](#async-calls)
@@ -249,14 +252,40 @@
 
 ### Rotate
 This method can be used to solve a captcha that asks to rotate an object. Mostly used to bypass FunCaptcha. Returns the rotation angle.
 ```python
 result = solver.rotate('path/to/captcha.jpg', param1=..., ...)
 ```
 
+### MTCaptcha
+Use this method to solve MTCaptcha and obtain a token to bypass the protection.
+```python
+result = solver.mtcaptcha(sitekey='MTPublic-KzqLY1cKH',
+                          url='https://2captcha.com/demo/mtcaptcha',
+                          param1=..., ...)
+```
+
+### Friendly Captcha
+Friendly Captcha solving method. Returns a token.
+```python
+result = solver.friendly_captcha(sitekey='FCMGEMUD2KTDSQ5H',
+                                 url='https://friendlycaptcha.com/demo',
+                                 param1=..., ...)
+```
+
+### Cutcaptcha
+Use this method to solve Cutcaptcha. Returns the response in JSON.
+```python
+result = solver.cutcaptcha(misery_key='ad52c87af17e2ec09b8d918c9f00416b1cb8c320',
+                           apikey='SAs61IAI',
+                           url='https://mysite.com/page/with/cutcaptcha',
+                           param1=..., ...)
+```
+
+
 ## Other methods
 
 ### send / getResult
 These methods can be used for manual captcha submission and answer polling.
 ```python
 import time
 . . . . .
```

### Comparing `2captcha-python-1.2.2/setup.py` & `2captcha-python-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/tests/test_amazon_waf.py` & `2captcha-python-1.2.3/tests/test_amazon_waf.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/tests/test_canvas.py` & `2captcha-python-1.2.3/tests/test_canvas.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/tests/test_capy.py` & `2captcha-python-1.2.3/tests/test_capy.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/tests/test_coordinates.py` & `2captcha-python-1.2.3/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/tests/test_funcaptcha.py` & `2captcha-python-1.2.3/tests/test_funcaptcha.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/tests/test_geetest.py` & `2captcha-python-1.2.3/tests/test_geetest.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/tests/test_geetest_v4.py` & `2captcha-python-1.2.3/tests/test_geetest_v4.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/tests/test_grid.py` & `2captcha-python-1.2.3/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/tests/test_hcaptcha.py` & `2captcha-python-1.2.3/tests/test_hcaptcha.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/tests/test_keycaptcha.py` & `2captcha-python-1.2.3/tests/test_keycaptcha.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/tests/test_lemin.py` & `2captcha-python-1.2.3/tests/test_lemin.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/tests/test_normal.py` & `2captcha-python-1.2.3/tests/test_normal.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/tests/test_recaptcha.py` & `2captcha-python-1.2.3/tests/test_recaptcha.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/tests/test_rotate.py` & `2captcha-python-1.2.3/tests/test_rotate.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/tests/test_text.py` & `2captcha-python-1.2.3/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/tests/test_turnstile.py` & `2captcha-python-1.2.3/tests/test_turnstile.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/twocaptcha/api.py` & `2captcha-python-1.2.3/twocaptcha/api.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.2/twocaptcha/solver.py` & `2captcha-python-1.2.3/twocaptcha/solver.py`

 * *Files 5% similar despite different names*

```diff
@@ -499,15 +499,75 @@
                             context=context,
                             url=url,
                             method='amazon_waf',
                             **kwargs)
         
         return result
 
+    def mtcaptcha(self, sitekey, url, **kwargs):
+        '''
+        Wrapper for solving MTCaptcha
+
+        Required:
+            sitekey
+            url
+
+        Optional params:
+            softId
+            callback
+            proxy           =  {'type': 'HTTPS', 'uri': 'login:password@IP_address:PORT'})
+        '''
+
+        result = self.solve(sitekey=sitekey,
+                            url=url,
+                            method='mt_captcha',
+                            **kwargs)
+        return result
+
+    def friendly_captcha(self, sitekey, url, **kwargs):
+        '''
+        Wrapper for solving Friendly Captcha
+
+        Required:
+            sitekey
+            url
+
+        Optional params:
+            softId
+            callback
+            proxy           =  {'type': 'HTTPS', 'uri': 'login:password@IP_address:PORT'})
+        '''
 
+        result = self.solve(sitekey=sitekey,
+                            url=url,
+                            method='friendly_captcha',
+                            **kwargs)
+        return result
+
+    def cutcaptcha(self, misery_key, apikey, url, **kwargs):
+        '''
+        Wrapper for solving Friendly Captcha
+
+        Required:
+            misery_key
+            apikey
+            url
+
+        Optional params:
+            softId
+            callback
+            proxy           =  {'type': 'HTTPS', 'uri': 'login:password@IP_address:PORT'})
+        '''
+
+        result = self.solve(misery_key=misery_key,
+                            api_key=apikey,
+                            url=url,
+                            method='cutcaptcha',
+                            **kwargs)
+        return result
 
     def solve(self, timeout=0, polling_interval=0, **kwargs):
         '''
         sends captcha, receives result
 
 
         Parameters
```

