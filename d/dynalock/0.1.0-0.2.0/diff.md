# Comparing `tmp/dynalock-0.1.0.tar.gz` & `tmp/dynalock-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynalock-0.1.0.tar", last modified: Sat Mar 30 18:34:12 2024, max compression
+gzip compressed data, was "dynalock-0.2.0.tar", last modified: Mon Apr  1 16:17:42 2024, max compression
```

## Comparing `dynalock-0.1.0.tar` & `dynalock-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxr-x   0 bombadil  (1000) bombadil  (1000)        0 2024-03-30 18:34:12.557320 dynalock-0.1.0/
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      157 2024-03-30 15:55:11.000000 dynalock-0.1.0/AUTHORS.rst
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)     3532 2024-03-30 15:55:11.000000 dynalock-0.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)       89 2024-03-30 15:55:11.000000 dynalock-0.1.0/HISTORY.rst
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)     1071 2024-03-30 15:55:11.000000 dynalock-0.1.0/LICENSE
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      262 2024-03-30 15:55:12.000000 dynalock-0.1.0/MANIFEST.in
--rw-r--r--   0 bombadil  (1000) bombadil  (1000)     1753 2024-03-30 18:34:12.557320 dynalock-0.1.0/PKG-INFO
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      869 2024-03-30 15:55:11.000000 dynalock-0.1.0/README.rst
-drwxrwxr-x   0 bombadil  (1000) bombadil  (1000)        0 2024-03-30 18:34:12.553320 dynalock-0.1.0/docs/
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      609 2024-03-30 15:55:12.000000 dynalock-0.1.0/docs/Makefile
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)       28 2024-03-30 15:55:12.000000 dynalock-0.1.0/docs/authors.rst
--rwxrwxr-x   0 bombadil  (1000) bombadil  (1000)     4791 2024-03-30 15:55:12.000000 dynalock-0.1.0/docs/conf.py
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)       33 2024-03-30 15:55:12.000000 dynalock-0.1.0/docs/contributing.rst
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)       28 2024-03-30 15:55:12.000000 dynalock-0.1.0/docs/history.rst
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      305 2024-03-30 15:55:12.000000 dynalock-0.1.0/docs/index.rst
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)     1138 2024-03-30 15:55:12.000000 dynalock-0.1.0/docs/installation.rst
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      806 2024-03-30 15:55:12.000000 dynalock-0.1.0/docs/make.bat
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)       27 2024-03-30 15:55:12.000000 dynalock-0.1.0/docs/readme.rst
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)       71 2024-03-30 15:55:12.000000 dynalock-0.1.0/docs/usage.rst
-drwxrwxr-x   0 bombadil  (1000) bombadil  (1000)        0 2024-03-30 18:34:12.553320 dynalock-0.1.0/dynalock/
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      158 2024-03-30 18:25:35.000000 dynalock-0.1.0/dynalock/__init__.py
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)     2317 2024-03-30 18:22:05.000000 dynalock-0.1.0/dynalock/dynalock.py
-drwxrwxr-x   0 bombadil  (1000) bombadil  (1000)        0 2024-03-30 18:34:12.557320 dynalock-0.1.0/dynalock.egg-info/
--rw-r--r--   0 bombadil  (1000) bombadil  (1000)     1753 2024-03-30 18:34:12.000000 dynalock-0.1.0/dynalock.egg-info/PKG-INFO
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      528 2024-03-30 18:34:12.000000 dynalock-0.1.0/dynalock.egg-info/SOURCES.txt
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)        1 2024-03-30 18:34:12.000000 dynalock-0.1.0/dynalock.egg-info/dependency_links.txt
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)        1 2024-03-30 16:16:55.000000 dynalock-0.1.0/dynalock.egg-info/not-zip-safe
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)       31 2024-03-30 18:34:12.000000 dynalock-0.1.0/dynalock.egg-info/requires.txt
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)        9 2024-03-30 18:34:12.000000 dynalock-0.1.0/dynalock.egg-info/top_level.txt
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      423 2024-03-30 18:34:12.557320 dynalock-0.1.0/setup.cfg
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)     1354 2024-03-30 18:33:14.000000 dynalock-0.1.0/setup.py
-drwxrwxr-x   0 bombadil  (1000) bombadil  (1000)        0 2024-03-30 18:34:12.557320 dynalock-0.1.0/tests/
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)       38 2024-03-30 15:55:12.000000 dynalock-0.1.0/tests/__init__.py
--rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      556 2024-03-30 15:55:12.000000 dynalock-0.1.0/tests/test_dynalock.py
+drwxrwxr-x   0 bombadil  (1000) bombadil  (1000)        0 2024-04-01 16:17:42.195381 dynalock-0.2.0/
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      157 2024-03-30 15:55:11.000000 dynalock-0.2.0/AUTHORS.rst
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)     3532 2024-03-30 15:55:11.000000 dynalock-0.2.0/CONTRIBUTING.rst
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)       89 2024-03-30 15:55:11.000000 dynalock-0.2.0/HISTORY.rst
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)     1071 2024-03-30 15:55:11.000000 dynalock-0.2.0/LICENSE
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      262 2024-03-30 15:55:12.000000 dynalock-0.2.0/MANIFEST.in
+-rw-r--r--   0 bombadil  (1000) bombadil  (1000)     2566 2024-04-01 16:17:42.191381 dynalock-0.2.0/PKG-INFO
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)     1680 2024-04-01 16:17:17.000000 dynalock-0.2.0/README.rst
+drwxrwxr-x   0 bombadil  (1000) bombadil  (1000)        0 2024-04-01 16:17:42.187381 dynalock-0.2.0/docs/
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)    15720 2024-04-01 16:17:17.000000 dynalock-0.2.0/docs/DynaLockLogo.png
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      609 2024-03-30 15:55:12.000000 dynalock-0.2.0/docs/Makefile
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)       28 2024-03-30 15:55:12.000000 dynalock-0.2.0/docs/authors.rst
+-rwxrwxr-x   0 bombadil  (1000) bombadil  (1000)     4886 2024-04-01 16:17:17.000000 dynalock-0.2.0/docs/conf.py
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)       33 2024-03-30 15:55:12.000000 dynalock-0.2.0/docs/contributing.rst
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)       28 2024-03-30 15:55:12.000000 dynalock-0.2.0/docs/history.rst
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      305 2024-04-01 16:17:17.000000 dynalock-0.2.0/docs/index.rst
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      542 2024-04-01 16:17:17.000000 dynalock-0.2.0/docs/installation.rst
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      806 2024-03-30 15:55:12.000000 dynalock-0.2.0/docs/make.bat
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)       27 2024-03-30 15:55:12.000000 dynalock-0.2.0/docs/readme.rst
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)     5968 2024-04-01 16:17:17.000000 dynalock-0.2.0/docs/usage.rst
+drwxrwxr-x   0 bombadil  (1000) bombadil  (1000)        0 2024-04-01 16:17:42.191381 dynalock-0.2.0/dynalock/
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      247 2024-04-01 16:17:17.000000 dynalock-0.2.0/dynalock/__init__.py
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)     3577 2024-04-01 16:17:17.000000 dynalock-0.2.0/dynalock/dynalock.py
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      145 2024-04-01 16:17:17.000000 dynalock-0.2.0/dynalock/exceptions.py
+drwxrwxr-x   0 bombadil  (1000) bombadil  (1000)        0 2024-04-01 16:17:42.191381 dynalock-0.2.0/dynalock.egg-info/
+-rw-r--r--   0 bombadil  (1000) bombadil  (1000)     2566 2024-04-01 16:17:42.000000 dynalock-0.2.0/dynalock.egg-info/PKG-INFO
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      573 2024-04-01 16:17:42.000000 dynalock-0.2.0/dynalock.egg-info/SOURCES.txt
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)        1 2024-04-01 16:17:42.000000 dynalock-0.2.0/dynalock.egg-info/dependency_links.txt
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)        1 2024-03-30 16:16:55.000000 dynalock-0.2.0/dynalock.egg-info/not-zip-safe
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)       33 2024-04-01 16:17:42.000000 dynalock-0.2.0/dynalock.egg-info/requires.txt
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)        9 2024-04-01 16:17:42.000000 dynalock-0.2.0/dynalock.egg-info/top_level.txt
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      423 2024-04-01 16:17:42.195381 dynalock-0.2.0/setup.cfg
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)     1356 2024-04-01 16:17:17.000000 dynalock-0.2.0/setup.py
+drwxrwxr-x   0 bombadil  (1000) bombadil  (1000)        0 2024-04-01 16:17:42.191381 dynalock-0.2.0/tests/
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)       38 2024-03-30 15:55:12.000000 dynalock-0.2.0/tests/__init__.py
+-rw-rw-r--   0 bombadil  (1000) bombadil  (1000)      556 2024-03-30 15:55:12.000000 dynalock-0.2.0/tests/test_dynalock.py
```

### Comparing `dynalock-0.1.0/CONTRIBUTING.rst` & `dynalock-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dynalock-0.1.0/LICENSE` & `dynalock-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dynalock-0.1.0/docs/Makefile` & `dynalock-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dynalock-0.1.0/docs/conf.py` & `dynalock-0.2.0/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,30 +27,31 @@
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
+extensions = ['sphinx.ext.autodoc', 
+              'sphinx.ext.viewcode']
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = 'dynalock'
+project = 'Dynaock'
 copyright = "2024, Hamzah Bawah"
 author = "Hamzah Bawah"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
