# Comparing `tmp/nestpython-0.3.1.tar.gz` & `tmp/nestpython-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestpython-0.3.1.tar", last modified: Mon Apr  1 17:22:35 2024, max compression
+gzip compressed data, was "nestpython-0.3.2.tar", last modified: Mon Apr  1 18:03:02 2024, max compression
```

## Comparing `nestpython-0.3.1.tar` & `nestpython-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 17:22:35.068213 nestpython-0.3.1/
--rw-rw-rw-   0        0        0     1346 2024-04-01 17:22:35.066218 nestpython-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1141 2024-04-01 17:19:29.000000 nestpython-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 17:22:35.058241 nestpython-0.3.1/nestpy/
--rw-rw-rw-   0        0        0       39 2024-04-01 14:53:49.000000 nestpython-0.3.1/nestpy/__init__.py
--rw-rw-rw-   0        0        0     2340 2024-04-01 14:53:49.000000 nestpython-0.3.1/nestpy/files.py
--rw-rw-rw-   0        0        0    14518 2024-04-01 16:21:43.000000 nestpython-0.3.1/nestpy/main.py
-drwxrwxrwx   0        0        0        0 2024-04-01 17:22:35.064223 nestpython-0.3.1/nestpython.egg-info/
--rw-rw-rw-   0        0        0     1346 2024-04-01 17:22:34.000000 nestpython-0.3.1/nestpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-04-01 17:22:34.000000 nestpython-0.3.1/nestpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 17:22:34.000000 nestpython-0.3.1/nestpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-01 17:22:34.000000 nestpython-0.3.1/nestpython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 17:22:35.068213 nestpython-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      856 2024-04-01 17:18:49.000000 nestpython-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 18:03:02.659628 nestpython-0.3.2/
+-rw-rw-rw-   0        0        0     1346 2024-04-01 18:03:02.658607 nestpython-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1141 2024-04-01 17:19:29.000000 nestpython-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 18:03:02.650630 nestpython-0.3.2/nestpy/
+-rw-rw-rw-   0        0        0       39 2024-04-01 14:53:49.000000 nestpython-0.3.2/nestpy/__init__.py
+-rw-rw-rw-   0        0        0     2340 2024-04-01 14:53:49.000000 nestpython-0.3.2/nestpy/files.py
+-rw-rw-rw-   0        0        0    14523 2024-04-01 17:49:57.000000 nestpython-0.3.2/nestpy/main.py
+drwxrwxrwx   0        0        0        0 2024-04-01 18:03:02.656612 nestpython-0.3.2/nestpython.egg-info/
+-rw-rw-rw-   0        0        0     1346 2024-04-01 18:03:02.000000 nestpython-0.3.2/nestpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-04-01 18:03:02.000000 nestpython-0.3.2/nestpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 18:03:02.000000 nestpython-0.3.2/nestpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-01 18:03:02.000000 nestpython-0.3.2/nestpython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 18:03:02.660606 nestpython-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      856 2024-04-01 17:25:34.000000 nestpython-0.3.2/setup.py
```

### Comparing `nestpython-0.3.1/PKG-INFO` & `nestpython-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestpython
-Version: 0.3.1
+Version: 0.3.2
 Summary: python with braces.
 Author: slycedf
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 
 ## nestpy
```

### Comparing `nestpython-0.3.1/README.md` & `nestpython-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nestpython-0.3.1/nestpy/files.py` & `nestpython-0.3.2/nestpy/files.py`

 * *Files identical despite different names*

### Comparing `nestpython-0.3.1/nestpy/main.py` & `nestpython-0.3.2/nestpy/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     isNotShorthand = Token(r'!=&', TokenTypes.SHORTHAND)
     defShorthand = Token(r':=', TokenTypes.SHORTHAND)
     inShorthand = Token(r'->', TokenTypes.SHORTHAND)
     notInShorthand = Token(r'!>', TokenTypes.SHORTHAND)
     delShorthand = Token(r'~>', TokenTypes.SHORTHAND)
     lambdaShorthand = Token(r';=', TokenTypes.SHORTHAND)
     indentNewline = Token(r';', TokenTypes.INDENTED, TokenTypes.SYNTACTICAL)
-    notShorthand = Token(r'!', TokenTypes.SHORTHAND)
+    notShorthand = Token(r'!(?!=)', TokenTypes.SHORTHAND)
     andDeconflict = Token(sclund('and'), TokenTypes.APPENDSUB)
     orDeconflict = Token(sclund('or'), TokenTypes.APPENDSUB)
     notDeconflict = Token(sclund('not'), TokenTypes.APPENDSUB)
     isDeconflict = Token(sclund('is'), TokenTypes.APPENDSUB)
     defDeconflict = Token(sclund('def'), TokenTypes.APPENDSUB)
     lambdaDeconflict = Token(sclund('lambda'), TokenTypes.APPENDSUB)
     inDeconflict = Token(sclund('in'), TokenTypes.APPENDSUB)
```

### Comparing `nestpython-0.3.1/nestpython.egg-info/PKG-INFO` & `nestpython-0.3.2/nestpython.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestpython
-Version: 0.3.1
+Version: 0.3.2
 Summary: python with braces.
 Author: slycedf
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 
 ## nestpy
```

### Comparing `nestpython-0.3.1/setup.py` & `nestpython-0.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,11 +19,11 @@
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     classifiers=[
         "Development Status :: 4 - Beta"
     ]
 )
 
-token = open(f'D:/slycefolder/ins/all/{ {True: "tt", False: "tr"}[test]}', 'r').read()
+token = open(f'D:/slycefolder/ins/nsp/{ {True: "tt", False: "tr"}[test]}', 'r').read()
 
 runcmd(
     f'pause & twine upload --repository { {True: "testpypi", False: "pypi"}[test]} dist/*{version}* -u __token__ -p {token} --verbose')
```

