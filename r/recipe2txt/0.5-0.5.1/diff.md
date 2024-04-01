# Comparing `tmp/recipe2txt-0.5.tar.gz` & `tmp/recipe2txt-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recipe2txt-0.5.tar", last modified: Mon Feb 12 10:28:25 2024, max compression
+gzip compressed data, was "recipe2txt-0.5.1.tar", last modified: Mon Apr  1 20:30:48 2024, max compression
```

## Comparing `recipe2txt-0.5.tar` & `recipe2txt-0.5.1.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-02-12 10:28:25.161930 recipe2txt-0.5/
--rw-rw-r--   0 pc        (1000) pc        (1000)    35149 2023-07-25 13:15:25.000000 recipe2txt-0.5/LICENSE
--rw-r--r--   0 pc        (1000) pc        (1000)     9789 2024-02-12 10:28:25.161930 recipe2txt-0.5/PKG-INFO
--rw-rw-r--   0 pc        (1000) pc        (1000)     8295 2024-02-12 10:23:25.000000 recipe2txt-0.5/README.md
--rw-rw-r--   0 pc        (1000) pc        (1000)     3520 2024-02-12 10:23:25.000000 recipe2txt-0.5/pyproject.toml
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-02-12 10:28:25.157930 recipe2txt-0.5/recipe2txt/
--rw-rw-r--   0 pc        (1000) pc        (1000)        0 2023-07-11 12:26:00.000000 recipe2txt-0.5/recipe2txt/__init__.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     7243 2024-02-12 10:23:25.000000 recipe2txt-0.5/recipe2txt/fetcher.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3380 2024-02-12 10:23:25.000000 recipe2txt-0.5/recipe2txt/fetcher_async.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    10403 2024-02-12 10:23:25.000000 recipe2txt-0.5/recipe2txt/file_setup.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    15276 2024-02-12 10:23:25.000000 recipe2txt-0.5/recipe2txt/html2recipe.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     9424 2024-02-12 10:23:25.000000 recipe2txt-0.5/recipe2txt/parsing_error.py
--rw-rw-r--   0 pc        (1000) pc        (1000)        0 2023-03-10 13:56:18.000000 recipe2txt-0.5/recipe2txt/py.typed
--rw-rw-r--   0 pc        (1000) pc        (1000)     2757 2024-02-12 10:23:25.000000 recipe2txt-0.5/recipe2txt/re2txt.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     4005 2024-02-12 10:23:25.000000 recipe2txt-0.5/recipe2txt/recipes2out.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    15691 2024-02-12 10:23:25.000000 recipe2txt-0.5/recipe2txt/sql.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    10158 2024-02-12 10:23:25.000000 recipe2txt-0.5/recipe2txt/user_interface.py
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-02-12 10:28:25.161930 recipe2txt-0.5/recipe2txt/utils/
--rw-rw-r--   0 pc        (1000) pc        (1000)    18854 2024-02-12 10:23:25.000000 recipe2txt-0.5/recipe2txt/utils/ArgConfig.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    11731 2024-02-12 10:23:25.000000 recipe2txt-0.5/recipe2txt/utils/ContextLogger.py
--rw-rw-r--   0 pc        (1000) pc        (1000)        0 2024-02-12 10:23:25.000000 recipe2txt-0.5/recipe2txt/utils/__init__.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     1259 2024-02-12 10:23:25.000000 recipe2txt-0.5/recipe2txt/utils/conditional_imports.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     4320 2024-02-12 10:23:25.000000 recipe2txt-0.5/recipe2txt/utils/markdown.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    12724 2024-02-12 10:23:25.000000 recipe2txt-0.5/recipe2txt/utils/misc.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3158 2024-02-12 10:23:25.000000 recipe2txt-0.5/recipe2txt/utils/traceback_utils.py
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-02-12 10:28:25.161930 recipe2txt-0.5/recipe2txt.egg-info/
--rw-r--r--   0 pc        (1000) pc        (1000)     9789 2024-02-12 10:28:25.000000 recipe2txt-0.5/recipe2txt.egg-info/PKG-INFO
--rw-rw-r--   0 pc        (1000) pc        (1000)      981 2024-02-12 10:28:25.000000 recipe2txt-0.5/recipe2txt.egg-info/SOURCES.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)        1 2024-02-12 10:28:25.000000 recipe2txt-0.5/recipe2txt.egg-info/dependency_links.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)       86 2024-02-12 10:28:25.000000 recipe2txt-0.5/recipe2txt.egg-info/entry_points.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)      207 2024-02-12 10:28:25.000000 recipe2txt-0.5/recipe2txt.egg-info/requires.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)       11 2024-02-12 10:28:25.000000 recipe2txt-0.5/recipe2txt.egg-info/top_level.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)       38 2024-02-12 10:28:25.161930 recipe2txt-0.5/setup.cfg
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-02-12 10:28:25.161930 recipe2txt-0.5/test/
--rw-rw-r--   0 pc        (1000) pc        (1000)     8838 2024-02-12 10:23:25.000000 recipe2txt-0.5/test/test4recipe2txt.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    17177 2024-02-12 10:23:25.000000 recipe2txt-0.5/test/test_argconfig.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    15034 2024-02-12 10:23:25.000000 recipe2txt-0.5/test/test_contextlogger.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3003 2024-02-12 10:23:25.000000 recipe2txt-0.5/test/test_fetcher.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     5197 2024-02-12 10:23:25.000000 recipe2txt-0.5/test/test_file_setup.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     6174 2024-02-12 10:23:25.000000 recipe2txt-0.5/test/test_helpers.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     4635 2024-02-12 10:23:25.000000 recipe2txt-0.5/test/test_html2recipe.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     8090 2024-02-12 10:23:25.000000 recipe2txt-0.5/test/test_misc.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3088 2024-02-12 10:23:25.000000 recipe2txt-0.5/test/test_recipes2out.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     9835 2024-02-12 10:23:25.000000 recipe2txt-0.5/test/test_sql.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3389 2024-02-12 10:23:25.000000 recipe2txt-0.5/test/test_traceback_utils.py
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-04-01 20:30:48.742472 recipe2txt-0.5.1/
+-rw-rw-r--   0 pc        (1000) pc        (1000)    35149 2023-07-25 13:15:25.000000 recipe2txt-0.5.1/LICENSE
+-rw-r--r--   0 pc        (1000) pc        (1000)     9818 2024-04-01 20:30:48.742472 recipe2txt-0.5.1/PKG-INFO
+-rw-rw-r--   0 pc        (1000) pc        (1000)     8295 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/README.md
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3541 2024-04-01 20:29:15.000000 recipe2txt-0.5.1/pyproject.toml
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-04-01 20:30:48.734472 recipe2txt-0.5.1/recipe2txt/
+-rw-rw-r--   0 pc        (1000) pc        (1000)        0 2023-07-11 12:26:00.000000 recipe2txt-0.5.1/recipe2txt/__init__.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     7243 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/recipe2txt/fetcher.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3380 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/recipe2txt/fetcher_async.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    10409 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/recipe2txt/file_setup.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    15310 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/recipe2txt/html2recipe.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     9424 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/recipe2txt/parsing_error.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)        0 2023-03-10 13:56:18.000000 recipe2txt-0.5.1/recipe2txt/py.typed
+-rw-rw-r--   0 pc        (1000) pc        (1000)     2796 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/recipe2txt/re2txt.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     4044 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/recipe2txt/recipes2out.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    15720 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/recipe2txt/sql.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    10197 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/recipe2txt/user_interface.py
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-04-01 20:30:48.738472 recipe2txt-0.5.1/recipe2txt/utils/
+-rw-rw-r--   0 pc        (1000) pc        (1000)    18860 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/recipe2txt/utils/ArgConfig.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    11731 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/recipe2txt/utils/ContextLogger.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)        0 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/recipe2txt/utils/__init__.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     1259 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/recipe2txt/utils/conditional_imports.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    11029 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/recipe2txt/utils/filesystem.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     4320 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/recipe2txt/utils/markdown.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     6242 2024-04-01 18:59:04.000000 recipe2txt-0.5.1/recipe2txt/utils/misc.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3158 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/recipe2txt/utils/traceback_utils.py
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-04-01 20:30:48.738472 recipe2txt-0.5.1/recipe2txt.egg-info/
+-rw-r--r--   0 pc        (1000) pc        (1000)     9818 2024-04-01 20:30:48.000000 recipe2txt-0.5.1/recipe2txt.egg-info/PKG-INFO
+-rw-rw-r--   0 pc        (1000) pc        (1000)     1037 2024-04-01 20:30:48.000000 recipe2txt-0.5.1/recipe2txt.egg-info/SOURCES.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)        1 2024-04-01 20:30:48.000000 recipe2txt-0.5.1/recipe2txt.egg-info/dependency_links.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)       86 2024-04-01 20:30:48.000000 recipe2txt-0.5.1/recipe2txt.egg-info/entry_points.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)      219 2024-04-01 20:30:48.000000 recipe2txt-0.5.1/recipe2txt.egg-info/requires.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)       11 2024-04-01 20:30:48.000000 recipe2txt-0.5.1/recipe2txt.egg-info/top_level.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)       38 2024-04-01 20:30:48.742472 recipe2txt-0.5.1/setup.cfg
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-04-01 20:30:48.738472 recipe2txt-0.5.1/test/
+-rw-rw-r--   0 pc        (1000) pc        (1000)     8844 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/test/test4recipe2txt.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    17183 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/test/test_argconfig.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    15340 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/test/test_contextlogger.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3042 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/test/test_fetcher.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     5203 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/test/test_file_setup.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     6434 2024-04-01 20:25:12.000000 recipe2txt-0.5.1/test/test_filestystem.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     6174 2024-04-01 20:25:12.000000 recipe2txt-0.5.1/test/test_helpers.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     4635 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/test/test_html2recipe.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     2958 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/test/test_misc.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3094 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/test/test_recipes2out.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     9851 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/test/test_sql.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3389 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/test/test_traceback_utils.py
```

### Comparing `recipe2txt-0.5/LICENSE` & `recipe2txt-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5/PKG-INFO` & `recipe2txt-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recipe2txt
-Version: 0.5
+Version: 0.5.1
 Summary: Scrapes recipes and converts them to txt or markdown
 Author-email: Jan Philipp Berg <git.7ksst@aleeas.com>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://github.com/jp-berg/recipe2txt
 Project-URL: Bug Tracker, https://github.com/jp-berg/recipe2txt/issues
 Keywords: recipes,cooking,scraping,website
 Classifier: Programming Language :: Python :: 3
