# Comparing `tmp/edx-auth-backends-4.2.0.tar.gz` & `tmp/edx-auth-backends-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-auth-backends-4.2.0.tar", last modified: Thu Aug  3 13:34:59 2023, max compression
+gzip compressed data, was "edx-auth-backends-4.3.0.tar", last modified: Mon Apr  1 14:47:09 2024, max compression
```

## Comparing `edx-auth-backends-4.2.0.tar` & `edx-auth-backends-4.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:34:59.550680 edx-auth-backends-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-08-03 13:34:35.000000 edx-auth-backends-4.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)     1909 2023-08-03 13:34:35.000000 edx-auth-backends-4.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2555 2023-08-03 13:34:35.000000 edx-auth-backends-4.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-08-03 13:34:35.000000 edx-auth-backends-4.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-08-03 13:34:35.000000 edx-auth-backends-4.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10855 2023-08-03 13:34:59.550680 edx-auth-backends-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7425 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:34:59.546679 edx-auth-backends-4.2.0/auth_backends/
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5108 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)     3216 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:34:59.550680 edx-auth-backends-4.2.0/auth_backends/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2245 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/tests/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)     6457 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     2269 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/tests/test_strategies.py
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)      463 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:34:59.550680 edx-auth-backends-4.2.0/edx_auth_backends.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10855 2023-08-03 13:34:59.000000 edx-auth-backends-4.2.0/edx_auth_backends.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-08-03 13:34:59.000000 edx-auth-backends-4.2.0/edx_auth_backends.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 13:34:59.000000 edx-auth-backends-4.2.0/edx_auth_backends.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-08-03 13:34:59.000000 edx-auth-backends-4.2.0/edx_auth_backends.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-08-03 13:34:59.000000 edx-auth-backends-4.2.0/edx_auth_backends.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:34:59.550680 edx-auth-backends-4.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-08-03 13:34:59.550680 edx-auth-backends-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:47:09.240428 edx-auth-backends-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35136 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11069 2024-04-01 14:47:09.240428 edx-auth-backends-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:47:09.236428 edx-auth-backends-4.3.0/auth_backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/auth_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/auth_backends/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/auth_backends/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/auth_backends/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:47:09.236428 edx-auth-backends-4.3.0/auth_backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/auth_backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/auth_backends/tests/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/auth_backends/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/auth_backends/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/auth_backends/tests/test_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/auth_backends/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/auth_backends/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/auth_backends/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:47:09.240428 edx-auth-backends-4.3.0/edx_auth_backends.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11069 2024-04-01 14:47:09.000000 edx-auth-backends-4.3.0/edx_auth_backends.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-01 14:47:09.000000 edx-auth-backends-4.3.0/edx_auth_backends.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:47:09.000000 edx-auth-backends-4.3.0/edx_auth_backends.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-01 14:47:09.000000 edx-auth-backends-4.3.0/edx_auth_backends.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 14:47:09.000000 edx-auth-backends-4.3.0/edx_auth_backends.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:47:09.240428 edx-auth-backends-4.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-01 14:47:09.240428 edx-auth-backends-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-01 14:47:05.000000 edx-auth-backends-4.3.0/setup.py
```

### Comparing `edx-auth-backends-4.2.0/CHANGELOG.rst` & `edx-auth-backends-4.3.0/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,26 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
 *
 
+Added
+~~~~~~~
+
+[4.3.0] - 2024-04-01
+--------------------
+
+* Added support for python3.11 and 3.12
+* Dropped django 3.2 support.
+
 [4.2.0] - 2023-08-03
 --------------------
 
-Added
-~~~~~~~
 * Added support for Django 4.2
 
 [4.1.0] - 2022-01-28
 --------------------
 
 Removed
 ~~~~~~~
```

### Comparing `edx-auth-backends-4.2.0/HISTORY.rst` & `edx-auth-backends-4.3.0/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.2.0/LICENSE.txt` & `edx-auth-backends-4.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.2.0/PKG-INFO` & `edx-auth-backends-4.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: edx-auth-backends
-Version: 4.2.0
+Version: 4.3.0
 Summary: Custom edX authentication backends and pipeline steps
 Home-page: https://github.com/openedx/auth-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Keywords: authentication edx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet
 License-File: LICENSE.txt
 License-File: AUTHORS