@@ -79,15 +80,15 @@
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = 'sphinx_book_theme'
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
@@ -154,9 +155,13 @@
      'dynalock Documentation',
      author,
      'dynalock',
      'One line description of project.',
      'Miscellaneous'),
 ]
 
+html_title = "DynaLock Documentation"
+
+html_logo = "./DynaLockLogo.png"
+
```

### Comparing `dynalock-0.1.0/docs/make.bat` & `dynalock-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dynalock-0.1.0/dynalock.egg-info/SOURCES.txt` & `dynalock-0.2.0/dynalock.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
+docs/DynaLockLogo.png
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 dynalock/__init__.py
 dynalock/dynalock.py
+dynalock/exceptions.py
 dynalock.egg-info/PKG-INFO
 dynalock.egg-info/SOURCES.txt
 dynalock.egg-info/dependency_links.txt
 dynalock.egg-info/not-zip-safe
 dynalock.egg-info/requires.txt
 dynalock.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `dynalock-0.1.0/setup.py` & `dynalock-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = [
-    "boto3>=1.18.0",
-    "botocore>=1.21.0",
+    "boto3>=1.34.74",
+    "botocore>=1.34.74",
 ]
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Hamzah Bawah",
     author_email='bhamza123@gmail.com',
@@ -39,10 +39,10 @@
     include_package_data=True,
     keywords='dynalock',
     name='dynalock',
     packages=find_packages(include=['dynalock', 'dynalock.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/skywalker427/dynalock',
-    version='0.1.0',
+    version='0.2.0',
     zip_safe=False,
 )
```

### Comparing `dynalock-0.1.0/tests/test_dynalock.py` & `dynalock-0.2.0/tests/test_dynalock.py`

 * *Files identical despite different names*

