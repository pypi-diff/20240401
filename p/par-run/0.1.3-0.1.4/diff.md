# Comparing `tmp/par_run-0.1.3.tar.gz` & `tmp/par_run-0.1.4.tar.gz`

## Comparing `par_run-0.1.3.tar` & `par_run-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 par_run-0.1.3/.python-version
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 par_run-0.1.3/commands.ini
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 par_run-0.1.3/requirements-dev.lock
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 par_run-0.1.3/requirements.lock
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/.gitignore
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/coverage_html.js
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/d_417a353b6036f046___init___py.html
--rw-r--r--   0        0        0    78275 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/d_417a353b6036f046_cli_py.html
--rw-r--r--   0        0        0   106323 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/d_417a353b6036f046_executor_py.html
--rw-r--r--   0        0        0    46396 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/d_417a353b6036f046_web_cli_py.html
--rw-r--r--   0        0        0    23925 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/d_417a353b6036f046_web_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/favicon_32.png
--rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/keybd_open.png
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/status.json
--rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 par_run-0.1.3/.reports/html/style.css
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 par_run-0.1.3/.vscode/launch.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 par_run-0.1.3/py_tests/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 par_run-0.1.3/py_tests/conftest.py
--rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 par_run-0.1.3/py_tests/test_cli.py
--rw-r--r--   0        0        0    13799 2020-02-02 00:00:00.000000 par_run-0.1.3/py_tests/test_executor.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 par_run-0.1.3/py_tests/test_main.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 par_run-0.1.3/py_tests/test_web.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 par_run-0.1.3/src/par_run/__init__.py
--rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 par_run-0.1.3/src/par_run/cli.py
--rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 par_run-0.1.3/src/par_run/executor.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 par_run-0.1.3/src/par_run/web.py
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 par_run-0.1.3/src/par_run/static/css/style.css
--rw-r--r--   0        0        0     8623 2020-02-02 00:00:00.000000 par_run-0.1.3/src/par_run/static/js/app.js
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 par_run-0.1.3/src/par_run/templates/index.html
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 par_run-0.1.3/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 par_run-0.1.3/LICENSE
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 par_run-0.1.3/README.md
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 par_run-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 par_run-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 par_run-0.1.4/.python-version
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 par_run-0.1.4/commands.ini
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 par_run-0.1.4/requirements-dev.lock
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 par_run-0.1.4/requirements.lock
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/coverage_html.js
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/d_417a353b6036f046___init___py.html
+-rw-r--r--   0        0        0    78275 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/d_417a353b6036f046_cli_py.html
+-rw-r--r--   0        0        0   106323 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/d_417a353b6036f046_executor_py.html
+-rw-r--r--   0        0        0    46396 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/d_417a353b6036f046_web_cli_py.html
+-rw-r--r--   0        0        0    23925 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/d_417a353b6036f046_web_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/favicon_32.png
+-rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/keybd_open.png
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/status.json
+-rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 par_run-0.1.4/.reports/html/style.css
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 par_run-0.1.4/.vscode/launch.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 par_run-0.1.4/py_tests/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 par_run-0.1.4/py_tests/conftest.py
+-rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 par_run-0.1.4/py_tests/test_cli.py
+-rw-r--r--   0        0        0    13799 2020-02-02 00:00:00.000000 par_run-0.1.4/py_tests/test_executor.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 par_run-0.1.4/py_tests/test_main.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 par_run-0.1.4/py_tests/test_web.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 par_run-0.1.4/src/par_run/__init__.py
+-rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 par_run-0.1.4/src/par_run/cli.py
+-rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 par_run-0.1.4/src/par_run/executor.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 par_run-0.1.4/src/par_run/web.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 par_run-0.1.4/src/par_run/static/css/style.css
+-rw-r--r--   0        0        0     8623 2020-02-02 00:00:00.000000 par_run-0.1.4/src/par_run/static/js/app.js
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 par_run-0.1.4/src/par_run/templates/index.html
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 par_run-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 par_run-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 par_run-0.1.4/README.md
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 par_run-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 par_run-0.1.4/PKG-INFO
```

### Comparing `par_run-0.1.3/requirements-dev.lock` & `par_run-0.1.4/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/requirements.lock` & `par_run-0.1.4/requirements.lock`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/.reports/html/coverage_html.js` & `par_run-0.1.4/.reports/html/coverage_html.js`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/.reports/html/d_417a353b6036f046___init___py.html` & `par_run-0.1.4/.reports/html/d_417a353b6036f046___init___py.html`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/.reports/html/d_417a353b6036f046_cli_py.html` & `par_run-0.1.4/.reports/html/d_417a353b6036f046_cli_py.html`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/.reports/html/d_417a353b6036f046_executor_py.html` & `par_run-0.1.4/.reports/html/d_417a353b6036f046_executor_py.html`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/.reports/html/d_417a353b6036f046_web_cli_py.html` & `par_run-0.1.4/.reports/html/d_417a353b6036f046_web_cli_py.html`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/.reports/html/d_417a353b6036f046_web_py.html` & `par_run-0.1.4/.reports/html/d_417a353b6036f046_web_py.html`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/.reports/html/favicon_32.png` & `par_run-0.1.4/.reports/html/favicon_32.png`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/.reports/html/index.html` & `par_run-0.1.4/.reports/html/index.html`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/.reports/html/keybd_closed.png` & `par_run-0.1.4/.reports/html/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/.reports/html/keybd_open.png` & `par_run-0.1.4/.reports/html/keybd_open.png`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/.reports/html/status.json` & `par_run-0.1.4/.reports/html/status.json`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/.reports/html/style.css` & `par_run-0.1.4/.reports/html/style.css`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/.vscode/launch.json` & `par_run-0.1.4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/py_tests/conftest.py` & `par_run-0.1.4/py_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/py_tests/test_cli.py` & `par_run-0.1.4/py_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/py_tests/test_executor.py` & `par_run-0.1.4/py_tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/py_tests/test_web.py` & `par_run-0.1.4/py_tests/test_web.py`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/src/par_run/cli.py` & `par_run-0.1.4/src/par_run/cli.py`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/src/par_run/executor.py` & `par_run-0.1.4/src/par_run/executor.py`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/src/par_run/web.py` & `par_run-0.1.4/src/par_run/web.py`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/src/par_run/static/css/style.css` & `par_run-0.1.4/src/par_run/static/css/style.css`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/src/par_run/static/js/app.js` & `par_run-0.1.4/src/par_run/static/js/app.js`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/src/par_run/templates/index.html` & `par_run-0.1.4/src/par_run/templates/index.html`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/.gitignore` & `par_run-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/LICENSE` & `par_run-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/README.md` & `par_run-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `par_run-0.1.3/pyproject.toml` & `par_run-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 [project]
 name = "par-run"