+Requires-Dist: Django
+Requires-Dist: pyjwt[crypto]>=2.1.0
+Requires-Dist: six
+Requires-Dist: social-auth-app-django
+Requires-Dist: social-auth-core
 
 auth-backends  |CI|_ |Codecov|_
 ===================================
 .. |CI| image:: https://github.com/openedx/auth-backends/workflows/Python%20CI/badge.svg?branch=master
 .. _CI: https://github.com/openedx/auth-backends/actions?query=workflow%3A%22Python+CI%22
 
 .. |Codecov| image:: http://codecov.io/github/edx/auth-backends/coverage.svg?branch=master
@@ -158,15 +164,15 @@
 Contributions are very welcome!
 
 Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Mailing List and IRC Channel
 ----------------------------
 
 You can discuss this code on the `edx-code Google Group <https://groups.google.com/forum/#!forum/edx-code>`_ or in the
 ``#edx-code`` IRC channel on Freenode.
```

### Comparing `edx-auth-backends-4.2.0/README.rst` & `edx-auth-backends-4.3.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,14 @@
 Contributions are very welcome!
 
 Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Mailing List and IRC Channel
 ----------------------------
 
 You can discuss this code on the `edx-code Google Group <https://groups.google.com/forum/#!forum/edx-code>`_ or in the
 ``#edx-code`` IRC channel on Freenode.
```

### Comparing `edx-auth-backends-4.2.0/auth_backends/backends.py` & `edx-auth-backends-4.3.0/auth_backends/backends.py`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.2.0/auth_backends/pipeline.py` & `edx-auth-backends-4.3.0/auth_backends/pipeline.py`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.2.0/auth_backends/strategies.py` & `edx-auth-backends-4.3.0/auth_backends/strategies.py`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.2.0/auth_backends/tests/mixins.py` & `edx-auth-backends-4.3.0/auth_backends/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.2.0/auth_backends/tests/test_backends.py` & `edx-auth-backends-4.3.0/auth_backends/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.2.0/auth_backends/tests/test_pipeline.py` & `edx-auth-backends-4.3.0/auth_backends/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.2.0/auth_backends/tests/test_strategies.py` & `edx-auth-backends-4.3.0/auth_backends/tests/test_strategies.py`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.2.0/auth_backends/tests/test_views.py` & `edx-auth-backends-4.3.0/auth_backends/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.2.0/auth_backends/views.py` & `edx-auth-backends-4.3.0/auth_backends/views.py`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.2.0/edx_auth_backends.egg-info/PKG-INFO` & `edx-auth-backends-4.3.0/edx_auth_backends.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: edx-auth-backends
-Version: 4.2.0
+Version: 4.3.0
 Summary: Custom edX authentication backends and pipeline steps
 Home-page: https://github.com/openedx/auth-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Keywords: authentication edx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet
 License-File: LICENSE.txt
 License-File: AUTHORS
+Requires-Dist: Django
+Requires-Dist: pyjwt[crypto]>=2.1.0
+Requires-Dist: six
+Requires-Dist: social-auth-app-django
+Requires-Dist: social-auth-core
 
 auth-backends  |CI|_ |Codecov|_
 ===================================
 .. |CI| image:: https://github.com/openedx/auth-backends/workflows/Python%20CI/badge.svg?branch=master
 .. _CI: https://github.com/openedx/auth-backends/actions?query=workflow%3A%22Python+CI%22
 
 .. |Codecov| image:: http://codecov.io/github/edx/auth-backends/coverage.svg?branch=master
@@ -158,15 +164,15 @@
 Contributions are very welcome!
 
 Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Mailing List and IRC Channel
 ----------------------------
 
 You can discuss this code on the `edx-code Google Group <https://groups.google.com/forum/#!forum/edx-code>`_ or in the
 ``#edx-code`` IRC channel on Freenode.
```

### Comparing `edx-auth-backends-4.2.0/edx_auth_backends.egg-info/SOURCES.txt` & `edx-auth-backends-4.3.0/edx_auth_backends.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.2.0/setup.py` & `edx-auth-backends-4.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,17 +102,18 @@
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         'Topic :: Internet',
     ],
     keywords='authentication edx',
     url='https://github.com/openedx/auth-backends',
     author='edX',
     author_email='oscm@edx.org',
     license='AGPL',
```

