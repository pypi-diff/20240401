# Comparing `tmp/fsbi-0.3.tar.gz` & `tmp/fsbi-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsbi-0.3.tar", last modified: Sun Mar 31 19:25:49 2024, max compression
+gzip compressed data, was "fsbi-0.4.tar", last modified: Mon Apr  1 11:18:20 2024, max compression
```

## Comparing `fsbi-0.3.tar` & `fsbi-0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 19:25:49.141632 fsbi-0.3/
--rw-rw-rw-   0        0        0     2098 2024-03-31 19:25:49.141632 fsbi-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-31 19:25:49.126006 fsbi-0.3/fsbi/
--rw-rw-rw-   0        0        0     2280 2024-03-31 19:07:51.000000 fsbi-0.3/fsbi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 19:25:49.141632 fsbi-0.3/fsbi.egg-info/
--rw-rw-rw-   0        0        0     2098 2024-03-31 19:25:49.000000 fsbi-0.3/fsbi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2024-03-31 19:25:49.000000 fsbi-0.3/fsbi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 19:25:49.000000 fsbi-0.3/fsbi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-03-31 19:25:49.000000 fsbi-0.3/fsbi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-03-31 19:25:49.000000 fsbi-0.3/fsbi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 19:25:49.141632 fsbi-0.3/setup.cfg
--rw-rw-rw-   0        0        0     2152 2024-03-31 19:20:40.000000 fsbi-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 11:18:20.074053 fsbi-0.4/
+-rw-rw-rw-   0        0        0     2320 2024-04-01 11:18:20.074053 fsbi-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-01 11:18:20.074053 fsbi-0.4/fsbi/
+-rw-rw-rw-   0        0        0     2314 2024-04-01 11:00:13.000000 fsbi-0.4/fsbi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 11:18:20.074053 fsbi-0.4/fsbi.egg-info/
+-rw-rw-rw-   0        0        0     2320 2024-04-01 11:18:19.000000 fsbi-0.4/fsbi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2024-04-01 11:18:20.000000 fsbi-0.4/fsbi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 11:18:19.000000 fsbi-0.4/fsbi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-01 11:18:19.000000 fsbi-0.4/fsbi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-01 11:18:19.000000 fsbi-0.4/fsbi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 11:18:20.074053 fsbi-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2367 2024-04-01 11:17:56.000000 fsbi-0.4/setup.py
```

### Comparing `fsbi-0.3/PKG-INFO` & `fsbi-0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsbi
-Version: 0.3
+Version: 0.4
 Summary: Font Stretch Bold Italic
 Home-page: http://phyl.io/?page=fsbi.html
 Author: Philippe Kappel
 Author-email: philippe.kappel@gmail.com
 License: MIT
 Keywords: font
 Classifier: Development Status :: 3 - Alpha
@@ -73,7 +73,14 @@
 | 3 | Condensed | Light
 | 4 | SemiCondensed | Regular
 | 5 | Normal | Medium
 | 6 | SemiExtended | SemiBold
 | 7 | Extended | Bold
 | 8 | ExtraExtended | ExtraBold
 | 9 | UltraExtended | Black
+
+# Changelog
+
+- 2024.04.01 – **0.4** – Parse `Expanded` keyword as `Extended`
+- 2024.03.31 – **0.3** – Add `stretch` parameter and `-s` argument
+- 2024.03.31 – **0.2** – Bug fix
+- 2024.03.30 – **0.1**
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fsbi-0.3/fsbi/__init__.py` & `fsbi-0.4/fsbi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 __all__ = ['compact','expand','rename']
 
 def compact(font, stretch=False):
 	d,f,x,s,b,i,t = compact.e(font).groups()
 	return f'''{d or ''}{f}-{5+compact.x[x]*compact.s[s] if s or stretch else ''
 		}{compact.b[b]}{compact.i[i]}.{t}'''
 
-compact.e = re.compile(r'(.*[/\\])?(.+?)(?:(Semi|Extra|Ultra)?(Condensed|Extended))?-'
+compact.e = re.compile(
+	r'(.*[/\\])?(.+?)(?:[-_]?(Semi|Extra|Ultra)?(Condensed|Extended|Expanded))?[-_]?'
 	r'(Hairline|Thin|ExtraLight|Light|Regular|Medium|SemiBold|Bold|ExtraBold|Black|Heavy)?'
 	r'(Italic|Oblique)?\.(otf|ttf|woff2)', re.M).fullmatch
 compact.x = {'Semi':1, None:2, 'Extra':3, 'Ultra':4}
-compact.s = {'Condensed':-1, None:0, 'Extended':1}
+compact.s = {'Condensed':-1, None:0, 'Extended':1, 'Expanded':1}
 compact.b = {'Hairline':0, 'Thin':1, 'ExtraLight':2, 'Light':3, None:4, 'Regular':4,
 	'Medium':5, 'SemiBold':6, 'Bold':7, 'ExtraBold':8, 'Black':9, 'Heavy':9}
 compact.i = {None:'', 'Italic':'i', 'Oblique':'o'}
 
 def expand(font):
 	d,f,s,b,i,t = expand.e(font).groups()
 	s,b = int(s or 5)-5, int(b)
```

### Comparing `fsbi-0.3/fsbi.egg-info/PKG-INFO` & `fsbi-0.4/fsbi.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsbi
-Version: 0.3
+Version: 0.4
 Summary: Font Stretch Bold Italic
 Home-page: http://phyl.io/?page=fsbi.html
 Author: Philippe Kappel
 Author-email: philippe.kappel@gmail.com
 License: MIT
 Keywords: font
 Classifier: Development Status :: 3 - Alpha
@@ -73,7 +73,14 @@
 | 3 | Condensed | Light
 | 4 | SemiCondensed | Regular
 | 5 | Normal | Medium
 | 6 | SemiExtended | SemiBold
 | 7 | Extended | Bold
 | 8 | ExtraExtended | ExtraBold
 | 9 | UltraExtended | Black
+
+# Changelog
+
+- 2024.04.01 – **0.4** – Parse `Expanded` keyword as `Extended`
+- 2024.03.31 – **0.3** – Add `stretch` parameter and `-s` argument
+- 2024.03.31 – **0.2** – Bug fix
+- 2024.03.30 – **0.1**
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fsbi-0.3/setup.py` & `fsbi-0.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -52,19 +52,26 @@
 | 2 | ExtraCondensed | ExtraLight
 | 3 | Condensed | Light
 | 4 | SemiCondensed | Regular
 | 5 | Normal | Medium
 | 6 | SemiExtended | SemiBold
 | 7 | Extended | Bold
 | 8 | ExtraExtended | ExtraBold
-| 9 | UltraExtended | Black'''
+| 9 | UltraExtended | Black
+
+# Changelog
+
+- 2024.04.01 – **0.4** – Parse `Expanded` keyword as `Extended`
+- 2024.03.31 – **0.3** – Add `stretch` parameter and `-s` argument
+- 2024.03.31 – **0.2** – Bug fix
+- 2024.03.30 – **0.1**'''
 
 setup(
 	name = 'fsbi',
-	version = '0.3',
+	version = '0.4',
 	description = 'Font Stretch Bold Italic',
 	long_description = description,
 	long_description_content_type = 'text/markdown',
 	license = 'MIT',
 	url = 'http://phyl.io/?page=fsbi.html',
 	author = 'Philippe Kappel',
 	author_email = 'philippe.kappel@gmail.com',
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