@@ -19,24 +19,25 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: recipe-scrapers~=14.54
-Requires-Dist: xdg-base-dirs~=6.0
-Requires-Dist: validators~=0.22
-Requires-Dist: jinja2~=3.1
-Requires-Dist: importlib-metadata~=7.0
+Requires-Dist: aiodns~=3.2
+Requires-Dist: aiohttp~=3.9
 Requires-Dist: backports.strenum~=1.2; python_version < "3.11"
-Requires-Dist: typing_extensions~=4.6.2; python_version < "3.11"
+Requires-Dist: importlib-metadata~=7.1
+Requires-Dist: jinja2~=3.1
+Requires-Dist: lxml==5.0.2
+Requires-Dist: recipe-scrapers~=14.55
 Requires-Dist: tomli~=2.0; python_version < "3.11"
-Requires-Dist: aiohttp~=3.9
-Requires-Dist: aiodns~=3.1
+Requires-Dist: typing_extensions~=4.6.2; python_version < "3.11"
+Requires-Dist: validators~=0.24
+Requires-Dist: xdg-base-dirs~=6.0
 
 # Introduction
 
 `recipe2txt` is a CLI-program that you can feed your urls of recipes and it spits out formatted cookbooks containing those recipes. Highlights include:
 
 * asynchronous fetching of recipes
 * formatted output either as txt- or markdown-file
```

### Comparing `recipe2txt-0.5/README.md` & `recipe2txt-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5/pyproject.toml` & `recipe2txt-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "recipe2txt"
-version = "0.5"
+version = "0.5.1"
 authors = [
   { name="Jan Philipp Berg", email="git.7ksst@aleeas.com" },
 ]
 description = "Scrapes recipes and converts them to txt or markdown"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "GNU General Public License v3 or later (GPLv3+)"}
