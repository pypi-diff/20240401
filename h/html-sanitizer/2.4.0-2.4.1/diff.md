# Comparing `tmp/html_sanitizer-2.4.0.tar.gz` & `tmp/html_sanitizer-2.4.1.tar.gz`

## Comparing `html_sanitizer-2.4.0.tar` & `html_sanitizer-2.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 html_sanitizer-2.4.0/.editorconfig
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 html_sanitizer-2.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 html_sanitizer-2.4.0/CHANGELOG.rst
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 html_sanitizer-2.4.0/tox.ini
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 html_sanitizer-2.4.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 html_sanitizer-2.4.0/html_sanitizer/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 html_sanitizer-2.4.0/html_sanitizer/__main__.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 html_sanitizer-2.4.0/html_sanitizer/django.py
--rw-r--r--   0        0        0    13787 2020-02-02 00:00:00.000000 html_sanitizer-2.4.0/html_sanitizer/sanitizer.py
--rw-r--r--   0        0        0    24288 2020-02-02 00:00:00.000000 html_sanitizer-2.4.0/html_sanitizer/tests.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 html_sanitizer-2.4.0/.gitignore
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 html_sanitizer-2.4.0/LICENSE
--rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 html_sanitizer-2.4.0/README.rst
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 html_sanitizer-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     7898 2020-02-02 00:00:00.000000 html_sanitizer-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/.editorconfig
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/CHANGELOG.rst
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/tox.ini
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/html_sanitizer/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/html_sanitizer/__main__.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/html_sanitizer/django.py
+-rw-r--r--   0        0        0    13787 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/html_sanitizer/sanitizer.py
+-rw-r--r--   0        0        0    24288 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/html_sanitizer/tests.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/.gitignore
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/LICENSE
+-rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/README.rst
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7924 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/PKG-INFO
```

### Comparing `html_sanitizer-2.4.0/.pre-commit-config.yaml` & `html_sanitizer-2.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.0/CHANGELOG.rst` & `html_sanitizer-2.4.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.0/.github/workflows/test.yml` & `html_sanitizer-2.4.1/.github/workflows/test.yml`

 * *Files 3% similar despite different names*

```diff
@@ -18,12 +18,12 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install beautifulsoup4 lxml[html_clean]
+          python -m pip install beautifulsoup4 lxml lxml-html-clean
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
       - name: Run tests
         run: |
           python -m unittest discover -v
```

### Comparing `html_sanitizer-2.4.0/html_sanitizer/django.py` & `html_sanitizer-2.4.1/html_sanitizer/django.py`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.0/html_sanitizer/sanitizer.py` & `html_sanitizer-2.4.1/html_sanitizer/sanitizer.py`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.0/html_sanitizer/tests.py` & `html_sanitizer-2.4.1/html_sanitizer/tests.py`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.0/LICENSE` & `html_sanitizer-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.0/README.rst` & `html_sanitizer-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.0/pyproject.toml` & `html_sanitizer-2.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,16 @@
   "Topic :: Software Development",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   "beautifulsoup4",
-  "lxml[html_clean]>=5.2.0",
+  "lxml>=5.2.0",
+  "lxml-html-clean>=0.1.0",
 ]
 [project.urls]
 Homepage = "https://github.com/matthiask/html-sanitizer/"
 
 [tool.hatch.version]
 path = "html_sanitizer/__init__.py"
```

### Comparing `html_sanitizer-2.4.0/PKG-INFO` & `html_sanitizer-2.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html-sanitizer
-Version: 2.4.0
+Version: 2.4.1
 Summary: HTML sanitizer
 Project-URL: Homepage, https://github.com/matthiask/html-sanitizer/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -19,15 +19,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Requires-Dist: beautifulsoup4
-Requires-Dist: lxml[html-clean]>=5.2.0
+Requires-Dist: lxml-html-clean>=0.1.0
+Requires-Dist: lxml>=5.2.0
 Description-Content-Type: text/x-rst
 
 ==============
 HTML sanitizer
 ==============
 
 This is a allowlist-based and very opinionated HTML sanitizer that
```

