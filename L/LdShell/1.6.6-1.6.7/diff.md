# Comparing `tmp/LdShell-1.6.6.tar.gz` & `tmp/LdShell-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LdShell-1.6.6.tar", last modified: Mon Apr  1 08:58:40 2024, max compression
+gzip compressed data, was "LdShell-1.6.7.tar", last modified: Mon Apr  1 09:42:50 2024, max compression
```

## Comparing `LdShell-1.6.6.tar` & `LdShell-1.6.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 08:58:40.181058 LdShell-1.6.6/
--rw-rw-rw-   0        0        0     1060 2024-03-21 08:18:32.000000 LdShell-1.6.6/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-01 08:58:40.175251 LdShell-1.6.6/LdShell/
--rw-rw-rw-   0        0        0       20 2024-03-21 08:18:32.000000 LdShell-1.6.6/LdShell/__init__.py
--rw-rw-rw-   0        0        0      352 2024-03-21 08:18:32.000000 LdShell-1.6.6/LdShell/__version__.py
--rw-rw-rw-   0        0        0     7392 2024-04-01 08:57:41.000000 LdShell-1.6.6/LdShell/core.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:58:40.179751 LdShell-1.6.6/LdShell.egg-info/
--rw-rw-rw-   0        0        0     3038 2024-04-01 08:58:40.000000 LdShell-1.6.6/LdShell.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-04-01 08:58:40.000000 LdShell-1.6.6/LdShell.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 08:58:40.000000 LdShell-1.6.6/LdShell.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-01 08:58:40.000000 LdShell-1.6.6/LdShell.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2024-03-21 08:18:32.000000 LdShell-1.6.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3038 2024-04-01 08:58:40.179751 LdShell-1.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     2338 2024-03-21 08:18:32.000000 LdShell-1.6.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-01 08:58:40.182037 LdShell-1.6.6/setup.cfg
--rw-rw-rw-   0        0        0     3767 2024-04-01 08:58:36.000000 LdShell-1.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:42:50.668486 LdShell-1.6.7/
+-rw-rw-rw-   0        0        0     1060 2024-03-21 08:18:32.000000 LdShell-1.6.7/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-01 09:42:50.661913 LdShell-1.6.7/LdShell/
+-rw-rw-rw-   0        0        0       20 2024-03-21 08:18:32.000000 LdShell-1.6.7/LdShell/__init__.py
+-rw-rw-rw-   0        0        0      352 2024-03-21 08:18:32.000000 LdShell-1.6.7/LdShell/__version__.py
+-rw-rw-rw-   0        0        0     8036 2024-04-01 09:40:54.000000 LdShell-1.6.7/LdShell/core.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:42:50.665816 LdShell-1.6.7/LdShell.egg-info/
+-rw-rw-rw-   0        0        0     3038 2024-04-01 09:42:50.000000 LdShell-1.6.7/LdShell.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-04-01 09:42:50.000000 LdShell-1.6.7/LdShell.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 09:42:50.000000 LdShell-1.6.7/LdShell.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-01 09:42:50.000000 LdShell-1.6.7/LdShell.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2024-03-21 08:18:32.000000 LdShell-1.6.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3038 2024-04-01 09:42:50.667002 LdShell-1.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2338 2024-03-21 08:18:32.000000 LdShell-1.6.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-01 09:42:50.668486 LdShell-1.6.7/setup.cfg
+-rw-rw-rw-   0        0        0     3767 2024-04-01 09:42:25.000000 LdShell-1.6.7/setup.py
```

### Comparing `LdShell-1.6.6/LICENSE` & `LdShell-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `LdShell-1.6.6/LdShell/core.py` & `LdShell-1.6.7/LdShell/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,16 +22,18 @@
         text=13
         content=14
         child=15
         Tap=16
         Checked=17
 class InitLdPlayer :
      index=0
-     def __init__(self, index=None):
+     _debug=False
+     def __init__(self, index=None,debug=False):
           InitLdPlayer.index=index
+          InitLdPlayer._debug=debug
     
       
 class d() :
 
     # 下面定义了一个类变量
     lds=None
     resourceid =None
@@ -67,29 +69,47 @@
 
             }
     def IniPost(self,ldtype):
         for a in range(3):
             try:
                 self.initJson(ldtype);
                 url = 'http://127.0.0.1:33221/ldshell/'
+                if(InitLdPlayer._debug):
+                    print(url)
+                    print(json.dumps(self.lds))
+
                 res = requests.post( url=url,data=json.dumps(self.lds),timeout=30)
+                if(InitLdPlayer._debug):
+                    print(res)
                 return bool(res.text)
-            except:
+            except Exception as e:
+                if(InitLdPlayer._debug):
+                    print(e)
                 time.sleep(1)
                 pass
         return False;
 
     def InistrPost(self,ldtype):
         for a in range(3):
             try:
                 self.initJson(ldtype);
                 url = 'http://127.0.0.1:33221/ldshell/'
+
+                if(InitLdPlayer._debug):
+                    print(url)
+                    print(json.dumps(self.lds))
                 res = requests.post(url=url,data=json.dumps(self.lds),timeout=30)
+
+                if(InitLdPlayer._debug):
+                    print(res)
+                    
                 return res.text
-            except:
+            except Exception as e:
+                if(InitLdPlayer._debug):
+                    print(e)
                 time.sleep(1)
                 pass
         return "";
 
     # 下面定义了一个CLick方法
     def Click(self):
         return self.IniPost(LdType.Click)
```

### Comparing `LdShell-1.6.6/LdShell.egg-info/PKG-INFO` & `LdShell-1.6.7/LdShell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LdShell
-Version: 1.6.6
+Version: 1.6.7
 Summary: My short description for my project.
 Home-page: http://www.google.com/
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `LdShell-1.6.6/PKG-INFO` & `LdShell-1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LdShell
-Version: 1.6.6
+Version: 1.6.7
 Summary: My short description for my project.
 Home-page: http://www.google.com/
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `LdShell-1.6.6/README.md` & `LdShell-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `LdShell-1.6.6/setup.py` & `LdShell-1.6.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'LdShell'
 DESCRIPTION = 'My short description for my project.'
 URL="http://www.google.com/"
 EMAIL = 'me@example.com'
 AUTHOR = 'Awesome Soul'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.6.6'
+VERSION = '1.6.7'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