-version = "0.1.3"
+version = "0.1.4"
 description = "Parallel command runner"
 license = "MIT"
 authors = [
     { name = "Naz Quadri", email = "naz.quadri@gmail.com" }
 ]
 classifiers = [
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
 ]
 dependencies = [
     "rich>=13.0.0",
@@ -75,15 +73,15 @@
 packages = [
     "src/par_run",
     "static",
     "templates",
 ]
 
 [tool.bumpversion]
-current_version = "0.1.3"
+current_version = "0.1.4"
 commit = true
 tag = true
 tag_name = "{new_version}"
 tag_message = "Version {new_version}"
 message = "Bump version: {current_version} → {new_version}"
 allow_dirty = true
 parse = """(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"""
```

### Comparing `par_run-0.1.3/PKG-INFO` & `par_run-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.3
 Name: par-run
-Version: 0.1.3
+Version: 0.1.4
 Summary: Parallel command runner
 Project-URL: Homepage, https://github.com/nazq/par-run
 Project-URL: Documentation, https://github.com/nazq/par-run
 Project-URL: Repository, https://github.com/nazq/par-run
 Project-URL: Issues, https://github.com/nazq/par-run/issues
 Project-URL: Changelog, https://github.com/nazq/par-run
 Author-email: Naz Quadri <naz.quadri@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: rich>=13.0.0
```