@@ -31,24 +31,25 @@
     "Programming Language :: Python",
     "Topic :: Internet",
     "Topic :: Text Processing :: Markup :: Markdown",
     "Typing :: Typed"
 ]
 keywords = ["recipes", "cooking", "scraping", "website"]
 dependencies = [
-  "recipe-scrapers ~= 14.54",
-  "xdg-base-dirs ~= 6.0",
-  "validators ~= 0.22",
-  "jinja2 ~= 3.1",
-  "importlib-metadata ~= 7.0",
+  "aiodns ~= 3.2",
+  "aiohttp ~= 3.9",
   "backports.strenum ~= 1.2; python_version < '3.11'",
-  "typing_extensions ~= 4.6.2; python_version < '3.11'",
+  "importlib-metadata ~= 7.1",
+  "jinja2 ~= 3.1",
+  "lxml == 5.0.2",
+  "recipe-scrapers ~= 14.55",
   "tomli ~= 2.0; python_version < '3.11'",
-  "aiohttp ~= 3.9",
-  "aiodns ~= 3.1"
+  "typing_extensions ~= 4.6.2; python_version < '3.11'",
+  "validators ~= 0.24",
+  "xdg-base-dirs ~= 6.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/jp-berg/recipe2txt"
 "Bug Tracker" = "https://github.com/jp-berg/recipe2txt/issues"
 
 [project.scripts]
```

### Comparing `recipe2txt-0.5/recipe2txt/fetcher.py` & `recipe2txt-0.5.1/recipe2txt/fetcher.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5/recipe2txt/fetcher_async.py` & `recipe2txt-0.5.1/recipe2txt/fetcher_async.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5/recipe2txt/file_setup.py` & `recipe2txt-0.5.1/recipe2txt/file_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from pathlib import Path
 from shutil import rmtree
 from typing import Final, NamedTuple
 
 from xdg_base_dirs import xdg_config_home, xdg_data_home, xdg_state_home
 
 from recipe2txt.utils.ContextLogger import get_logger
-from recipe2txt.utils.misc import (
+from recipe2txt.utils.filesystem import (
     AccessibleDatabase,
     Directory,
     File,
     create_timestamped_dir,
     ensure_accessible_db_critical,
     ensure_accessible_file,
     ensure_accessible_file_critical,
```

### Comparing `recipe2txt-0.5/recipe2txt/html2recipe.py` & `recipe2txt-0.5.1/recipe2txt/html2recipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,18 +153,20 @@
     if len(t) > len(RECIPE_ATTRIBUTES):
         raise ValueError(
             f"Expected a Recipe-based tuple (length {len(t)},"
             f" but got something longer (length {len(RECIPE_ATTRIBUTES)})"
         )
     if None in t:
         tmp = list(t)
-        t = tuple([
-            tmp[i] if tmp[i] else getattr(UNINIT_RECIPE, RECIPE_ATTRIBUTES[i])
-            for i in range(len(tmp))
-        ])
+        t = tuple(
+            [
+                tmp[i] if tmp[i] else getattr(UNINIT_RECIPE, RECIPE_ATTRIBUTES[i])
+                for i in range(len(tmp))
+            ]
+        )
     return t
 
 
 ESSENTIAL: Final[list[LiteralString]] = ["ingredients", "instructions"]
 """names of attributes that are considered essential for the recipe"""
 
 ON_DISPLAY: Final[list[LiteralString]] = ESSENTIAL + [
```

### Comparing `recipe2txt-0.5/recipe2txt/parsing_error.py` & `recipe2txt-0.5.1/recipe2txt/parsing_error.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5/recipe2txt/re2txt.py` & `recipe2txt-0.5.1/recipe2txt/re2txt.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     init_database,
     init_logging,
     mutex_args,
     sancheck_args,
     strings2urls,
 )
 from recipe2txt.utils.ContextLogger import get_logger
-from recipe2txt.utils.misc import Counts, dict2str, ensure_accessible_file_critical
+from recipe2txt.utils.filesystem import ensure_accessible_file_critical
+from recipe2txt.utils.misc import Counts, dict2str
 
 try:
     from recipe2txt.fetcher_async import AsyncFetcher as Fetcher
 except ImportError:
     from recipe2txt.fetcher import (  # type: ignore[assignment] # isort: skip
         Fetcher as Fetcher,
     )
```

### Comparing `recipe2txt-0.5/recipe2txt/recipes2out.py` & `recipe2txt-0.5.1/recipe2txt/recipes2out.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
 from jinja2 import Environment, StrictUndefined
 
 from recipe2txt.file_setup import JINJA_TEMPLATE_DIR, get_template_files
 from recipe2txt.html2recipe import NA, Recipe
 from recipe2txt.utils import markdown
 from recipe2txt.utils.ContextLogger import get_logger
-from recipe2txt.utils.misc import File, ensure_accessible_file, get_all_dict
+from recipe2txt.utils.filesystem import File, ensure_accessible_file
+from recipe2txt.utils.misc import get_all_dict
 
 logger = get_logger(__name__)
 
 
 @cache
 def get_env() -> Environment:
     """
```

### Comparing `recipe2txt-0.5/recipe2txt/sql.py` & `recipe2txt-0.5.1/recipe2txt/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 
 from recipe2txt.utils.conditional_imports import LiteralString
 from recipe2txt.utils.ContextLogger import get_logger
 
 from .html2recipe import METHODS, NA, RECIPE_ATTRIBUTES, SCRAPER_VERSION, Recipe
 from .html2recipe import RecipeStatus as RS
 from .html2recipe import gen_status, int2status, none2na
-from .utils.misc import URL, AccessibleDatabase, File, head_str, obj2sql_str
+from .utils.filesystem import AccessibleDatabase, File
+from .utils.misc import URL, head_str, obj2sql_str
 
 logger = get_logger(__name__)
 """The logger for the module. Receives the constructed logger from 
 :py:mod:`recipe2txt.utils.ContextLogger`"""
 
 
 _CREATE_TABLES: Final = textwrap.dedent(
```

### Comparing `recipe2txt-0.5/recipe2txt/user_interface.py` & `recipe2txt-0.5.1/recipe2txt/user_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,16 @@
 from recipe2txt.utils.conditional_imports import tomllib
 from recipe2txt.utils.ContextLogger import (
     LOG_LEVEL_NAMES,
     STRING2LEVEL,
     get_logger,
     root_log_setup,
 )
-from recipe2txt.utils.misc import URL, Counts, File, extract_urls, read_files
+from recipe2txt.utils.filesystem import File, read_files
+from recipe2txt.utils.misc import URL, Counts, extract_urls
 
 try:
     from recipe2txt.fetcher_async import AsyncFetcher as Fetcher
 except ImportError:
     from recipe2txt.fetcher import (  # type: ignore[assignment] # isort: skip
         Fetcher as Fetcher,
     )
```

### Comparing `recipe2txt-0.5/recipe2txt/utils/ArgConfig.py` & `recipe2txt-0.5.1/recipe2txt/utils/ArgConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import sys
 import textwrap
 from enum import unique
 from pathlib import Path
 from typing import Any, Final, Generic, Iterable, Literal, TypeVar
 
 from recipe2txt.utils.conditional_imports import StrEnum, tomllib
-from recipe2txt.utils.misc import File, ensure_accessible_file_critical
+from recipe2txt.utils.filesystem import File, ensure_accessible_file_critical
 
 
 def short_flag(long_name: str) -> str:
     """
     Creates a shortened version of a long flag-name
 
     Uses the first letter of each word. Words should be separated by '-'.
```

### Comparing `recipe2txt-0.5/recipe2txt/utils/ContextLogger.py` & `recipe2txt-0.5.1/recipe2txt/utils/ContextLogger.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5/recipe2txt/utils/conditional_imports.py` & `recipe2txt-0.5.1/recipe2txt/utils/conditional_imports.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5/recipe2txt/utils/markdown.py` & `recipe2txt-0.5.1/recipe2txt/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5/recipe2txt/utils/misc.py` & `recipe2txt-0.5.1/recipe2txt/utils/filesystem.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,113 +9,59 @@
 # recipe2txt is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # recipe2txt. If not, see <https://www.gnu.org/licenses/>.
+"""
+Module offering additional functions for filesystem-interactions.
+"""
 import os
-import os.path
-import re
 import sqlite3
 import sys
-import urllib.parse
-from os import linesep
 from pathlib import Path
 from time import localtime, strftime
-from types import ModuleType
-from typing import Any, Final, NewType, TypeGuard
-
-import validators
+from typing import Any, NewType, TypeGuard
 
 from recipe2txt.utils.ContextLogger import DO_NOT_LOG, get_logger
 
-__all__ = [
-    "NEVER_CATCH",
-    "URL",
-    "is_url",
-    "extract_urls",
-    "File",
-    "is_file",
-    "Directory",
-    "is_dir",
-    "AccessibleDatabase",
-    "is_accessible_db",
-    "full_path",
-    "ensure_existence_dir",
-    "ensure_existence_dir_critical",
-    "create_timestamped_dir",
-    "ensure_accessible_file",
-    "ensure_accessible_file_critical",
-    "ensure_accessible_db_critical",
-    "read_files",
-    "Counts",
-    "dict2str",
-    "head_str",
-    "obj2sql_str",
-    "get_all_dict",
-]
-
 logger = get_logger(__name__)
 
-NEVER_CATCH: Final = (SystemExit, MemoryError, KeyboardInterrupt)
-
-URL = NewType("URL", str)
-
-
-def is_url(value: str) -> TypeGuard[URL]:
-    return bool(validators.url(value))
-
-
-def extract_urls(lines: list[str]) -> set[URL]:
-    processed: set[URL] = set()
-    for line in lines:
-        strings = line.split()
-        for string in strings:
-            tmp = string
-            if not string.startswith("http"):
-                string = "http://" + string
-            if is_url(string):
-                url = string
-
-                # Strip variables to avoid duplicating urls
-                parsed = urllib.parse.urlparse(url)
-                reconstructed = urllib.parse.urlunparse(
-                    (parsed.scheme, parsed.netloc, parsed.path, "", "", "")
-                )
-                url = reconstructed if is_url(reconstructed) else url
-
-                if url in processed:
-                    logger.warning("%s already queued", url)
-                else:
-                    processed.add(url)
-                    logger.info("Queued %s", url)
-            else:
-                logger.debug("Not an URL: %s", tmp)
-    return processed
-
-
 File = NewType("File", Path)
+"""
+Type representing a path to a file. The type states that the file has existed at the point in time the Path-type
+was narrowed to the File-type, but does not represent a guarantee that the file still exists at a later point in time.
+"""
 
 
-def is_file(value: Path) -> TypeGuard[File]:
+def real_file(value: Path) -> TypeGuard[File]:
+    """Checks if the file 'path' points to is an :py:data:`File`"""
     return value.is_file()
 
 
 Directory = NewType("Directory", Path)
+"""
+Type representing a path to a directory. The type states that the directory has existed at the point in time the
+Path-type was narrowed to the Directory-type, but does not represent a guarantee that the file still exists at a later
+point in time.
+"""
 
 
-def is_dir(value: Path) -> TypeGuard[Directory]:
+def real_dir(value: Path) -> TypeGuard[Directory]:
+    """Checks if the file 'path' points to is an :py:data:`Directory`"""
     return value.is_dir()
 
 
 AccessibleDatabase = NewType("AccessibleDatabase", Path)
-"""Type representing a database file, that was (at one point during program 
-execution) a valid and accessible
-Sqlite3-database"""
+"""
+Type representing a path to a sqlite3-database-file. The type states that the file has existed and represented a valid
+and accessible sqlite3-database-file at the point in time the Path-type was narrowed to the database-type, but does not 
+represent a guarantee that the file will hold those properties at a later point in time.
+"""
 
 
 def is_accessible_db(path: Path) -> TypeGuard[AccessibleDatabase]:
     """Checks if the file 'path' points to is an :py:data:`AccessibleDatabase`"""
     try:
         con = sqlite3.connect(path)
     except sqlite3.OperationalError:
@@ -129,14 +75,27 @@
     finally:
         cur.close()
         con.close()
     return True
 
 
 def full_path(*pathelements: str | Path) -> Path:
+    """
+    Creates an absolute path from pathelements
+
+    Will expand variables.
+    Will expand USER.
+    Will remove leading and trailing whitespace
+    Args:
+        *pathelements (): elements of the path to be formed (correctly ordered)
+
+    Returns:
+        An absolute path
+
+    """
     first = str(pathelements[0]).lstrip()
     last = str(pathelements[-1]).rstrip() if len(pathelements) > 1 else ""
 
     path = Path(first, *pathelements[1:-1], last)
     path = path.expanduser()
     path = Path(os.path.expandvars(path))
     path = path.resolve()
@@ -151,15 +110,15 @@
             return None, (
                 (
                     "%s is already a file, thus a directory with the same name cannot"
                     " exist"
                 ),
                 path,
             )
-        exists = is_dir(path)
+        exists = real_dir(path)
     except OSError as e:
         return None, (
             "Directory cannot be accessed: %s (%s)",
             path,
             getattr(e, "message", repr(e)),
         )
     if not exists:
@@ -172,32 +131,71 @@
                 path,
                 getattr(e, "message", repr(e)),
             )
     return Directory(path), (DO_NOT_LOG, "", "")
 
 
 def ensure_existence_dir(*path_elem: str | Path) -> Directory | None:
+    """
+    Constructs an absolute path from path_elem pointing to a directory
+
+    If the directory described by the path does not exist it will be created
+    Args:
+        *path_elem (): elements of the path to be formed (correctly ordered). The last will be the target directory
+
+    Returns:
+        An absolute path to an existing directory or None if the directory cannot be created
+    """
     path = full_path(*path_elem)
     directory, msg = _ensure_existence_dir(path)
     if not directory:
         if msg:
             logger.error(*msg)
     return directory
 
 
 def ensure_existence_dir_critical(*path_elem: str | Path) -> Directory:
+    """
+    Constructs an absolute path from path_elem pointing to a directory
+
+    If the directory described by the path does not exist it will be created
+    Args:
+        *path_elem (): elements of the path to be formed (correctly ordered). The last will be the target directory
+
+    Returns:
+        An absolute path to an existing directory
+
+    Raises:
+        SystemExit: When the directory does not exist and cannot be created
+
+    """
     path = full_path(*path_elem)
     directory, msg = _ensure_existence_dir(path)
     if not directory:
         logger.critical(*msg)
         sys.exit(os.EX_IOERR)
     return directory
 
 
 def create_timestamped_dir(*path_elem: str | Path, name: str = "") -> Directory | None:
+    """
+    Creates a directory at the tip of path_elem whose name is derived from the current time
+
+    The format for the name is 'YYYY-mm-DD_HH-MM-SS' if name is empty, otherwise name will be prepended
+    like this: 'NAME__YYYY-mm-DD_HH-MM-SS'.
+
+    Args:
+        *path_elem (): elements of the path pointing to the directory (correctly ordered)
+        name (): An optional name for the directory
+
+    Returns:
+        An absolute path to an existing directory with the current timestamp in its name or None if the directory could
+        not be created
+
+    """
     current_time = strftime("%Y-%m-%d_%H-%M-%S", localtime())
     parent = ensure_existence_dir(*path_elem)
     if not parent:
         return None
     dir_name = f"{name}__{current_time}" if name else current_time
     i = 1
     tmp = parent / dir_name
@@ -248,22 +246,49 @@
     with path.open("a") as f:
         if not f.writable():
             return None, ("File is not writable: %s", path)
     return File(path), (DO_NOT_LOG, "", "")
 
 
 def ensure_accessible_file(*path_elem: str | Path) -> File | None:
+    """
+    Constructs an absolute path from path_elem pointing to a file
+
+    If the file described by the path does not exist it will be created.
+    The file is readable and writeable by this program
+
+    Args:
+        *path_elem (): elements of the path to be formed (correctly ordered). The last will be the target file
+
+    Returns:
+        An absolute path to an existing, readable, writeable file
+
+    Raises:
+        SystemExit: When the path does not describe a readable/writable file and no such file can be created
+    """
     path = full_path(*path_elem)
     file, msg = _ensure_accessible_file(path)
     if not file:
         logger.error(*msg)
     return file
 
 
 def ensure_accessible_file_critical(*path_elem: str | Path) -> File:
+    """
+    Constructs an absolute path from path_elem pointing to a file
+
+    If the file described by the path does not exist it will be created.
+    The file is readable and writeable by this program
+
+    Args:
+        *path_elem (): elements of the path to be formed (correctly ordered). The last will be the target file
+
+    Returns:
+        An absolute path to an existing, readable, writeable file or None if no such file can be created/found
+    """
     path = full_path(*path_elem)
     file, msg = _ensure_accessible_file(path)
     if not file:
         logger.critical(*msg)
         sys.exit(os.EX_IOERR)
     return file
 
@@ -275,149 +300,43 @@
 
     Works like :py:function:`recipe2txt.utils.misc.ensure_accessible_file_critical`.
     Args:
         *path_elem: The elements from which a path should be constructed
     Returns:
         A path to a valid Sqlite3-database-file, which is accessible by this program
     Raises:
-        SystemExit: If the database-file cannot be created.
+        SystemExit: If the database-file cannot be found/created.
 
     """
     db_path = full_path(*path_elem)
     ensure_existence_dir_critical(db_path.parent)
     if is_accessible_db(db_path):
         db_file = db_path
     else:
         logger.critical("Database not accessible: %s", db_path)
         sys.exit(os.EX_IOERR)
     return db_file
 
 
 def read_files(*possible_paths: str | Path) -> list[str]:
+    """
+    Reads multiple files and concatenates their lines into a list of strings.
+
+    Paths that do not point to readable textfiles will be skipped.
+
+    Args:
+        *possible_paths (): Paths to potential text-files
+
+    Returns:
+        A list of strings, where each string represents a line from one file.
+
+    """
     lines = []
     for p in possible_paths:
         path = full_path(p)
         if path.is_file():
             logger.info("Reading %s", path)
-            path.read_text()
             with path.open("r") as file:
                 lines += list(file.readlines())
         else:
             logger.error("Not a file: %s", path)
     return lines
-
-
-class Counts:
-    def __init__(self) -> None:
-        self.strings: int = 0
-        self.urls: int = 0
-        self.require_fetching: int = 0
-        self.reached: int = 0
-        self.parsed_successfully: int = 0
-        self.parsed_partially: int = 0
-
-    def __str__(self) -> str:
-        s = linesep.join([
-            "[Absolute|Percentage of count above]",
-            "",
-            "Total number of strings: {}",
-            "Identified as URLs: [{}|{:.2f}%]",
-            "URLs not yet (fully) saved: [{}|{:.2f}%]",
-            "URLs reached: [{}|{:.2f}%]",
-            "Recipes parsed partially: [{}|{:.2f}%]",
-            "Recipes parsed fully: [{}|{:.2f}%]",
-            "",
-        ]).format(
-            self.strings,
-            self.urls,
-            (self.urls / self.strings) * 100,
-            self.require_fetching,
-            (self.require_fetching / self.urls) * 100,
-            self.reached,
-            (self.reached / self.urls) * 100,
-            self.parsed_partially,
-            (self.parsed_partially / self.urls) * 100,
-            self.parsed_successfully,
-            (self.parsed_successfully / self.urls) * 100,
-        )
-        return s
-
-
-def dict2str(dictionary: dict[Any, Any], sep: str = linesep) -> str:
-    items = [f"{item[0]}: {item[1]}" for item in dictionary.items()]
-    return sep.join(items)
-
-
-def head_str(o: Any, max_length: int = 50) -> str:
-    s = str(o)
-    if len(s) > max_length:
-        s = s[: max_length - 3].rstrip() + "..."
-    return s.replace(linesep, " ")
-
-
-_ONLY_ALPHANUM_DOT_UNDERSCORE: Final = re.compile(r"^[\w_\.]+$")
-
-
-def _sanitize(value: object) -> str:
-    string = str(value)
-    matches = _ONLY_ALPHANUM_DOT_UNDERSCORE.findall(string)
-    if len(matches) == 0:
-        raise ValueError(
-            "Strings used as identifiers in SQL-statements for this application"
-            " are only allowed to contain alphanumeric characters, dots and underscores"
-            f" (offending string : '{string}')"
-        )
-    if len(matches) > 1:
-        raise RuntimeError("This should not be possible")
-    return f'"{string}"'
-
-
-def obj2sql_str(*values: object) -> str:
-    """
-    Function preventing SQL-injection attacks from arbitrary values.
-
-    Since inserting arbitrary values into SQL-queries can lead to a SQL-injection
-    attack, this function disallows anything but alphanumeric characters, dots and
-    underscores.
-
-    Additionally, it wraps each string into double-quotes. This prevents SQLite
-    from executing any SQL-statement hidden inside the quotes, since the contained
-    characters can only be treated as strings and never as part of the statement.
-
-    Args:
-        *values (): One or more values
-
-    Returns:
-        'STRING' -> '"STRING"'
-        'STRING1', 'STRING2', 'STRING3' -> '"STRING1", "STRING2", "STRING3"'
-        'String_2' -> '"String_2"'
-        'String 2' -> RuntimeError
-        '); DROP TABLE recipes' -> RuntimeError
-
-    Raises:
-        RuntimeError: If characters other than alphanumeric ASCII-characters and
-            underscores are detected in strings.
-
-    """
-    sanitized = [_sanitize(value) for value in values]
-    return ", ".join(sanitized)
-
-
-def get_all_dict(mod: ModuleType) -> dict[str, Any]:
-    """
-    Builds a dictionary from the __all__-attribute of mod.
-
-    The keys are the strings in __all__ and the values are references to the
-    corresponding module-members (e.g. the functions, classes, variables declared in
-    that module)
-
-    Args:
-        mod (): A python module
-
-    Returns:
-        A dictionary filled with member-name|member-reference pairs or an empty
-        dictionary if the module does not declare __all__
-
-    """
-    if not (declared_items := mod.__dict__["__all__"]):
-        return {}
-    return {name: mod.__dict__[name] for name in declared_items}
```

### Comparing `recipe2txt-0.5/recipe2txt/utils/traceback_utils.py` & `recipe2txt-0.5.1/recipe2txt/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5/recipe2txt.egg-info/PKG-INFO` & `recipe2txt-0.5.1/recipe2txt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recipe2txt
-Version: 0.5
+Version: 0.5.1
 Summary: Scrapes recipes and converts them to txt or markdown
 Author-email: Jan Philipp Berg <git.7ksst@aleeas.com>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://github.com/jp-berg/recipe2txt
 Project-URL: Bug Tracker, https://github.com/jp-berg/recipe2txt/issues
 Keywords: recipes,cooking,scraping,website
 Classifier: Programming Language :: Python :: 3
@@ -19,24 +19,25 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: recipe-scrapers~=14.54
-Requires-Dist: xdg-base-dirs~=6.0
-Requires-Dist: validators~=0.22
-Requires-Dist: jinja2~=3.1
-Requires-Dist: importlib-metadata~=7.0
+Requires-Dist: aiodns~=3.2
+Requires-Dist: aiohttp~=3.9
 Requires-Dist: backports.strenum~=1.2; python_version < "3.11"
-Requires-Dist: typing_extensions~=4.6.2; python_version < "3.11"
+Requires-Dist: importlib-metadata~=7.1
+Requires-Dist: jinja2~=3.1
+Requires-Dist: lxml==5.0.2
+Requires-Dist: recipe-scrapers~=14.55
 Requires-Dist: tomli~=2.0; python_version < "3.11"
-Requires-Dist: aiohttp~=3.9
-Requires-Dist: aiodns~=3.1
+Requires-Dist: typing_extensions~=4.6.2; python_version < "3.11"
+Requires-Dist: validators~=0.24
+Requires-Dist: xdg-base-dirs~=6.0
 
 # Introduction
 
 `recipe2txt` is a CLI-program that you can feed your urls of recipes and it spits out formatted cookbooks containing those recipes. Highlights include:
 
 * asynchronous fetching of recipes
 * formatted output either as txt- or markdown-file
```

### Comparing `recipe2txt-0.5/recipe2txt.egg-info/SOURCES.txt` & `recipe2txt-0.5.1/recipe2txt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,23 @@
 recipe2txt.egg-info/entry_points.txt
 recipe2txt.egg-info/requires.txt
 recipe2txt.egg-info/top_level.txt
 recipe2txt/utils/ArgConfig.py
 recipe2txt/utils/ContextLogger.py
 recipe2txt/utils/__init__.py
 recipe2txt/utils/conditional_imports.py
+recipe2txt/utils/filesystem.py
 recipe2txt/utils/markdown.py
 recipe2txt/utils/misc.py
 recipe2txt/utils/traceback_utils.py
 test/test4recipe2txt.py
 test/test_argconfig.py
 test/test_contextlogger.py
 test/test_fetcher.py
 test/test_file_setup.py
+test/test_filestystem.py
 test/test_helpers.py
 test/test_html2recipe.py
 test/test_misc.py
 test/test_recipes2out.py
 test/test_sql.py
 test/test_traceback_utils.py
```

### Comparing `recipe2txt-0.5/test/test4recipe2txt.py` & `recipe2txt-0.5.1/test/test4recipe2txt.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from collections import OrderedDict
 from pathlib import Path
 from test.test_helpers import TEST_PROJECT_TMPDIR
 from typing import Final, Literal, TypeAlias, get_args
 
 from recipe2txt.file_setup import DB_NAME, DEBUG_DIRS, LOG_NAME
 from recipe2txt.utils.ContextLogger import LOG_LEVEL_NAMES
-from recipe2txt.utils.misc import (
+from recipe2txt.utils.filesystem import (
     Directory,
     create_timestamped_dir,
     ensure_accessible_file_critical,
 )
 
 
 def escape_whitespace(element: str) -> str:
```

### Comparing `recipe2txt-0.5/test/test_argconfig.py` & `recipe2txt-0.5.1/test/test_argconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from recipe2txt.file_setup import (
     CONFIG_NAME,
     DEBUG_DIRECTORY_BASE,
     DEBUG_DIRS,
     get_default_output,
 )
 from recipe2txt.user_interface import config_args
-from recipe2txt.utils.misc import ensure_accessible_file, ensure_existence_dir
+from recipe2txt.utils.filesystem import ensure_accessible_file, ensure_existence_dir
 
 
 class TestFunctions(unittest.TestCase):
     def test_short_flag(self):
         parameter = [
             ("--verbose", "-v"),
             ("--file", "-f"),
```

### Comparing `recipe2txt-0.5/test/test_contextlogger.py` & `recipe2txt-0.5.1/test/test_contextlogger.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import unittest
 from test.test_helpers import TEST_PROJECT_TMPDIR, assertFilesEqual
 from test.testfiles.permanent.gen_log import gen_logs, log_paths
 from typing import Any, Final, TypeVar
 
 import recipe2txt.utils.ContextLogger as CTXL
 from recipe2txt.utils.conditional_imports import LiteralString
-from recipe2txt.utils.misc import File
+from recipe2txt.utils.filesystem import File
 
 level = logging.WARNING
 test_msg = "THIS IS A TESTMESSAGE"
 context_msg = "context_msg: %s %s %s"
 context_args = ("This", "is", "a message")
 
 
@@ -401,10 +401,16 @@
 
 class TestAll(unittest.TestCase):
     def test_logging(self):
         test_path = TEST_PROJECT_TMPDIR / "logfiles"
         if test_path.is_dir():
             shutil.rmtree(test_path)
         test_paths: list[File] = gen_logs(test_path)
+        self.assertEqual(len(log_paths), 5)
+        for i in range(len(log_paths) - 1):
+            with self.subTest(greater=log_paths[i], smaller=log_paths[i + 1]):
+                self.assertTrue(
+                    log_paths[i].stat().st_size > log_paths[i + 1].stat().st_size
+                )
         for test, validation in zip(test_paths, log_paths):
             with self.subTest(msg=f"While testing {test.name}"):
                 assertFilesEqual(self, test, validation)
```

### Comparing `recipe2txt-0.5/test/test_fetcher.py` & `recipe2txt-0.5.1/test/test_fetcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 import unittest
 from test.test_helpers import TEST_PROJECT_TMPDIR, create_tmpdirs, delete_tmpdirs
 from test.test_sql import db_path, out_name_md, out_name_txt, out_path_txt
 from typing import Final
 
 from recipe2txt.fetcher import Cache, Fetcher
 from recipe2txt.sql import Database
-from recipe2txt.utils.misc import URL, ensure_accessible_file, is_accessible_db
+from recipe2txt.utils.filesystem import ensure_accessible_file, is_accessible_db
+from recipe2txt.utils.misc import URL
 
 
 class TestFileFetcher(Fetcher):
     URL2HTML: Final[dict[str, bytes]] = {
         url: html for url, html in zip(file_gen.URL_LIST, file_gen.HTML_LIST)
     }
```

### Comparing `recipe2txt-0.5/test/test_file_setup.py` & `recipe2txt-0.5.1/test/test_file_setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import os.path
 import unittest
 from shutil import rmtree
 from test.test_helpers import TEST_PROJECT_TMPDIR, TESTFILE, assertAccessibleFile
 
 import recipe2txt.file_setup as fs
 from recipe2txt.utils.ContextLogger import disable_loggers
-from recipe2txt.utils.misc import (
+from recipe2txt.utils.filesystem import (
     ensure_accessible_file_critical,
     ensure_existence_dir,
     is_accessible_db,
 )
 
 copy_debug_dirs = fs.DEBUG_DIRS
 tmp_data_dir = TEST_PROJECT_TMPDIR / "test-xdg-dirs"
```

### Comparing `recipe2txt-0.5/test/test_helpers.py` & `recipe2txt-0.5.1/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5/test/test_html2recipe.py` & `recipe2txt-0.5.1/test/test_html2recipe.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5/test/test_misc.py` & `recipe2txt-0.5.1/test/test_filestystem.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,74 +9,52 @@
 # recipe2txt is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # recipe2txt. If not, see <https://www.gnu.org/licenses/>.
-
 import os
 import shutil
 import unittest
 from pathlib import Path
 from test.test_helpers import (
     NONE_DIRS,
     NORMAL_DIRS,
-    TEST_FILEDIR,
     TEST_PROJECT_TMPDIR,
     TESTFILE,
     XDG_TMPDIR,
     assertAccessibleFile,
     create_tmpdirs,
     delete_tmpdirs,
 )
 from test.test_sql import db_name, db_paths
 
-from recipe2txt.utils import misc
+from recipe2txt.utils import filesystem
 
 
 class FileTests(unittest.TestCase):
     def setUp(self) -> None:
         if not create_tmpdirs():
             self.fail()
 
     def tearDown(self) -> None:
         if not delete_tmpdirs():
             self.fail()
 
     def test_is_accessible_db(self):
         for path in db_paths:
             with self.subTest(path=path):
-                self.assertTrue(misc.is_accessible_db(path))
+                self.assertTrue(filesystem.is_accessible_db(path))
 
         db_path_inaccessible = os.path.join("/root", db_name)
-        self.assertFalse(misc.is_accessible_db(db_path_inaccessible))
+        self.assertFalse(filesystem.is_accessible_db(db_path_inaccessible))
 
         db_path_nonexistent = os.path.join(TEST_PROJECT_TMPDIR, "NOT_A_FOLDER", db_name)
-        self.assertFalse(misc.is_accessible_db(db_path_nonexistent))
-
-    def test_extract_urls(self):
-        obscured_urls = TEST_FILEDIR / "permanent" / "obscured_urls.txt"
-        unobscured_urls = obscured_urls.with_name("unobscured_urls.txt")
-        if not obscured_urls.is_file():
-            self.fail(f"{obscured_urls} does not exist.")
-        if not unobscured_urls.is_file():
-            self.fail(f"{unobscured_urls} does not exist.")
-
-        validation = set()
-        for url in misc.read_files(unobscured_urls):
-            if url := url.strip():
-                validation.add(url)
-
-        lines = misc.read_files(obscured_urls)
-        urls = misc.extract_urls(lines)
-        if diff := validation - urls:
-            self.fail(f"Validation contains URLs that were not extracted:{diff}")
-        if diff := urls - validation:
-            self.fail(f"Validation does not contain URLs that were extracted:{diff}")
+        self.assertFalse(filesystem.is_accessible_db(db_path_nonexistent))
 
     def test_full_path(self):
         params = [
             (
                 ["~", "Documents", "File1"],
                 os.path.expanduser(os.path.join("~", "Documents", "File1")),
             ),
@@ -97,37 +75,41 @@
                 ["/home", "user", Path("Documents", "important"), "file1.txt"],
                 os.path.join("/home", "user", "Documents", "important", "file1.txt"),
             ),
         ]
 
         for test, validation in params:
             with self.subTest(testdata=test):
-                self.assertEqual(str(misc.full_path(*test)), validation)
+                self.assertEqual(str(filesystem.full_path(*test)), validation)
 
     def test_ensure_existence_dir(self):
         params_path = [(test, os.path.join(*test)) for test in NORMAL_DIRS]
 
         for test, validation in params_path:
             with self.subTest(testpath=test):
                 self.assertTrue(
-                    os.path.samefile(misc.ensure_existence_dir(*test), validation)
+                    os.path.samefile(
+                        filesystem.ensure_existence_dir(*test),
+                        validation,
+                    )
                 )
                 os.removedirs(validation)
 
         for test in NONE_DIRS:
             with self.subTest(directory=test):
-                self.assertIsNone(misc.ensure_existence_dir(*test))
+                self.assertIsNone(filesystem.ensure_existence_dir(*test))
 
     def test_ensure_accessible_file(self):
         params_path = [(test, os.path.join(*test, TESTFILE)) for test in NORMAL_DIRS]
         for test, validation in params_path:
             with self.subTest(directory=test):
                 self.assertTrue(
                     os.path.samefile(
-                        misc.ensure_accessible_file(*test, TESTFILE), validation
+                        filesystem.ensure_accessible_file(*test, TESTFILE),
+                        validation,
                     )
                 )
                 if not os.path.isfile(validation):
                     self.fail(f"File {validation} was not created")
                 try:
                     with open(validation, "w") as file:
                         file.write("TEST")
@@ -138,81 +120,51 @@
                     self.fail(e)
 
                 os.remove(validation)
                 os.rmdir(validation := os.path.dirname(validation))
                 os.rmdir(os.path.dirname(validation))
 
         for test in NONE_DIRS:
-            self.assertIsNone(misc.ensure_accessible_file(*test, TESTFILE))
+            self.assertIsNone(filesystem.ensure_accessible_file(*test, TESTFILE))
 
     def test_ensure_critical(self):
         crit_fail_path = NONE_DIRS[1]
 
         with self.assertRaises(SystemExit) as e:
-            misc.ensure_existence_dir_critical(*crit_fail_path)
+            filesystem.ensure_existence_dir_critical(*crit_fail_path)
         self.assertEqual(e.exception.code, os.EX_IOERR)
 
         with self.assertRaises(SystemExit) as e:
-            misc.ensure_accessible_file_critical(*crit_fail_path, TESTFILE)
+            filesystem.ensure_accessible_file_critical(*crit_fail_path, TESTFILE)
         self.assertEqual(e.exception.code, os.EX_IOERR)
 
     def test_read_files(self):
         file1_content = ["one", "two", "three", "four"]
         file2_content = ["five", "six", "seven", "eight"]
 
         file1_path = TEST_PROJECT_TMPDIR / "testfile1.txt"
         file2_path = XDG_TMPDIR / "testfile2.txt"
         file_notafile_path = TEST_PROJECT_TMPDIR / "NOTAFILE"
 
         file1_path.write_text(os.linesep.join(file1_content) + os.linesep)
         file2_path.write_text(os.linesep.join(file2_content) + os.linesep)
 
-        str_list = misc.read_files(file1_path, file_notafile_path, file2_path)
+        str_list = filesystem.read_files(file1_path, file_notafile_path, file2_path)
 
         for test, validation in zip(str_list, (file1_content + file2_content)):
             with self.subTest(validation_line=validation):
                 self.assertEqual(test.rstrip(), validation)
 
         os.remove(file1_path)
         os.remove(file2_path)
 
     def test_dir_file_name_conflict(self):
-        directory = misc.full_path(*NORMAL_DIRS[0])
+        directory = filesystem.full_path(*NORMAL_DIRS[0])
         os.makedirs(directory, exist_ok=True)
 
-        self.assertIsNone(misc.ensure_accessible_file(directory))
+        self.assertIsNone(filesystem.ensure_accessible_file(directory))
         shutil.rmtree(directory)
-        assertAccessibleFile(self, misc.ensure_accessible_file(directory))
+        assertAccessibleFile(self, filesystem.ensure_accessible_file(directory))
 
-        self.assertIsNone(misc.ensure_existence_dir(directory))
+        self.assertIsNone(filesystem.ensure_existence_dir(directory))
         os.remove(directory)
-        self.assertTrue(misc.ensure_existence_dir(directory).is_dir())
-
-
-class StrTests(unittest.TestCase):
-    def test_dict2str(self):
-        dicts = [
-            (
-                {1: "one", 2: "two", 3: "three"},
-                os.linesep.join(["1: one", "2: two", "3: three"]),
-            ),
-            (
-                {"one": "Eins", "two": "Zwei", "three": "Drei"},
-                os.linesep.join(["one: Eins", "two: Zwei", "three: Drei"]),
-            ),
-        ]
-
-        for d, validation in dicts:
-            with self.subTest(testdict=d):
-                self.assertEqual(misc.dict2str(d), validation)
-
-    def test_head_str(self):
-        objects = [
-            ("teststringteststringteststring", "teststr..."),
-            ("teststring", "teststring"),
-            ("test       ", "test..."),
-            ([1, 2, 3, 4, 5, 6, 7, 8, 9, 10], "[1, 2,..."),
-        ]
-
-        for obj, validation in objects:
-            with self.subTest(testobj=obj):
-                self.assertEqual(misc.head_str(obj, 10), validation)
+        self.assertTrue(filesystem.ensure_existence_dir(directory).is_dir())
```

### Comparing `recipe2txt-0.5/test/test_recipes2out.py` & `recipe2txt-0.5.1/test/test_recipes2out.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     MD_LIST,
     RECIPE_LIST,
     TXT_LIST,
 )
 
 from recipe2txt.recipes2out import RecipeWriter
 from recipe2txt.utils.ContextLogger import suppress_logging
-from recipe2txt.utils.misc import ensure_accessible_file_critical
+from recipe2txt.utils.filesystem import ensure_accessible_file_critical
 
 TESTFILE_MD = TESTFILE.replace("txt", "md")
 
 
 class Test(unittest.TestCase):
 
     def tearDown(self) -> None:
```

### Comparing `recipe2txt-0.5/test/test_sql.py` & `recipe2txt-0.5.1/test/test_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     create_tmpdirs,
     delete_tmpdirs,
     test_recipes,
 )
 
 import recipe2txt.html2recipe as h2r
 import recipe2txt.sql as sql
-import recipe2txt.utils.misc as misc
+from recipe2txt.utils.filesystem import File, is_accessible_db
 
 db_name = "db_test.sqlite3"
 out_name = "out"
 out_name_txt = out_name + ".txt"
 out_name_md = out_name + ".md"
 
 db_path = TEST_PROJECT_TMPDIR / db_name
@@ -136,16 +136,16 @@
             print("Could not delete tmpdirs:", TMPDIRS, file=sys.stderr)
 
     def __init__(self, methodName="runTest"):
         super().__init__(methodName)
         self.db = None
 
     def setUp(self) -> None:
-        if misc.is_accessible_db(db_path):
-            self.db = sql.Database(db_path, misc.File(out_path_txt))
+        if is_accessible_db(db_path):
+            self.db = sql.Database(db_path, File(out_path_txt))
             for recipe in test_recipes:
                 with self.subTest(recipe=recipe.url):
                     try:
                         self.db.new_recipe(recipe)
                     except sqlite3.OperationalError:
                         self.fail("ERROR")
         else:
```

### Comparing `recipe2txt-0.5/test/test_traceback_utils.py` & `recipe2txt-0.5.1/test/test_traceback_utils.py`

 * *Files identical despite different names*

